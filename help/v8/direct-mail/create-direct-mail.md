---
audience: end-user
title: 创建直邮投放
description: 了解如何使用Adobe Campaign Web创建直邮投放
exl-id: 9b5172b2-1880-4768-a33b-8a20ec5a30ab
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 19%

---

# 创建直邮投放 {#create-direct-mail}

您可以创建独立的直邮投放，也可以在活动工作流的上下文中创建直邮投放。 以下步骤详细介绍了独立（一次性）直邮投放的过程。 如果您在活动工作流的上下文中工作，有关创建步骤的详情，请参阅 [本节](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

要创建新的独立直邮投放，请执行以下步骤：

1. 浏览至 **[!UICONTROL 投放]** 菜单，然后单击  **[!UICONTROL 创建投放]** 按钮。

1. 在 **[!UICONTROL 渠道]** 部分，选择 **[!UICONTROL 直邮]** 作为渠道，并选择模板。 [了解有关模板的更多信息](../msg/delivery-template.md)

1. 单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮以进行确认。

   ![](assets/dm-create.png){zoomable="yes"}

1. 输入 **[!UICONTROL 标签]** ，并访问 **[!UICONTROL 其他选项]** 下拉菜单。 如果您的投放基于扩展模式，请指定 **自定义选项** 字段可用。

   ![](assets/dm-properties.png){zoomable="yes"}

   +++根据您的要求配置以下设置。
   * **[!UICONTROL 内部名称]**：为投放分配一个唯一标识符。
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中。
   * **[!UICONTROL 投放代码]**：使用您自己的命名惯例整理投放。
   * **[!UICONTROL 描述]**：提供投放的描述。
   * **[!UICONTROL 自然]**：指定投放的性质以进行分类。
+++

1. 单击 **[!UICONTROL 选择受众]** 按钮以定位现有受众或创建您自己的受众。

   * [了解如何选择现有受众](../audience/add-audience.md)
   * [了解如何创建新受众](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >直邮收件人必须至少包含其姓名和邮政地址。 如果名称、邮政编码字段和城镇/城市字段不为空，则认为地址完整。 将从直邮投放中排除任何地址不完整的收件人。

1. 打开 **[!UICONTROL 启用对照组]** 用于设置控制组以测量投放影响的选项。 消息不会发送到该控制组，因此您可以将收到消息的群体的行为与未收到消息的联系人的行为进行比较。 [了解如何使用对照组](../audience/control-group.md)

1. 单击 **[!UICONTROL 编辑内容]** 定义要导出到提取文件中的信息（列）。 [了解更多信息](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable="yes"}

1. 要安排在特定的日期和时间投放，请开启&#x200B;**[!UICONTROL 启用计划]**&#x200B;选项。启动投放后，提取文件将在您定义的确切日期和时间自动生成。 [了解如何计划投放](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >在工作流上下文中发送投放时，您必须使用 **计划程序** 活动。 请参阅[此页面](../workflows/activities/scheduler.md)以了解详情。

1. 单击 **[!UICONTROL 设置]** 访问与投放模板相关的高级选项。 [了解更多信息](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable="yes"}

1. 直邮投放就绪后，单击 **[!UICONTROL 审阅并发送]** 按钮以验证和发送投放并生成提取文件。 [了解如何预览和发送直邮投放](send-direct-mail.md)
