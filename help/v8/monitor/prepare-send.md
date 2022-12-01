---
audience: end-user
title: 准备和发送电子邮件
description: Campaign v8 Web文档
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 2%

---

# 准备并发送电子邮件 {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="准备并发送电子邮件"
>abstract="了解如何准备电子邮件，并了解有关发送KPI的更多信息。"

>[!NOTE]
>
>此文档正在构建中并且经常更新。 此内容的最终版本将于2023年1月准备就绪。

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 准备发送

在准备期间，将计算目标群体，并为目标中包含的每个用户档案生成消息内容。 准备完成后，即可立即发送消息，或者在计划的日期和时间发送消息。 分析过程中使用的验证规则如下所述 [部分](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. 单击 **准备** 按钮。

1. 将显示准备进度。 根据目标群体的大小，此操作可能需要一些时间。

   >[!NOTE]
   >
   >您可以随时使用 **停止准备** 按钮。 在准备阶段期间，不会发送任何消息。 因此，您可以启动或停止此操作，而不会产生任何影响。

1. 准备完成后，检查 **目标**, **交付** 和 **排除** KPI。 如果要发送的消息数与您的预期不符，请修改受众并重新开始准备。

1. 单击 **日志** 按钮，并检查没有错误。 列出了所有验证步骤、警告和错误。 彩色图标显示消息类型：

   * 灰色图标表示信息性消息。
   * 黄色图标表示非关键处理错误。
   * 红色图标表示阻止发送投放的严重错误。

1. 进行更改后，重新开始准备。

准备完成后，即可发送您的消息。 有关更多信息，请参阅确认发送。


## 发送消息

准备完成后，请按照以下步骤发送消息。

1. 单击 **“发送”按钮** 并确认。

1. 发送进度与三个KPI一起显示：送达、打开、单击。

1. 单击确定按钮以完成发送。

日志

>[!NOTE]
>
>如果已计划发送消息，则在到达发送时间时发送该消息。 有关计划发送消息的更多信息，请参阅此章节。

