---
audience: end-user
title: 使用“合并工作流”活动
description: 了解如何使用“合并工作流”活动
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 100%

---


# 合并 {#combine}

此活动允许对集客群体进行分段。因此，您可以合并多个群体、排除其中的一部分或者仅保留多个目标共有的数据。下面显示了可用的分段类型：

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* **并集**&#x200B;可将多个活动的结果重组为单个目标。
* **交集**&#x200B;可仅在活动中保留不同集客群体的共有元素。
* **差集**&#x200B;可根据特定条件从一个群体中排除某些元素。

## 常规配置 {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="交集合并选项"
>abstract="交集可仅在活动中保留不同集客群体的共有元素。在“要加入的集合”部分中，选中您之前希望加入的所有活动。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="差集合并选项"
>abstract="差集可根据特定条件从一个群体中排除某些元素。在“要加入的集合”部分中，选中您之前希望加入的所有活动。"

请按照以下常见步骤操作，开始配置&#x200B;**合并**&#x200B;活动：

1. 添加多项活动（例如&#x200B;**生成受众**&#x200B;活动），来构成至少两个不同的执行分支。
1. 向先前的任何分支添加一个&#x200B;**合并**&#x200B;活动。
1. 选择分段类型：[并集](#union)、[交集](#intersection)或[差集](#exclusion)。
1. 单击&#x200B;**继续**。
1. 在&#x200B;**要加入的集合**&#x200B;部分中，选中您之前希望加入的所有活动。

## 并集 {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="交集协调选项"
>abstract="选择协调类型以定义如何处理重复项。"

对于&#x200B;**并集**，需要选择&#x200B;**协调类型**&#x200B;以定义如何处理重复项：

* **仅键值**：这是默认模式。当来自不同集客过渡的元素具有相同的键值时，该活动只保留一个元素。仅当集客群体具有同样的性质时，才能使用此选项。
* **选择的一组列**：选择此选项可定义要应用数据协调的列的列表。必须先选择主集（包含源数据的集），然后选择用于连接的列。

## 交集 {#intersection}

对于&#x200B;**交集**，您需要额外执行以下步骤：

1. 选择&#x200B;**协调类型**&#x200B;以定义如何处理重复项。请参阅[并集](#union)部分。
1. 如果您想处理剩余的人群，可以选中&#x200B;**生成补集**&#x200B;选项。补集将包含所有集客活动减去交集的结果的并集。然后，一个额外的叫客过渡将添加到活动中。

## 差集 {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="差集规则"
>abstract="必要时，您可以操作集客表。事实上，要从另一个维度排除一个目标，必须将该目标返回到与主目标相同的目标维度。为此，请单击“差集规则”部分中的“添加规则”，并指定维度更改条件。数据协调是通过属性或联接来执行的。"

对于&#x200B;**差集**，您需要额外执行以下步骤：

1. 在&#x200B;**要加入的集合**&#x200B;部分中，从集客过渡中选择&#x200B;**主集**。这是排除了元素的集合。其他集合用于匹配从主集中排除之前的元素。
1. 必要时，您可以操作集客表。事实上，要从另一个维度排除一个目标，必须将该目标返回到与主目标相同的目标维度。为此，请单击&#x200B;**差集规则**&#x200B;部分中的&#x200B;**添加规则**，并指定维度更改条件。数据协调是通过属性或联接来执行的。
1. 如果您想处理剩余的人群，可以选中&#x200B;**生成补集**&#x200B;选项。请参阅[交集](#intersection)部分。

## 示例

在下例中，我们添加了一个&#x200B;**并集**，用来检索以下两个查询的所有个人资料：18 至 27 岁之间的人员以及 34 至 40 岁之间的人员。

![](../assets/workflow-union-example.png)

下例展示了两个查询活动之间的&#x200B;**交集**。此处使用它来检索年龄在 18 至 27 岁之间且已提供电子邮件地址的人员的个人资料。

![](../assets/workflow-intersection-example.png)

下面的&#x200B;**差集**&#x200B;示例展示了两个查询，这两个查询配置为筛选出年龄在 18 岁到 27 岁之间且具有 Adobe 电子邮件域的人员的个人资料。随后，具有 Adobe 电子邮件域的个人资料将从第一个集合中排除。

![](../assets/workflow-exclusion-example.png)


