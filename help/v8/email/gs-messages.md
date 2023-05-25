---
audience: end-user
title: 在 Campaign v8 Web 中开始使用消息和投放
description: 了解如何使用 Campaign Web 处理投放和发送消息
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 9f9b5b9ce08aa50986c75f1dd3afba8e2bc4f700
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 32%

---

# 在 Campaign Web 中开始使用消息 {#gs-messages}

借助Adobe Campaign，您可以发送跨渠道营销活动，包括电子邮件、短信和推送通知，并使用各种专用报告衡量其有效性。 这些消息通过投放设计和发送，并且可以针对每个收件人进行个性化。这些投放可以是独立的，也可以包含在营销活动上下文中。

Adobe Campaign v8 附带以下投放渠道：

* **电子邮件渠道**：电子邮件投放可让您向目标群体发送个性化电子邮件。了解如何在中创建和发送电子邮件 [此页面](../email/create-email.md).

* **短信渠道**：移动渠道中的投放可让您向目标群体发送个性化短信。  了解如何在中创建和发送短信 [此页面](../sms/create-sms.md).

* **移动应用程序渠道**：移动应用程序投放可让您向 iOS 和 Android 系统发送通知。了解如何在中创建和发送推送通知 [此页面](../push/gs-push.md).

## 创建投放

您可以从以下位置创建独立投放 **投放** 左侧菜单，或在营销活动上下文中创建投放，来自 **营销活动** 左侧菜单。

>[!BEGINTABS]

>[!TAB 创建独立投放]

要创建独立投放，请执行以下步骤：

1. 浏览至 **[!UICONTROL 投放]** 菜单，然后单击 **[!UICONTROL 创建投放]** 按钮。
1. 选择投放渠道。 要了解有关投放渠道以及如何定义投放内容的更多信息，请参阅以下部分：

   * [电子邮件渠道](../email/create-email.md)
   * [推送通知渠道](../push/gs-push.md)
   * [短信渠道](../sms/create-sms.md)

1. 为主要目标和控制组定义投放受众。 了解有关受众的更多信息，请参阅 [本节](../audience/about-audiences.md).
1. 定义消息内容。
1. （可选）定义投放计划。 如果未定义计划，则在单击 **[!UICONTROL 发送]** 按钮。
1. 单击  **[!UICONTROL 查看并发送]** 按钮以检查您的设置。
1. 使用  **[!UICONTROL 模拟内容]** 按钮以测试您的投放和个性化设置。 在中了解有关消息模拟的更多信息 [本节](../preview-test/preview-test.md).
1. 单击  **[!UICONTROL 准备]** 按钮以计算目标群体并生成消息。 准备步骤可能需要几分钟。 准备完成后，消息即可发送。 如果出现错误，请浏览 **日志** 以检查警报和警告。
1. 检查结果，然后单击  **[!UICONTROL 发送]** 按钮以开始发送消息。
1. 发送消息后，浏览到报表部分以访问关键量度。 要了解有关投放报告的更多信息，请参阅 [本节](../reporting/reports.md).

>[!TAB 在营销活动中创建投放]

要在营销策划中创建投放，请执行以下步骤：

1. 创建营销活动或打开现有营销活动。
1. 创建工作流或打开现有工作流。
1. 添加和配置 **构建受众** 活动，然后单击 `+`按钮。
   ![](assets/add-delivery-in-wf.png)
1. 选择投放活动：电子邮件、短信、推送通知(Android)或推送通知(iOS)。 要了解有关投放渠道以及如何定义投放内容的更多信息，请参阅以下部分：

   * [电子邮件渠道](../email/create-email.md)
   * [推送通知渠道](../push/gs-push.md)
   * [短信渠道](../sms/create-sms.md)

1. 启动工作流并检查日志。

有关如何配置营销活动的更多信息，

>[!ENDTABS]


## 选择发送消息的方式{#gs-send-msg}

创建消息并对其内容进行设计和测试后，您可以选择发送消息的方式。

Campaign 提供了一套功能用于：

* 手动将消息发送到主目标

* 发送与[营销活动](../campaigns/gs-campaigns.md)关联的消息

* 通过[工作流](../workflows/channel-activities.md)发送消息


## 添加个性化内容{#personalization}

通过Adobe Campaign投放的消息可以通过多种方式进行个性化


## 投放和跟踪日志{#gs-tracking-logs}

在发送后监测投放是确保营销活动有效并接触到客户的重要步骤。您可以在发送投放后进行监测，并了解如何管理投放失败和隔离。
