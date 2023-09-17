---
audience: end-user
title: 创建受众
description: 了解如何在Adobe Campaign Web中创建受众
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# 创建受众 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="受众"
>abstract="在此屏幕中，您可以创建受众并将受众组合到可视画布中。 添加各种工作流活动，例如 **Split** 或 **排除** 以生成新的和优化的受众。"

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="受众设置"
>abstract="输入受众的名称和其他选项，然后单击 **创建受众** 按钮。"

Campaign Web允许您在可视工作流画布中创建新受众。 除了从头开始创建简单的受众之外，您还可以利用工作流活动来优化受众。 例如，您可以将多个受众合并为单个受众、使用外部属性扩充受众，或将给定受众划分为多个受众。

创建工作流后，生成的受众将自动与现有受众一起存储在Campaign数据库中。 然后，可以在营销策划或独立投放中定位这些受众。

创建受众的主要步骤如下：

1. 创建受众工作流。
1. 配置构建受众活动，以根据您的需求查询数据库。
1. 添加工作流活动以优化受众（可选）。
1. 配置保存受众活动。
1. 运行工作流以将生成的受众保存到数据库。


## 创建您的第一个受众 {#create}

要创建受众，请执行以下步骤：

1. 导航至 **[!UICONTROL 受众]** 菜单，然后单击 **[!UICONTROL 创建受众]** 按钮进行标记。
1. 为受众提供标签。
1. 展开 **[!UICONTROL 其他选项]** 部分来配置高级受众参数。

   默认情况下，受众将创建到 **[!UICONTROL 配置文件和目标]** / **[!UICONTROL 列表]** 资源管理器菜单。 您可以使用更改默认存储位置 **[!UICONTROL 文件夹]** 字段。

   ![](assets/audiences-settings.png)

1. 配置受众设置后，单击 **[!UICONTROL 创建受众]** 按钮。

1. 此时会显示一个工作流画布，其中包含两个默认活动：

   * **[!UICONTROL 构建受众]**：这是工作流的起点，允许您创建受众，并将其用作工作流的基础。 [了解如何配置构建受众活动](../workflows/activities/build-audience.md)

   * **[!UICONTROL 保存受众]**：这是工作流中的最后一步，使您能够将结果另存为新受众。 [了解如何配置保存受众活动](../workflows/activities/save-audience.md)

1. 如果要在以下步骤之后执行附加操作： **[!UICONTROL 构建受众]** 活动，根据需要在工作流中添加所需数量的活动。 有关如何配置工作流活动的更多信息，请参阅 [工作流文档](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >渠道活动不可用于受众工作流。

   ![](assets/audience-creation-canvas.png)

1. 工作流准备就绪后，单击 **[!UICONTROL 开始]** 执行它。

1. 工作流将保存在中 **[!UICONTROL 工作流]** 列表，而生成的受众可在中访问 **[!UICONTROL 受众]** 列表。 [了解如何监测和管理受众](access-audiences.md)

## 受众工作流示例 {#example}

下方的示例显示了一个受众工作流，该工作流配置为定向生活在纽约的女客户，并根据这些客户在“瑜伽”或“奔跑”装备中的兴趣中心创建两个新受众。 这两个受众中增加了与客户购买相关的其他信息。

添加屏幕快照

1. 构建受众活动，可定向居住在纽约的所有女性用户档案。
1. 扩充活动通过Purchases表中的属性来丰富受众。
1. 拆分活动根据客户的兴趣中心将工作流分为两个路径。
1. 位于每个路径末尾的Save audience活动可将每个受众保存到数据库中。
