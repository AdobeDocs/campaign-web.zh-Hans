---
audience: end-user
title: 创建短信投放
description: 了解如何使用 Adobe Campaign Web 创建和发送短信
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 40%

---

# 创建短信投放 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="短信投放属性"
>abstract="这些属性包括常见的投放参数，可帮助您为投放命名和分类。如果您的投放使用扩展架构，则有专门的“自定义选项”字段可用。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="定义短信受众"
>abstract="创建新受众或通过单击&#x200B;**选择受众**&#x200B;按钮选择现有受众。如果需要，可添加对照组以衡量投放的影响力。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=zh-hans" text="设置对照组"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="短信模板选择"
>abstract="选择预定义模板以开始投放您的短信。通过投放模板，您可在各种营销活动和投放中重用自定义内容和设置。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=zh-hans" text="使用投放模板"

您可以创建独立的短信投放，或在活动工作流的上下文中创建短信。 以下步骤解释独立（一次性）短信投放的过程。 如果您在营销活动工作流的上下文中工作，将在[此部分](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow)中说明创建步骤。

要创建新的独立短信投放，请执行以下步骤：

1. 浏览到左边栏上的&#x200B;**[!UICONTROL 投放]**&#x200B;菜单，然后单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮。

1. 在&#x200B;**[!UICONTROL 渠道]**&#x200B;部分下，选择短信作为渠道，然后选择模板。 [了解有关模板的更多信息](../msg/delivery-template.md)

1. 单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮以进行确认。

   ![显示“创建投放”按钮和短信渠道选择的屏幕截图](assets/sms_create_1.png){zoomable="yes"}

1. 为投放输入&#x200B;**[!UICONTROL 标签]**&#x200B;并访问&#x200B;**[!UICONTROL 其他选项]**&#x200B;下拉列表。 如果您的投放使用扩展架构，则特定的&#x200B;**自定义选项**&#x200B;字段可用。

   +++根据您的要求配置以下设置。
   * **[!UICONTROL 内部名称]**：为投放分配一个唯一标识符。
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中。
   * **[!UICONTROL 投放代码]**：使用您自己的命名惯例整理投放。
   * **[!UICONTROL 描述]**：提供投放的描述。
   * **[!UICONTROL 性质]**：指定投放的性质以进行分类。
+++

1. 单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮以现有受众为目标或创建您自己的受众。[了解有关受众的详细信息](../audience/about-recipients.md)。

   ![显示“选择受众”按钮的屏幕截图](assets/sms_create_2.png){zoomable="yes"}

   了解如何在[此页面](../audience/add-audience.md)中选择现有受众。

   了解如何在[此页面](../audience/one-time-audience.md)中创建新受众。

1. 打开&#x200B;**[!UICONTROL 启用控制组]**&#x200B;选项，设置控制组以测量传递的影响。 消息不会发送到该控制组，因此您可以将收到消息的群体的行为与未收到消息的联系人的行为进行比较。 [了解详情](../audience/control-group.md)

1. 单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;开始设计短信消息的内容。 [了解详情](content-sms.md)

   ![显示“编辑内容”按钮的屏幕截图](assets/sms_create_4.png){zoomable="yes"}

   在此屏幕中，您还可以[模拟您的内容](../preview-test/preview-test.md)和[设置选件](../msg/offers.md)。

1. 要安排在特定的日期和时间投放，请开启&#x200B;**[!UICONTROL 启用计划]**&#x200B;选项。启动投放后，系统会在您为收件人定义的确切日期和时间自动发送消息。 在[本节](../msg/gs-deliveries.md#gs-schedule)中了解有关投放计划的更多信息。

   >[!NOTE]
   >
   >在工作流上下文中发送投放时，请使用&#x200B;**调度程序**&#x200B;活动。 请参阅[此页面](../workflows/activities/scheduler.md)以了解详情。

1. 单击&#x200B;**[!UICONTROL 设置]**&#x200B;可访问与您的投放模板相关的高级选项。 [了解详情](../advanced-settings/delivery-settings.md)

   ![显示“设置”按钮的屏幕截图](assets/sms_create_3.png){zoomable="yes"}