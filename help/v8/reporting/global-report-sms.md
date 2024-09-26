---
audience: end-user
title: 短信渠道全局报表
description: 了解短信渠道的全局报告
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 31%

---

# 短信渠道全局报表 {#campaign-reports-sms}

全局报告可在渠道级别为用户提供流量和参与量度的全面概述。

导航到&#x200B;**[!UICONTROL 报告]**&#x200B;部分中的&#x200B;**[!UICONTROL 报告]**&#x200B;菜单。 您可以根据报表日期、文件夹或规则过滤数据。 [了解详情](global-reports.md)

## 投放摘要 {#delivery-summary-sms}

### 投放概述 {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="短信投放概述"
>abstract="**短信投放概述** KPI 提供您的短信投放的全面摘要，并提供详细见解和具体数据。它提供有关您的投放的效果、有效性和成果的全面信息。"

**[!UICONTROL 投放概述]**&#x200B;报表提供了全面的关键绩效指标(KPI)，可深入分析访客与每个短信投放的交互模式。 以下列出了以下量度。

![](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的邮件]**：投放准备期间处理的邮件总数。

* **[!UICONTROL 已投放]**：成功发送的邮件占已发送邮件总数的百分比。

* **[!UICONTROL 点进率]**：在投放中至少点击一次的不同收件人的百分比。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误数占已发送邮件总数的百分比。

+++

### 目标受众 {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="短信目标群体"
>abstract="**目标群体**&#x200B;图和表展示与您的短信受众相关的数据，包括有关要投放的消息和排除项的信息。"

**[!UICONTROL 目标受众]**&#x200B;表和图表显示与每个已发送短信投放的收件人相关的数据。 指标详见下文。

![](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++了解有关目标受众量度的更多信息。

* **[!UICONTROL 目标受众]**：目标收件人的总数。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* **[!UICONTROL 排除]**：应用规则时在分析期间忽略的地址总数：地址缺失、隔离、列入阻止列表等。

+++

### 投放统计信息 {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="短信投放统计信息"
>abstract="通过&#x200B;**投放统计信息**&#x200B;报告可全面了解发送的短信，其中细分各种指标，如成功率、错误发生率和被隔离的受众。通过此详细演示可全面地检查短信投放过程的整体效果和成果。"

**[!UICONTROL 投放统计数据]**&#x200B;表详细说明了每次SMS投放的成功情况。 指标详见下文。

![](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++了解有关投放统计量度的更多信息。

* **[!UICONTROL 邮件总数]**：准备传递后要传递的邮件总数。

* **[!UICONTROL 成功]**：已成功处理的邮件数与要传递的邮件数相关。

* **[!UICONTROL 错误/退回]**：投放和自动回弹处理期间累计的错误总数与要投放的消息数相关。

* **[!UICONTROL 新隔离]**：在投放失败（用户未知，域无效）后隔离的地址总数与要投放的消息数相关。

  [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}中列出了短信错误类型。

+++

### 排除的原因 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="短信排除的原因"
>abstract="**排除的原因**&#x200B;图和表说明阻止用户轮廓接收短信的各种原因。"

**[!UICONTROL 排除原因]**&#x200B;图形和表格显示了阻止用户配置文件（已从目标配置文件中排除）接收短信投放的原因。

[Adobe Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}中列出了错误类型。

![](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## 投放吞吐量 {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="短信投放吞吐量"
>abstract="通过&#x200B;**投放吞吐量**&#x200B;报告可广泛了解短信投放系统的效率，并详细概述指定时间范围内的成功率和错误率。"

![](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

**[!UICONTROL 投放吞吐量]**&#x200B;报告提供了有关SMS消息投放系统有效性的全面见解，并提供了指定时间段内成功率和错误率的详细摘要。
