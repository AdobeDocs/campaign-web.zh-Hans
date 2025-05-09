---
audience: end-user
title: 监控投放日志
description: 了解如何监控投放日志
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 55%

---

# 监控投放日志 {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="投放日志"
>abstract="投放日志显示发送的详细信息。日志中包含发送、已排除的目标及排除原因，以及打开和单击等跟踪信息的详情。"

准备投放并单击&#x200B;**发送**&#x200B;按钮后，浏览投放日志以检查警告、错误、状态、排除和跟踪数据。 可直接从消息仪表板访问这些日志。日志中包含发送、已排除的目标及排除原因，以及打开和单击等跟踪信息的详情。

要查看日志，请访问您的投放仪表板并单击&#x200B;**日志**&#x200B;按钮。

可以使用以下选项卡：

* [日志](#logs-tab)
* [投放](#deliveries-tab)
* [排除项](#exclusion-tab)
* [排除原因](#exclusion-causes)
* [跟踪的 URL](#tracked-urls)
* [跟踪](#tracking)

## 日志 {#logs-tab}

**日志**&#x200B;选项卡包含与投放和校样有关的所有消息。利用特定的图标，可识别错误或警告。

列出所有验证步骤、警告和错误。 彩色图标显示消息类型：

* 灰色图标表示信息性消息。
* 黄色图标表示非关键处理错误。
* 红色图标表示阻止发送投放的严重错误。 必须修复严重错误才能发送投放。

![日志选项卡显示验证步骤、警告和错误，并带有彩色图标指示消息类型。](assets/logs.png){zoomable="yes"}

## 投放 {#deliveries-tab}

**发送日志**&#x200B;选项卡提供了每次进行此投放的历史记录。此处保存了已发送消息的列表及其状态。您可通过该处查看每个收件人的投放状态。

![ “投放”选项卡显示已发送消息的历史记录及其状态。](assets/logs2.png){zoomable="yes"}

## 排除项 {#exclusion-tab}

**排除日志**&#x200B;选项卡列出了从目标中排除的所有消息，并说明了发送失败的原因。

![排除项选项卡列出了已排除的消息和发送失败的原因。](assets/logs3.png){zoomable="yes"}

## 排除原因 {#exclusion-causes-tab}

针对每种可能的原因，**排除原因**&#x200B;选项卡显示已从目标中排除的消息数。

![排除原因选项卡显示每个原因的排除消息数。](assets/logs4.png){zoomable="yes"}

## 跟踪的 URL {#tracked-urls-tab}

**跟踪的URL**&#x200B;选项卡重组已发送消息中包含的URL，包括其URL类型和源URL。

![跟踪的URL选项卡显示已发送消息中包含的URL、其类型和源URL。](assets/logs5.png){zoomable="yes"}

## 跟踪 {#tracking-tab}

**跟踪**&#x200B;选项卡列出了此次投放的跟踪历史记录。此选项卡显示已发送消息的跟踪数据，包括所有受Adobe Campaign跟踪的URL。

![跟踪选项卡，显示已发送消息的跟踪历史记录和数据。](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>如果未为投放启用跟踪，则不会显示此选项卡。