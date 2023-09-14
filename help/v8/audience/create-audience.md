---
audience: end-user
title: 创建受众
description: 了解如何在Adobe Campaign Web中创建受众
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 1%

---


# 创建受众 {#create-audiences}

通过Campaign Web，您可以创建工作流以将现有受众合并到可视画布中，并利用各种活动（拆分、排除……）来创建新受众。

完成后，生成的受众将与现有受众一起保存在Campaign Web中，并可在独立投放或营销活动中利用它来定位个人。

## 创建您的第一个受众 {#create}

要创建受众，请执行以下步骤：

1. 导航至 **[!UICONTROL 受众]** 菜单并单击 **[!UICONTROL 创建受众]** 按钮进行标记。
1. 为受众提供标签。
1. 展开其他选项部分可为受众配置高级参数。

   >[!NOTE]
   >
   >默认情况下，受众会创建到Profiles and Targets / Lists explorer菜单中。 您可以在 **[!UICONTROL 文件夹]** 字段。

1. 配置受众设置后，单击 **[!UICONTROL 创建受众]** 按钮。

1. 此时将显示一个工作流画布，其中包含两个默认活动：

   * **[!UICONTROL 构建受众]**：工作流的起点。 此活动允许您选择一个或多个受众作为工作流的基础，
   * **[!UICONTROL 保存受众]**：工作流的最后一步。 此活动用于将工作流结果保存到新受众中。

1. 根据需要添加任意数量的活动，以配置工作流。 有关如何配置各种活动的更多信息，请参阅 [工作流文档](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >渠道活动不可用于受众工作流。

   ![](assets/audience-creation-canvas.png)

1. 工作流准备就绪后，单击 **[!UICONTROL 开始]** 执行它。

1. 工作流将保存到 **[!UICONTROL 工作流]** 列表以及生成的受众放入 **[!UICONTROL 受众]** 列表。 [了解如何监测和管理受众](access-audiences.md)
