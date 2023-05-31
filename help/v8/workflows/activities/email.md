---
audience: end-user
title: 使用电子邮件工作流活动
description: 了解如何使用电子邮件工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 6af0b460a3c81f063a855b2fabba221b43e4ebb9
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 10%

---


# 电子邮件 {#email}

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow

-->


利用电子邮件投放活动，可在工作流中配置发送电子邮件。

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

同一工作流中的上游活动，通过受众定位活动定义了电子邮件收件人。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
