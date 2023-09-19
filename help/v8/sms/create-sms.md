---
audience: end-user
title: 创建短信投放
description: 了解如何使用 Adobe Campaign Web 创建和发送短信
badge: label="Beta"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: 8139ec2f1e94bebacd89ea64af88d0b0babb8781
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 72%

---

# 创建短信投放 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="短信投放属性"
>abstract="这些属性包含帮助您为投放命名和分类的常见投放参数。如果您的投放基于扩展架构，则有特定的“自定义选项”字段可用。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="定义短信受众"
>abstract="选择最适合您的短信消息的受众。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="短信模板选择"
>abstract="选择预定义模板以开始您的短信投放。"

您可以创建独立的短信投放，或在活动工作流的上下文中创建短信。 以下步骤详细介绍了独立（一次性）短信投放的过程。 如果您在活动工作流的上下文中工作，有关创建步骤的详细信息，请参阅 [本节](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


要创建新的独立短信投放，请执行以下步骤：

1. 浏览至 **[!UICONTROL 投放]** 菜单，然后单击  **[!UICONTROL 创建投放]** 按钮。

1. 在&#x200B;**[!UICONTROL 渠道]**&#x200B;部分下，选择“短信”作为渠道并选择一个模板。[详细了解模板](../msg/delivery-template.md)

1. 单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮以进行确认。

   ![](assets/sms_create_1.png)

1. 输入投放的&#x200B;**[!UICONTROL 标签]**&#x200B;并访问&#x200B;**[!UICONTROL 其他选项]**&#x200B;下拉列表。

   +++根据您的要求配置以下设置。
   * **[!UICONTROL 内部名称]**：为投放分配一个唯一标识符。
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中。
   * **[!UICONTROL 投放代码]**：使用您自己的命名惯例整理投放。
   * **[!UICONTROL 描述]**：提供投放的描述。
   * **[!UICONTROL 性质]**：指定电子邮件的性质以进行分类。
+++

1. 单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮以现有受众为目标或创建您自己的受众。[了解详情](../audience/about-recipients.md)。

   ![](assets/sms_create_2.png)

1. 开启&#x200B;**[!UICONTROL 启用对照组]**&#x200B;选项以设置对照组以衡量投放的作用，并使您可比较收到消息的人群的行为与未收到消息的联系人的行为。[了解详情](../audience/control-group.md)

1. 单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;以开始设计短信消息的内容。[了解详情](content-sms.md)

   ![](assets/sms_create_4.png)

   在此屏幕中，您还可以 [模拟您的内容](../preview-test/preview-test.md) 和 [设置优惠](../content/offers.md).

1. 要安排在特定的日期和时间投放，请开启&#x200B;**[!UICONTROL 启用计划]**&#x200B;选项。开始投放后，将在您为收件人定义的确切日期和时间自动发送消息。在中了解有关投放计划的更多信息 [本节](../msg/gs-messages.md#gs-schedule).

1. 单击 **[!UICONTROL 配置投放设置]** 访问与投放模板相关的高级选项。 [了解详情](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
