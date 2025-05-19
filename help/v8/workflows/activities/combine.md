---
audience: end-user
title: 使用“合并工作流”活动
description: 了解如何使用“合并工作流”活动
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 61%

---

# 合并 {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="合并活动"
>abstract="通过&#x200B;**合并**&#x200B;活动，可对集客群体执行分段。您可以合并多个群体、排除其中的一部分或者仅保留多个目标共有的数据。"

**合并**&#x200B;活动是&#x200B;**定位**&#x200B;活动。 此活动允许对集客群体进行分段。您可以合并多个群体，排除其中一部分群体，或者仅保留多个目标共有的数据。 下面显示了可用的分段类型：

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* **Union**&#x200B;将多个活动的结果重组为单个目标。
* **交集**&#x200B;仅保留活动中不同集客群体的共有元素。
* **差集**&#x200B;根据特定条件从一个群体中排除了某些元素。

## 配置合并活动 {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="交集合并选项"
>abstract="交集仅包含活动中不同集客群体的共有元素。在“要加入的集合”部分中，选中您之前希望加入的所有活动。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="差集合并选项"
>abstract="差集根据特定条件从一个群体中排除了某些元素。在“要加入的集合”部分中，选中您之前希望加入的所有活动。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="选择分段类型"
>abstract="选择如何合并受众。**并集**&#x200B;将多个活动的结果重组为单个目标。**交集**&#x200B;仅包含活动中不同集客群体的共有元素。**差集**&#x200B;根据特定条件从一个群体中排除了某些元素。"

按照以下常用步骤配置&#x200B;**合并**&#x200B;活动：

![](../assets/workflow-combine.png)

1. 添加多个活动（如&#x200B;**构建受众**&#x200B;活动）以形成至少两个不同的执行分支。
1. 向先前的任何分支添加一个&#x200B;**合并**&#x200B;活动。
1. 选择分段类型： [联合](#union)、[交集](#intersection)或[排除](#exclusion)。
1. 单击&#x200B;**继续**。
1. 在&#x200B;**设置为加入**&#x200B;部分中，检查您之前希望加入的所有活动。

## 并集 {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="协调选项"
>abstract="选择&#x200B;**协调类型**&#x200B;以定义如何处理重复项。默认情况下，**键**&#x200B;选项处于激活状态，这意味着当来自不同入站过渡的元素具有相同的键时，该活动仅会保留一个元素。使用&#x200B;**选择列**&#x200B;选项定义应用数据协调的列的列表。"

在&#x200B;**组合**&#x200B;活动中，通过选择&#x200B;**协调类型**&#x200B;来配置&#x200B;**联合**&#x200B;以定义如何处理重复项：

* **仅键**：这是默认模式。 当来自不同集客过渡的元素具有相同的键值时，该活动仅保留一个元素。 仅当集客群体具有同样的性质时，才能使用此选项。
* **选择的列**：选择此选项可定义应用数据协调的列的列表。 首先，选择主集（源数据），然后选择要用于连接的列。

## 交集 {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="交叉协调选项"
>abstract="选择&#x200B;**协调类型**&#x200B;以定义如何处理重复项。默认情况下，**键**&#x200B;选项处于激活状态，这意味着当来自不同入站过渡的元素具有相同的键时，该活动仅会保留一个元素。使用&#x200B;**选择列**&#x200B;选项定义应用数据协调的列的列表。"

在&#x200B;**合并**&#x200B;活动中，按照以下额外步骤配置&#x200B;**交叉点**：

1. 选择&#x200B;**协调类型**&#x200B;以定义如何处理重复项。请参阅[并集](#union)部分。
1. 如果要处理剩余群体，请选中&#x200B;**生成补码**&#x200B;选项。 补数包含所有集客活动结果的并集减去交集。 然后，向活动中添加其他叫客过渡。

## 差集 {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="差集规则"
>abstract="必要时，操作集客表。要从另一个维度排除一个目标，将该目标返回到与主目标相同的定位维度。单击“差集规则”部分中的“添加规则”，并指定维度更改条件。数据协调是通过属性或联接来执行的。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="选择要合并的集合"
>abstract="在&#x200B;**要加入的集合**&#x200B;部分中，从集客过渡中选择&#x200B;**主集**。这是排除了元素的集合。其他集合用于匹配从主集中排除之前的元素。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="差集规则"
>abstract="必要时，操作集客表。要从另一个维度排除一个目标，将该目标返回到与主目标相同的定位维度。单击“差集规则”部分中的“添加规则”，并指定维度更改条件。数据协调是通过属性或联接来执行的。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="合并生成补集"
>abstract="开启“生成补集”选项以在额外的过渡中处理剩余群体。"

在&#x200B;**合并**&#x200B;活动中，按照以下额外步骤配置&#x200B;**排除项**：

1. 在&#x200B;**要加入的集合**&#x200B;部分中，从集客过渡中选择&#x200B;**主集**。这是排除了元素的集合。其他集合用于匹配从主集中排除之前的元素。
1. 必要时，操作集客表。要从另一个维度排除一个目标，将该目标返回到与主目标相同的定位维度。在&#x200B;**排除规则**&#x200B;部分中单击&#x200B;**添加规则**&#x200B;并指定维度更改条件。 数据协调是通过属性或联接来执行的。
1. 如果要处理剩余群体，请选中&#x200B;**生成补码**&#x200B;选项。 请参阅[交集](#intersection)部分。

## 示例 {#combine-examples}

在下面的示例中，**Combine**&#x200B;活动使用&#x200B;**Union**&#x200B;检索两个查询的所有用户档案：18至27岁的人和34至40岁的人。

![](../assets/workflow-union-example.png)

以下示例显示两个查询活动之间的&#x200B;**交集**。 它会检索年龄在18到27岁之间且提供了电子邮件地址的用户档案。

![](../assets/workflow-intersection-example.png)

以下&#x200B;**排除项**&#x200B;示例显示了两个查询，配置为筛选18到27岁之间且具有Adobe电子邮件域的用户档案。 第一组中排除了具有Adobe电子邮件域的用户档案。

![](../assets/workflow-exclusion-example.png)