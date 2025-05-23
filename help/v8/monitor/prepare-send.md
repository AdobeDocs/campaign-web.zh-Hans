---
audience: end-user
title: 准备并发送电子邮件
description: 了解如何使用Campaign Web用户界面准备和发送电子邮件
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 31%

---

# 准备并发送您的电子邮件 {#prepare-send}

## 准备发送 {#prepare}

当您定义[内容](../email/edit-content.md)、[受众](../audience/add-audience.md)和[计划](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule)时，您已准备好准备电子邮件投放。

在投放准备期间，会计算目标群体，并为目标中包含的每个用户档案生成消息内容。 完成准备工作后，即可立即或在安排的日期和时间发送消息。

在[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html?lang=zh-Hans){target="_blank"}中介绍了投放准备期间使用的验证规则。

下面列出了准备发送的主要步骤。

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 审阅并发送]**。

   传递仪表板中的![审阅并发送按钮](assets/email-review-and-send.png){zoomable="yes"}

1. 单击右上角的&#x200B;**[!UICONTROL 准备]**&#x200B;按钮，然后进行确认。

   传递仪表板中的![准备按钮](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >如果您计划了投放并禁用了&#x200B;**[!UICONTROL 发送前启用确认]**&#x200B;选项，则准备和发送步骤将分组到&#x200B;**[!UICONTROL 准备和发送]**&#x200B;按钮下。 [了解有关计划的更多信息](../msg/gs-deliveries.md#gs-schedule)

1. 这将显示准备进度。根据目标人群的规模，此操作可能需要花费一些时间。

   您可以使用&#x200B;**[!UICONTROL 停止准备]**&#x200B;按钮随时停止准备。

   投放仪表板中的![停止准备按钮](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >在准备阶段，不发送任何邮件。您可以启动或停止此操作，而不会影响任何内容。

1. 准备完成后，检查KPI。 如果要发送的邮件数不符合您的期望，请修改您的受众并重新开始准备。

   显示KPI的![准备完成屏幕](assets/email-preparation-complete.png){zoomable="yes"}

   以下是显示的不同 KPI：

   * **[!UICONTROL 目标]**：目标收件人的数量。
   * **[!UICONTROL 投放]**：将发送的邮件数。
   * **[!UICONTROL 排除]**：[分类规则](../advanced-settings/delivery-settings.md#typology)排除的消息数。

1. 单击“**[!UICONTROL 日志]**”按钮，然后检查是否存在错误。 最后一条日志消息显示了所有错误消息和错误数。[了解详情](delivery-logs.md)

   投放仪表板中的![日志按钮](assets/email-prepare-logs.png){zoomable="yes"}

1. 如果准备阶段检测到阻止发送投放的严重错误，则准备状态在投放仪表板中显示为失败。

   传递仪表板中的![错误状态](assets/email-prepare-error.png){zoomable="yes"}

1. 如果在准备之后对投放进行了任何更改，请重新启动准备工作，以便将这些更改考虑在内。

完成准备工作且无错误后，即可发送消息。

## 发送邮件 {#send}

[准备](#prepare)完成后，您可以发送电子邮件。

如果消息是按计划发送的，则会在定义的日期和时间发送该消息。 [了解有关计划的更多信息](../msg/gs-deliveries.md#gs-schedule)

### 立即发送 {#send-immediately}

要立即发送电子邮件，请执行以下步骤。

1. 在投放仪表板中，单击右上角的&#x200B;**[!UICONTROL 发送]**&#x200B;按钮。

   投放仪表板中的![发送按钮](assets/email-send.png){zoomable="yes"}

1. 确认此操作以立即将消息发送到主目标。

1. 显示发送进度。

### 计划发送 {#schedule-the-send}

如果您安排在以后的日期和时间发送电子邮件，请按照以下步骤操作。

1. 在单击&#x200B;**[!UICONTROL 查看和发送]**&#x200B;按钮之前，请确保为电子邮件定义计划。 [了解有关计划的更多信息](../msg/gs-deliveries.md#gs-schedule)

1. 在投放仪表板中，单击右上角的&#x200B;**[!UICONTROL 按计划发送]**。

   ![投放仪表板中的“按计划发送”按钮](assets/email-send-as-scheduled.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 确认发送]**。 在计划日期将投放发送到主目标。

   >[!NOTE]
   >
   >如果禁用&#x200B;**[!UICONTROL 发送前启用确认]**&#x200B;选项，则准备和发送步骤将分组到&#x200B;**[!UICONTROL 准备和发送]**&#x200B;按钮下。 [了解有关计划的更多信息](../msg/gs-deliveries.md#gs-schedule)

## 暂停或停止发送 {#pause-stop-sending}

无论您是否计划了投放<!--TBC-->，在发送过程中，都可以随时执行两个操作：

* 单击&#x200B;**[!UICONTROL 暂停发送]**&#x200B;可中断消息的发送。 您可以随时恢复发送。

* 单击&#x200B;**[!UICONTROL 停止发送]**&#x200B;可立即中断发送。 一旦停止，准备工作和发送均无法恢复。

![在投放仪表板中暂停或停止发送按钮](assets/email-send-pause-or-stop.png){zoomable="yes"}

## 检查关键绩效指标 {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="已投放"
>abstract="成功送达的邮件数。该指示器每 5 分钟更新一次。显示的百分比是基于已发送邮件的总数计算所得。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="打开"
>abstract="打开的邮件数。该指示器每 5 分钟更新一次。显示的百分比是不同打开次数与已送达邮件数的比率。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="点击次数"
>abstract="在电子邮件中至少点击一次的收件人的数量。该指示器每 5 分钟更新一次。显示的百分比是不同单击次数与已送达邮件数的比率。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="已发送"
>abstract="投放分析期间处理的消息的总数。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="错误数"
>abstract="投放和自动返回处理期间累积的错误的总数与已发送消息总数有关。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"

发送完成后，您可以检查显示的KPI：

发送后显示![个KPI](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL 已发送]**：已送达的邮件数。 显示的百分比基于要投放的消息总数。

* **[!UICONTROL 已送达]**：成功送达的邮件数。显示的百分比是基于已发送邮件的总数计算所得。

* **[!UICONTROL 打开]**：打开的邮件数。显示的百分比是不同打开次数与已投放消息数的对比。

* **[!UICONTROL 点击次数]**：在电子邮件中至少点击一次的收件人数量。 显示的百分比是不同点击次数与已投放消息数的对比。

* **[!UICONTROL 错误]**：具有错误状态的电子邮件数。 显示的百分比是基于已发送邮件的总数计算所得。

>[!NOTE]
>
>投放开始后，所有指标每5分钟更新一次。 投放准备指标是实时的。

在[此页面](../reporting/kpis.md)上了解有关KPI的更多信息。

您也可以查看日志。[了解详情](delivery-logs.md)