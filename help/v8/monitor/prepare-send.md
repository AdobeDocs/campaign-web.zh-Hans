---
audience: end-user
title: 准备并发送电子邮件
description: 了解如何使用Campaign Web用户界面准备和发送电子邮件
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: c3148c9593aa4d323097135601616b9c43bae378
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 38%

---


# 准备并发送您的电子邮件 {#prepare-send}

## 准备发送 {#prepare}

当您定义了[内容](../email/edit-content.md)、[受众](../audience/add-audience.md)和[计划](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule)后，您就可以准备电子邮件投放了。

在投放准备期间，将计算目标群体并为目标中包含的每个用户档案生成消息内容。 完成准备工作后，即可立即或在安排的日期和时间发送消息。

在[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html){target="_blank"}中介绍了投放准备期间使用的验证规则。

下面列出了准备发送的主要步骤。

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 审阅并发送]**。

   ![](assets/email-review-and-send.png){zoomable="yes"}


1. 单击右上角的&#x200B;**[!UICONTROL 准备]**&#x200B;按钮并确认。

   ![](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >如果您计划了投放并禁用了&#x200B;**[!UICONTROL 发送前启用确认]**&#x200B;选项，则准备和发送步骤将分组到&#x200B;**[!UICONTROL 准备和发送]**&#x200B;按钮下。 [了解有关计划的更多信息](../msg/gs-deliveries.md#gs-schedule)

1. 这将显示准备进度。根据目标人群的规模，此操作可能需要花费一些时间。

   您可以使用&#x200B;**[!UICONTROL 停止准备]**&#x200B;按钮随时停止准备。

   ![](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >在准备阶段，不发送任何邮件。因此，您可以开始或停止准备而不影响任何内容。

1. 在准备完成后，检查 KPI。如果要发送的邮件数不符合您的期望，请修改您的受众并重新开始准备。

   ![](assets/email-preparation-complete.png){zoomable="yes"}

   以下是显示的不同 KPI：

   * **[!UICONTROL 目标]**：目标收件人的数量。
   * **[!UICONTROL 投放]**：将发送的邮件数。
   * **[!UICONTROL 排除]**：[分类规则](../advanced-settings/delivery-settings.md#typology)排除的消息数。

1. 单击&#x200B;**[!UICONTROL 日志]**&#x200B;按钮并检查确认没有错误。最后一条日志消息显示了所有错误消息和错误数。[了解详情](delivery-logs.md)

   ![](assets/email-prepare-logs.png){zoomable="yes"}

1. 如果准备阶段检测到阻止发送投放的严重错误，则准备状态在投放仪表板中显示为失败。

   ![](assets/email-prepare-error.png){zoomable="yes"}

1. 如果在准备之后对投放进行了任何更改，则必须重新开始准备以将这些更改考虑在内。

完成准备工作且无错误后，即可发送消息。

## 发送邮件 {#send}


[准备](#prepare)完成后，您现在可以发送电子邮件。

如果消息是按计划发送的，则会在定义的日期和时间发送该消息。 [了解详情](../msg/gs-deliveries.md#gs-schedule)

### 立即发送 {#send-immediately}

要立即发送电子邮件，请执行以下步骤。

1. 在投放仪表板中，单击右上角的&#x200B;**[!UICONTROL 发送]**&#x200B;按钮。

   ![](assets/email-send.png){zoomable="yes"}

1. 确认此操作以立即将消息发送到主目标。

1. 显示发送进度。

### 计划发送 {#schedule-the-send}

如果您计划稍后发送电子邮件，请按照以下步骤操作。

1. 在点击&#x200B;**[!UICONTROL 审阅并发送]**&#x200B;按钮之前，请确保为电子邮件定义了计划。 [了解详情](../msg/gs-deliveries.md#gs-schedule)

1. 在投放仪表板中，单击右上角的&#x200B;**[!UICONTROL 按计划发送]**&#x200B;按钮。

   ![](assets/email-send-as-scheduled.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 确认发送]**。 投放将在计划日期发送到主目标。

   >[!NOTE]
   >
   >如果您禁用了&#x200B;**[!UICONTROL 发送前启用确认]**&#x200B;选项，则准备和发送步骤将分组在&#x200B;**[!UICONTROL 准备和发送]**&#x200B;按钮下。 [了解有关计划的更多信息](../msg/gs-deliveries.md#gs-schedule)

## 暂停或停止发送 {#pause-stop-sending}

无论您是否计划了投放<!--TBC-->，在发送过程中，都可以随时执行两个操作：

* 单击&#x200B;**[!UICONTROL 暂停发送]**&#x200B;可中断消息的发送。 您可以随时恢复发送。

* 单击&#x200B;**[!UICONTROL 停止发送]**&#x200B;可立即中断发送。 一旦停止，准备工作和发送均无法恢复。

![](assets/email-send-pause-or-stop.png){zoomable="yes"}

## 检查 KPI {#check-kpis}

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
>abstract="在电子邮件中至少单击一次的收件人的数目。该指示器每 5 分钟更新一次。显示的百分比是不同单击次数与已送达邮件数的比率。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="已发送数指标"
>abstract="投放分析期间处理的消息的总数。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="错误数指标"
>abstract="投放和自动返回处理期间累积的错误的总数与已发送邮件总数有关。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/reports/kpis" text="了解关键绩效指标"


发送完成后，您可以检查显示的KPI：

![](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL 已发送]**：已送达的邮件数。 显示的百分比基于要投放的消息总数。

* **[!UICONTROL 已送达]**：成功送达的邮件数。显示的百分比是基于已发送邮件的总数计算所得。

* **[!UICONTROL 打开]**：打开的邮件数。显示的百分比是不同打开次数与已投放消息数的对比。

* **[!UICONTROL 点击次数]**：在电子邮件中至少点击一次的收件人数量。 显示的百分比是不同点击次数与已投放消息数的对比。

* **[!UICONTROL 错误]**：具有错误状态的电子邮件数。 显示的百分比是基于已发送邮件的总数计算所得。

>[!NOTE]
>
>在投放开始后，所有指标每 5 分钟更新一次。投放准备指标是实时的。

在[此页面](../reporting/kpis.md)中了解有关KPI的更多信息。

您也可以查看日志。[了解详情](delivery-logs.md)