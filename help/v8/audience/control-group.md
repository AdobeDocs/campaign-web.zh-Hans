---
audience: end-user
title: 设置对照组
description: 了解如何在 Campaign Web UI 中为您的消息设置对照组
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Alpha" type="Positive"
source-git-commit: fd9a5724aa9b97bffc6d143853742e0107bd3483
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 97%

---

# 设置对照组 {#control-group}

您可以使用对照组避免向部分受众发送消息，以便衡量活动的影响。

为此，可在定义投放受众时创建对照组。配置文件会随机、已筛选或未筛选或者根据条件添加到对照组中。之后，您可以将收到消息的目标人群的行为与非目标联系人的行为进行比较。

可以从主目标随机提取和/或从特定群体中选择该控制组。因此，有两种主要方法可定义控制组：

* 从主目标提取大量配置文件。
* 根据查询中定义的条件排除某些配置文件。

在定义对照组时，可以同时使用这两种方法。

在投放准备步骤中属于对照组的所有配置文件都将从主目标中删除。这些配置文件将不会收到消息。

要创建对照组，请从投放创建助手的&#x200B;**受众**&#x200B;部分中单击&#x200B;**[!UICONTROL 设置对照组]**&#x200B;按钮。

![](assets/control-group1.png)

>[!CAUTION]
>
>加载目标群体时不能使用对照组 [来自外部文件](file-audience.md).


## 从目标中提取 {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="从目标中提取"
>abstract="要定义对照组，您可以选择随机或基于排序从目标人群提取某个百分比或固定数量的配置文件。"

要定义对照组，您可以选择随机或基于排序从目标人群提取某个百分比或固定数量的配置文件。

首先，定义将从目标提取配置文件的方式：随机或基于排序。

在&#x200B;**从目标中提取**&#x200B;部分下方，选择一个&#x200B;**排除类型**：

* **随机**：在准备投放时，Adobe Campaign 将随机提取与百分比或与将设置为大小限制的最大数量对应的配置文件数。

   ![](assets/control-group.png)

* **按属性排名**：此选项使您能够根据特定属性按特定排序顺序排除一组配置文件。

   ![](assets/control-group2.png)

然后定义&#x200B;**大小限制**：您必须设置将如何限制从主目标中提取的配置文件数。

**示例**

您可以查看日志以检查和识别排除的配置文件。让我们以随机排除五个配置文件为例。

![](assets/control-group4.png)

投放准备后，您可以在以下屏幕上查看排除项：

* 发送前，投放仪表板中的&#x200B;**排除** KPI。

   ![](assets/control-group5.png)

* **排除日志**&#x200B;显示每个配置文件和相关的排除&#x200B;**原因**。

   ![](assets/control-group6.png)

* **排除原因**&#x200B;显示每个类型规则的排除配置文件数。

   ![](assets/control-group7.png)

有关投放日志的更多信息，请参阅此[章节](../monitor/delivery-logs.md)。

## 额外群体 {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="额外群体"
>abstract="定义对照组的另一种方法是通过使用现有受众或定义查询来从目标中排除特定群体。"

定义对照组的另一种方法是通过使用现有受众或定义查询来从目标中排除特定群体。

从&#x200B;**对照组**&#x200B;定义屏幕的&#x200B;**额外群体**&#x200B;部分中，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

![](assets/control-group3.png)

* 要使用现有受众，请单击&#x200B;**选择受众**。请参阅此[章节](add-audience.md)。

* 要定义新查询，请选择&#x200B;**创建您自己的**，并使用规则生成器定义排除标准。请参阅此[章节](segment-builder.md)。

将从目标中排除包含在受众中或与查询结果匹配的配置文件。