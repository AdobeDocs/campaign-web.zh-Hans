---
audience: end-user
title: 计划投放的发送
description: 了解如何计划投放
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 6%

---

# 计划投放的发送 {#schedule-sending}

您可以计划投放的发送。 这些步骤取决于它是独立（一次性）投放，还是您正在营销活动工作流的上下文中工作。

## 独立投放

对于独立投放，请直接在投放中计划日期和时间。 有关每种类型的投放，请参阅以下示例：电子邮件、短信和推送通知。

### 电子邮件 {#schedule-email-standalone}

要计划电子邮件投放的发送，请执行以下步骤：

1. 在投放属性的&#x200B;**[!UICONTROL 计划]**&#x200B;部分中，激活&#x200B;**[!UICONTROL 启用计划]**&#x200B;切换开关。

1. 设置所需的发送日期和时间，然后单击&#x200B;**[!UICONTROL 查看和发送]**&#x200B;按钮。

   ![激活计划并设置日期和时间](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>默认情况下，**[!UICONTROL 启用发送前确认]**&#x200B;选项处于启用状态。此选项要求您在安排的日期和时间发送投放之前确认发送。如果您需要在计划的日期和时间自动发送投放，请禁用此选项。
>

1. 检查计划是否正确，然后单击&#x200B;**[!UICONTROL 准备]**&#x200B;按钮。

![检查计划并准备投放](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. 准备完成后，即可发送消息。 显示投放的关键量度，包括目标人口总数、要投放的消息数量以及排除的收件人数量。 单击&#x200B;**[!UICONTROL 按计划发送]**&#x200B;按钮以确认将在计划的日期和时间将投放发送到主目标。

![确认按计划发送](assets/schedule-email-standalone-send.png){zoomable="yes"}

### 短信

要计划特定日期和时间的短信投放，请执行与电子邮件投放相同的步骤。 [请参阅上文](#schedule-email-standalone)。

![计划SMS投放](assets/schedule-sms-standalone.png){zoomable="yes"}

您还可以检查是否已应用计划：

![检查短信计划](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### 推送通知

要计划特定日期和时间的独立推送投放，请执行与电子邮件投放相同的步骤。 [请参阅上文](#schedule-email-standalone)。

![计划推送通知投放](assets/schedule-push-standalone.png){zoomable="yes"}

您还可以检查是否已应用计划：

![检查推送通知计划](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### 活动中的独立投放

您无需使用工作流，即可在营销策划中创建独立投放。 如上所述，为此投放设置日期和时间计划。 营销策划可能有自己的计划，包括开始日期和结束日期。 此计划不会干扰您的投放计划。

![营销活动中的独立投放](assets/schedule-delivery-standalone.png){zoomable="yes"}

## 在活动工作流中计划投放

在活动工作流的上下文中，最佳实践是使用&#x200B;**[!UICONTROL 调度程序]**&#x200B;活动来应用启动工作流的日期和时间，其中涉及发送投放。 [了解有关调度程序的详细信息](../workflows/activities/scheduler.md)。

![在活动工作流中计划投放](assets/schedule-workflow.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 调度程序]**&#x200B;活动中配置日期和时间。

![配置调度程序活动](assets/schedule-workflow-scheduler.png){zoomable="yes"}

>[!NOTE]
>
>当您使用&#x200B;**[!UICONTROL 调度程序]**&#x200B;活动安排在工作流中发送投放时，请勿在&#x200B;**[!UICONTROL 投放]**&#x200B;活动设置中激活&#x200B;**[!UICONTROL 启用计划]**&#x200B;切换开关。 您的投放将自动发送。
>

如果您在&#x200B;**[!UICONTROL 投放]**&#x200B;活动设置中激活&#x200B;**[!UICONTROL 启用计划]**&#x200B;切换并设置了日期和时间，则投放将在此日期和时间等待发送。 这意味着如果工作流启动日期和发送日期之间存在延迟，则受众可能不是最新状态。