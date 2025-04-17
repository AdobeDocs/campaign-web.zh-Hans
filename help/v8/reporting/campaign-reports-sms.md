---
audience: end-user
title: 短信渠道的营销活动报告
description: 了解短信渠道的营销活动报告
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 15%

---

# 短信渠道的营销活动报告 {#campaign-reports-sms-channel}

每个营销活动报告都分为不同的小组件，其中详细说明了营销活动的成功和错误。 对于短信渠道，下文将详细介绍相关报表和量度。 在[此页面](campaign-reports.md)上了解如何访问您的营销活动报告。

## 投放摘要 {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="投放概述"
>abstract="**投放概述**&#x200B;报告提供详述访客如何与短信投放互动的关键绩效指标 (KPI)。"

**[!UICONTROL 投放概述]**&#x200B;报告提供了关键绩效指标(KPI)，这些指标提供有关访客如何参与短信投放的详细信息。 指标详见下文。

显示SMS量度的![投放概述报告](assets/campaign_report_sms_1.png){zoomable="yes"}

+++了解有关短信营销活动报告量度的更多信息。

* **[!UICONTROL 发送的总数]**：投放准备期间处理的邮件总数。

* **[!UICONTROL 已投放]**：成功发送的邮件数与已发送的邮件总数相关。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息的总数之比。

* **[!UICONTROL 非重复点击]**：在投放中至少点击一次的非重复收件人总数。

+++

### 初始目标受众统计信息 {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="初始目标受众统计信息"
>abstract="**初始目标受众统计信息**&#x200B;表显示与收件人相关的数据。"

**[!UICONTROL 初始目标受众统计信息]**&#x200B;表显示与收件人相关的数据。 指标详见下文。

![显示收件人数据的初始目标受众统计信息表](assets/campaign_report_sms_2.png){zoomable="yes"}

+++了解有关短信营销活动报告量度的更多信息。

* **[!UICONTROL 初始受众]**：目标收件人的总数。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* 列入阻止列表 **[!UICONTROL 被规则拒绝]**：应用规则时分析期间忽略的地址总数，例如地址缺失、隔离或。

+++

### 执行统计信息 {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="执行统计信息"
>abstract="**执行统计信息**&#x200B;表详述投放是否成功：要投放的消息数、成功数、错误数和新隔离数。"

**[!UICONTROL 执行统计信息]**&#x200B;表详细说明了您的交付是否成功。 指标详见下文。

![显示投放成功量度的执行统计信息表](assets/campaign_report_sms_3.png){zoomable="yes"}

+++了解有关短信营销活动报告量度的更多信息。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* **[!UICONTROL 成功]**：已成功处理的邮件数与要传递的邮件数相关。

* **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数相关。

* **[!UICONTROL 新隔离]**：在投放失败（用户未知，域无效）后隔离的地址总数，与要投放的消息数相关。

  [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}中列出了短信错误类型。

+++

### 生成的点击流 {#delivery-summary-sms-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="生成的点击流"
>abstract="**生成的点击流**&#x200B;表显示有关接收者与投放如何互动的可用数据。"

**[!UICONTROL 生成的点击流]**&#x200B;表显示与收件人与投放交互方式相关的数据。 指标详见下文。

![生成的显示收件人交互数据的点击流表](assets/campaign_report_sms_4.png){zoomable="yes"}

+++了解有关短信营销活动报告量度的更多信息。

* **[!UICONTROL 非重复点击]**：在投放中至少点击一次的非重复收件人总数。

* **[!UICONTROL 点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之比。

+++