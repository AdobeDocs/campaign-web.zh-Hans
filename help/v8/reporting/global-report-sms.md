---
audience: end-user
title: 短信渠道全局报表
description: 了解短信渠道的全局报告
badge: label="有限发布版"
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 31%

---

# 短信渠道全局报表 {#campaign-reports-sms}

全局报告可在渠道级别为用户提供流量和参与量度的全面概述。

导航至 **[!UICONTROL 报表]** 中的菜单 **[!UICONTROL 报表]** 部分。 您可以根据报表日期、文件夹或规则过滤数据。 [了解详情](global-reports.md)

## 投放摘要 {#delivery-summary-sms}

### 投放概述 {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="短信投放概述"
>abstract="**短信投放概述** KPI 提供了短信投放的全面摘要，其中提供了详细的见解和具体数据。它提供了有关投放的效果、有效性和结果的全面信息。"

此 **[!UICONTROL 投放概述]** 报告提供全面的关键绩效指标(KPI)，可深入分析访客与每个短信投放的交互模式。 以下列出了以下量度。

![](assets/global_report_sms_delivery_overview.png)

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备期间处理的消息总数。

* **[!UICONTROL 已投放]**：成功发送的消息数占已发送消息总数的百分比。

* **[!UICONTROL 点进率]**：在投放中至少点击一次的不同收件人的百分比。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误数相对于已发送消息总数的百分比。

+++

### 目标受众 {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="短信目标群体"
>abstract="**目标群体**&#x200B;图表显示与您的短信受众相关的数据，包括有关要投放的消息和排除项的信息。"

此 **[!UICONTROL 目标受众]** 表格和图形可显示每个已发送短信投放的与收件人相关的数据。 指标详见下文。

![](assets/global_report_sms_targeted_audience.png)

+++了解有关目标受众量度的更多信息。

* **[!UICONTROL 目标受众]**：定向收件人总数。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 排除项]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

### 投放统计信息 {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="短信投放统计信息"
>abstract="**投放统计信息**&#x200B;报告提供了对已发送短信的全面见解，其中包含各种指标的细分，例如成功率、错误发生率和被隔离的受众。可根据此详细演示，全面检查短信投放过程的整体绩效和结果。"

此 **[!UICONTROL 投放统计信息]** 表详细列出了每次短信投放的成功情况。 指标详见下文。

![](assets/global_report_sms_delivery_statistics.png)

+++了解有关投放统计量度的更多信息。

* **[!UICONTROL 消息总数]**：投放准备后要投放的消息总数。

* **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

* **[!UICONTROL 错误/退回]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

* **[!UICONTROL 新隔离]**：在失败的投放（用户未知、域无效）后隔离的地址总数，与要投放的消息数相关。

  短信错误类型列在 [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### 排除原因 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="短信排除原因"
>abstract="**排除原因**&#x200B;图表说明了阻止用户配置文件接收短信消息的多种原因。"

此 **[!UICONTROL 排除的原因]** 图和表显示了阻止从定向用户档案中排除的用户用户档案接收短信投放的原因。

错误类型列在 [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## 投放吞吐量 {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="短信投放吞吐量"
>abstract="**投放吞吐量**&#x200B;报告提供了有关短信消息投放系统效率的广泛见解，详细概述了指定时间范围内的成功率和错误率。"

![](assets/global_report_sms_delivery_throughput.png)

此 **[!UICONTROL 投放吞吐量]** 报告提供了有关短信消息投放系统效率的全面见解，并提供了指定时间段内成功率和错误率的详细摘要。
