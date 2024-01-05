---
audience: end-user
title: 推送渠道全局报表
description: 了解推送渠道的全局报表
badge: label="有限发布版"
source-git-commit: ac9a7918045e7ff02ef27c348b28a6ce09802caf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 4%

---

# 推送渠道全局报表 {#campaign-reports-push}

全局报告可在渠道级别为用户提供流量和参与量度的全面概述。

导航至 **[!UICONTROL 报表]** 中的菜单 **[!UICONTROL 报表]** 部分。 您可以根据报表日期、文件夹或规则过滤数据。 [了解详情](global-reports.md)

## 投放摘要 {#delivery-summary-push}

### 投放摘要 {#delivery-overview-push}

此 **[!UICONTROL 投放概述]** 报告提供关键绩效指标(KPI)，提供关于访客如何参与每个推送通知投放的详细信息。 指标详见下文。

![](assets/global_report_push_delivery_overview.png)

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备期间处理的消息总数。

* **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

* **[!UICONTROL 总点击次数]**：在投放中至少点击一次的不同收件人的总数。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

+++

### 目标受众 {#delivery-summary-push-initial-target}

此 **[!UICONTROL 目标受众]** 表格和图形可显示与每个已发送推送通知投放的收件人相关的数据。 指标详见下文。

![](assets/global_report_push_targeted_audience.png)

+++了解有关目标受众量度的更多信息。

* **[!UICONTROL 目标受众]**：定向收件人总数。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 排除项]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

### 投放统计信息 {#delivery-summary-push-exec-stats}

此 **[!UICONTROL 投放统计信息]** 表详细列出了每次推送通知投放的成功情况。 指标详见下文。

![](assets/global_report_push_delivery_statistics.png)

+++了解有关投放统计量度的更多信息。

* **[!UICONTROL 消息总数]**：投放准备后要投放的消息总数。

* **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

* **[!UICONTROL 错误/退回]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

* **[!UICONTROL 新隔离]**：投放失败后隔离的地址总数（注册无效、消息拒绝、有效负载错误等） 与要投放的消息数相关。

  推送通知错误类型列在 [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### 排除原因 {#causes-exclusion}

此 **[!UICONTROL 排除的原因]** 图形和表格可显示阻止从定向用户档案中排除的用户用户档案接收消息的原因。

推送通知错误类型列在 [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## 投放吞吐量 {#delivery-throughput-sms}

![](assets/global_report_push_delivery_throughput.png)

此报表提供有关指定时间范围内的投放吞吐量的全面详细信息。

