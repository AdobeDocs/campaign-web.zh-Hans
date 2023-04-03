---
audience: end-user
title: 准备和发送电子邮件
description: 了解如何使用Campaign Web UI准备和发送电子邮件
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Alpha" type="Informitive"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 28%

---


# 准备并发送您的电子邮件 {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="准备并发送您的电子邮件"
>abstract="了解如何准备您的电子邮件，并了解有关发送关键绩效指标的更多信息。"

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 准备发送{#prepare}

定义内容、受众和计划后，您就可以准备消息。 在准备期间，将计算目标群体以及为目标中包含的每个用户档案生成的消息内容。 准备完成后，即可立即发送消息，或者在计划的日期和时间发送消息。 分析过程中使用的验证规则在 [Campaign Classicv7文档](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies){target="_blank"}.

按照下面的步骤进行操作：

1. 在投放仪表板中，单击 **准备** 按钮确认。

   ![](assets/prepare.png)

   将显示准备进度。 根据目标群体的大小，此操作可能需要一些时间。

   >[!NOTE]
   >
   >您可以随时使用 **停止准备** 按钮。 在准备阶段期间，不会发送任何消息。 因此，您可以启动或停止此操作，而不会产生任何影响。

1. 准备完成后，检查KPI。 如果要发送的消息数与您的预期不符，请修改受众并重新开始准备。

   ![](assets/prepare2.png)

   下面显示了不同的KPI:

   * **目标**:定向的收件人数量
   * **交付**:要发送的消息数
   * **排除**:分类规则排除的消息数

1. 单击 **日志** 按钮，并检查没有错误。 最后一个日志消息显示所有错误消息和错误数。 有关更多信息，请参阅[此章节](delivery-logs.md)。

   ![](assets/prepare-logs.png)

如果准备过程检测到阻止发送投放的关键错误，则投放仪表板中的准备状态将显示为失败。

![](assets/prepare-error.png)

如果您在准备之后需要对投放进行任何更改，则需要重新开始准备以考虑这些更改。

准备完成且无错误后，即可发送消息。 有关更多信息，请参阅[此章节](#send)。

## 发送消息{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="已送达"
>abstract="成功送达的邮件数。该指示器每 5 分钟更新一次。显示的百分比是基于已发送邮件的总数计算所得。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="打开"
>abstract="已打开消息的数量。 该指示器每 5 分钟更新一次。显示的百分比是不同打开次数与已送达邮件数的比率。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="单击次数"
>abstract="在电子邮件中至少单击一次的收件人的数目。该指示器每 5 分钟更新一次。显示的百分比是不同单击次数与已送达邮件数的比率。"


准备完成后，您现在即可发送消息。 只有立即发送的消息才需要此步骤。 如果消息已计划发送，则会在定义的日期发送。

请执行以下步骤：

1. 在投放仪表板中，单击 **发送** 按钮，然后确认。

   ![](assets/send.png)

1. 将显示发送进度。 检查显示的KPI。 您还可以检查日志。 有关更多信息，请参阅[此章节](delivery-logs.md)。

   ![](assets/send2.png)

   下面显示了不同的KPI:

   * **已交付**:成功投放的消息数。 显示的百分比是基于已发送邮件的总数计算所得。
   * **打开**:已打开消息的数量。 显示的百分比是不同打开次数与已送达邮件数的比率。
   * **点击次数**:在电子邮件中至少单击一次的收件人数。 显示的百分比是不同单击次数与已送达邮件数的比率。

   >[!NOTE]
   >
   >投放开始后，每5分钟更新一次所有指标。 投放准备指标是实时的。

   您可以随时暂停发送，然后继续。 如果在发送投放时停止投放，则无法继续。
