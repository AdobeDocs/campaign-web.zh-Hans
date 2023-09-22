---
audience: end-user
title: 创建受众
description: 了解如何在Adobe Campaign Web中创建受众
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 4%

---


# 创建受众 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="受众"
>abstract="在此屏幕中，您可以访问投放中可定位的所有受众的列表。 单击 **创建** 使用各种工作流活动(如 **Split** 或 **排除**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="受众设置"
>abstract="输入受众姓名和其他选项，然后单击&#x200B;**创建受众**&#x200B;按钮。"

Campaign Web允许您在可视工作流画布中创建新受众。 除了从头开始创建简单的受众之外，您还可以利用工作流活动来优化受众。 例如，您可以将多个受众合并为单个受众，使用外部属性丰富受众，或根据您选择的规则将受众划分为多个受众。

创建工作流后，生成的受众将自动与现有受众一起存储在Campaign数据库中。 然后，可以在工作流或独立投放中定位这些受众。

## 创建您的第一个受众 {#create}

要创建受众，请执行以下步骤：

1. 导航至 **[!UICONTROL 受众]** 菜单，然后单击 **[!UICONTROL 创建受众]** 按钮进行标记。
1. 为受众提供标签。
1. 展开 **[!UICONTROL 其他选项]** 部分来配置高级受众参数。

   默认情况下，受众将创建到 **[!UICONTROL 配置文件和目标]** / **[!UICONTROL 列表]** 资源管理器菜单。 您可以使用更改默认存储位置 **[!UICONTROL 文件夹]** 字段。

   ![](assets/audiences-settings.png)

1. 配置受众设置后，单击 **[!UICONTROL 创建受众]** 按钮。 此时会显示一个工作流画布，其中包含两个默认活动：

   * **[!UICONTROL 构建受众]**：这是工作流的起点，允许您创建受众，并将其用作工作流的基础。

   * **[!UICONTROL 保存受众]**：这是工作流的最后一步，让您能够将工作流结果另存为新受众。

1. 打开 **[!UICONTROL 构建受众]** 活动并使用规则生成器，通过过滤数据库中包含的数据来定义要包含在受众中的群体。 [了解如何配置构建受众活动](../workflows/activities/build-audience.md)

1. 如果想要对工作流中的定向群体执行其他操作，请根据需要添加尽可能多的活动，并将它们连接在一起。 有关如何配置工作流活动的更多信息，请参阅 [工作流文档](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >渠道活动不可用于受众工作流。

   ![](assets/audience-creation-canvas.png)

1. 配置 **[!UICONTROL 保存受众]** 活动，指定您希望如何保存工作流上游计算的群体。 [了解如何配置保存受众活动](../workflows/activities/save-audience.md)

1. 工作流准备就绪后，单击 **[!UICONTROL 开始]** 执行它。

工作流将保存在中 **[!UICONTROL 工作流]** 列表，而生成的受众可在中访问 **[!UICONTROL 受众]** 列表。 [了解如何监测和管理受众](manage-audience.md)

您现在可以使用此受众作为投放的主要目标。 [了解详情](add-audience.md)

## 受众工作流示例 {#example}

下方的示例显示了一个受众工作流，该工作流配置为定向居住在纽约的女客户，并根据他们最近购买过的物品（瑜伽或跑步装备）创建两个新受众。

![](assets/audiences-example.png)

1. 此 **[!UICONTROL 构建受众]** 活动针对居住在纽约的所有女性用户档案。
1. 此 **[!UICONTROL 扩充]** 活动通过“购买”表中的信息丰富了受众，以确定客户购买的产品类型。
1. 此 **[!UICONTROL Split]** 活动根据客户的最新购买情况将工作流分为两个路径。
1. 此 **[!UICONTROL 保存受众]** 每个路径末尾的活动会在数据库中创建两个新受众，其中包括每个路径中计算的群体。
