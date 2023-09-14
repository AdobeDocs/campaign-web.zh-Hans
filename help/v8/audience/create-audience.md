---
audience: end-user
title: 创建受众
description: 了解如何在Adobe Campaign Web中创建受众
badge: label="Beta"
source-git-commit: 1b17dcbdaadcbf45b2c26d9099e6d139143d253c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 1%

---


# 创建受众 {#create-audiences}

通过Campaign Web，您可以创建工作流并将现有受众合并到可视画布中。 通过合并各种工作流活动（如拆分或排除），可生成新的优化受众。

创建工作流后，生成的受众将自动与现有受众一起存储在Campaign Web中。 然后，可以在营销策划或独立投放中定位这些受众。

要创建受众，请执行以下步骤：

1. 导航至 **[!UICONTROL 受众]** 菜单，然后单击 **[!UICONTROL 创建受众]** 按钮进行标记。
1. 为受众提供标签。
1. 展开 **[!UICONTROL 其他选项]** 部分来配置高级受众参数。

   默认情况下，受众将创建到 **[!UICONTROL 配置文件和目标]** / **[!UICONTROL 列表]** 资源管理器菜单。 您可以使用更改默认存储位置 **[!UICONTROL 文件夹]** 字段。

   ![](assets/audiences-settings.png)

1. 配置受众设置后，单击 **[!UICONTROL 创建受众]** 按钮。

1. 此时会显示一个工作流画布，其中包含两个默认活动：

   * **[!UICONTROL 构建受众]**：这是工作流的起点，允许您创建受众，并将其用作工作流的基础。
   * **[!UICONTROL 保存受众]**：这是工作流中的最后一步，使您能够将结果另存为新受众。

1. 根据需要添加任意数量的活动，自定义您的工作流。 有关如何配置工作流活动的更多信息，请参阅 [工作流文档](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >渠道活动不可用于受众工作流。

   ![](assets/audience-creation-canvas.png)

1. 工作流准备就绪后，单击 **[!UICONTROL 开始]** 执行它。

1. 工作流将保存在中 **[!UICONTROL 工作流]** 列表，而生成的受众可在中访问 **[!UICONTROL 受众]** 列表。 [了解如何监测和管理受众](access-audiences.md)
