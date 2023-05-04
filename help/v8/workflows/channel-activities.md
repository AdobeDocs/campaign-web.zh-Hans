---
audience: end-user
title: 使用工作流渠道活动
description: 了解如何在Adobe Campaign Web工作流中使用渠道活动
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# 渠道活动 {#channel}

Adobe Campaign Web允许您跨多个渠道（如电子邮件、短信或推送）自动执行营销活动。 使用Adobe Campaign工作流，您可以将渠道活动组合到画布中，以创建跨渠道工作流，这些工作流可以根据客户行为触发操作。

例如，您可以创建一个欢迎电子邮件促销活动，该活动包含跨不同渠道的一系列消息，如电子邮件、短信和推送。 您还可以在客户完成购买后发送跟进电子邮件，或通过短信向客户发送个性化的生日消息。

通过使用渠道活动，您可以创建全面的个性化促销活动，以便跨多个接触点吸引客户并促进转化。

渠道活动在屏幕左侧的渠道部分的面板中可用。

## 电子邮件 {#email}

描述，您可以执行的用例（在活动之后可以链接的常见其他活动）

如何添加和配置活动

工作流中已配置活动的示例


利用电子邮件投放活动，可在工作流中配置发送电子邮件。

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

同一工作流中的上游活动，通过受众定位活动定义了电子邮件的收件人。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->