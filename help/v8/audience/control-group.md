---
audience: end-user
title: 设置对照组
description: 了解如何在Campaign Web用户界面中为消息设置控制组
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 21%

---

# 设置对照组 {#control-group}

控制组是从投放中排除的子群体。 您可以定义控制组以避免向部分受众发送消息，并将投放后的行为与主目标进行比较。 此选项有助于衡量活动的影响。

➡️ [通过观看视频了解此功能](create-audience.md#video)

## 启用对照组 {#add-a-control-group}

要添加控制组，请在定义投放受众时启用选项。 可以从主目标随机提取控制组或从特定群体中选择控制组。 因此，定义控制组的主要方法有两种：

* 从主目标提取大量轮廓。
* 从列表中或根据查询中定义的条件排除某些用户档案。

定义控制组时，可以合并这两种方法。

在投放准备步骤中控制组包含的所有用户档案都将从主目标中删除。 这些配置文件将不会收到消息。

>[!CAUTION]
>
>[从外部文件](file-audience.md)加载目标人群时，无法使用对照组。

要将控制组添加到投放，请从投放创建屏幕的&#x200B;**[!UICONTROL 受众]**&#x200B;部分激活&#x200B;**启用控制组**&#x200B;切换开关。

在投放创建屏幕上![启用控制组选项切换](assets/control-group1.png)

## 从目标中提取 {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="提取方式"
>abstract="对照组是从投放中排除的一组轮廓。要定义对照组，您可以选择随机或基于排序从目标人群提取某个百分比或固定数量的轮廓。"

### 构建对照组 {#build-extract-target}

要定义控制组，请选择随机或基于排序从目标群体提取某个百分比或固定数量的用户档案。 如果添加额外群体，请选择&#x200B;**无提取**&#x200B;选项，然后选择此处[详述的额外群体](#extra-population)。

首先，定义如何从目标提取用户档案：随机或基于排序。

在&#x200B;**控制组**&#x200B;部分下，选择&#x200B;**提取模式**：

* **随机**：在准备投放时，Adobe Campaign会随机提取与设置为大小限制的百分比或最大数量对应的用户档案数。
* **按属性排名**：此选项根据特定排序顺序中的特定属性排除一组配置文件。

然后，使用&#x200B;**大小限制**&#x200B;部分设置要从主目标提取的配置文件数。 它可以是原始数字（例如，要排除的50个用户档案）或初始受众的百分比（例如，主目标的5%）。

### 对照组样本 {#control-group-sample}

例如，要创建具有100个最新用户档案的控制组，请执行以下步骤：

1. 选择&#x200B;**年龄**&#x200B;字段作为排序条件。 保留&#x200B;**升序**&#x200B;排序选项。
1. 添加&#x200B;**创建日期**&#x200B;字段。 更改为&#x200B;**降序**&#x200B;排序选项。
1. 在&#x200B;**大小限制**&#x200B;部分中将100定义为阈值。

   最年轻配置文件的![控制组配置](assets/control-group2.png){zoomable="yes"}

然后，将从主目标中排除这100个最年轻的用户档案。

### 检查您的对照组 {#check-control-group}

查看日志以检查和识别排除的用户档案。 例如，假定随机排除五个用户档案。

![日志中排除的配置文件示例](assets/control-group4.png){zoomable="yes"}

在投放准备之后，查看排除项的应用方式：

* 在发送之前，在投放仪表板中，选中&#x200B;**要排除** KPI。

  ![显示“要排除”KPI的投放仪表板](assets/control-group5.png){zoomable="yes"}

* 在投放日志中， Logs选项卡显示排除步骤。

  ![显示排除步骤的投放日志](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* **排除原因**&#x200B;选项卡显示每个分类规则的排除配置文件数。

  ![排除原因选项卡显示类型规则排除](assets/control-group7.png){zoomable="yes"}

有关投放日志的更多信息，请参阅此[章节](../monitor/delivery-logs.md)。

## 添加额外群体 {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="额外群体"
>abstract="对照组是从投放中排除的一组轮廓。可通过选择现有受众或定义查询而从投放受众排除特定群体。"

定义控制组的另一种方法是选择现有受众中的特定群体或定义查询。

从&#x200B;**对照组**&#x200B;定义屏幕的&#x200B;**额外群体**&#x200B;部分中，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

![额外群体选择屏幕](assets/control-group3.png){zoomable="yes"}

* 要使用现有受众，请单击&#x200B;**选择受众**。可在[此部分](add-audience.md)中了解详情。
* 要定义新查询，请选择&#x200B;**创建您自己的查询**&#x200B;并使用查询建模器定义排除条件。 可在[此部分](../query/query-modeler-overview.md)中了解详情。

受众中包含的或与查询结果匹配的用户档案从投放目标中&#x200B;**排除**。 他们不会收到任何消息。

## 比较结果 {#control-group-results}

发送投放后，提取发送日志以比较未接收通信的用户档案和有效目标之间的行为。 使用投放日志构建新目标。

要查看从目标中删除了哪些用户档案，请检查&#x200B;**投放日志**。 在本节[中了解更多](#check-control-group)。