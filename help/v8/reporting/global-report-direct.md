---
audience: end-user
title: 直邮渠道的全局报告
description: 详细了解直邮渠道的全局报告
badge: label="有限可用性"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 4%

---

# 直邮渠道的全局报告 {#global-report-direct}

全局报告可在渠道级别为用户提供流量和参与量度的全面概述。

导航至 **[!UICONTROL 报表]** 中的菜单 **[!UICONTROL 报表]** 部分。 您可以根据报表日期、文件夹或规则过滤数据。 [了解详情](global-reports.md)

## 投放摘要 {#delivery-summary-direct}

### 投放概述 {#delivery-overview-direct}

此 **[!UICONTROL 投放概述]** 提供关键绩效指标(KPI)，用于深入分析访客与每次电子邮件投放的交互情况。 这些指标概述如下。

![](assets/global_report_email_delivery_overview.png){align="center"}

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备期间处理的消息总数。

* **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

* **[!UICONTROL 取消订阅]**：点击取消订阅的收件人数量。
+++

### 目标受众 {#delivery-summary-direct-initial-target}

表和图表 **[!UICONTROL 目标受众]** 显示与收件人相关的数据，并提供以下详细量度。

![](assets/global_report_email_targeted_audience.png){align="center"}

+++了解有关目标受众量度的更多信息。

* **[!UICONTROL 目标受众]**：定向收件人总数。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 排除项]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

### 投放统计信息 {#delivery-summary-direct-exec-stats}

此 **[!UICONTROL 投放统计信息]** 该表提供了每次直邮投放成功的明细，详见下面列出的指标。

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++了解有关投放统计量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

* **[!UICONTROL 错误/退回]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

* **[!UICONTROL 新隔离]**：在失败的投放（用户未知、域无效）后隔离的地址总数，与要投放的消息数相关。

+++

### 排除原因 {#causes-exclusion}

![](assets/global_report_email_exclusions.png){align="center"}

排除项图表和表说明了阻止从目标用户档案排除的用户用户档案接收消息的原因。

## 投放吞吐量 {#delivery-throughput}

此报表提供有关指定时间范围内的投放吞吐量的全面详细信息。 用于测量消息投放速度的关键量度是每小时发送的消息数。

## 投放失败 {#non-deliverables-direct}

### 按类型细分错误 {#delivery-summary-direct-breakdown-per-type}

此 **[!UICONTROL 每种类型的错误细分]** 表和图表显示了与各个域中遇到的潜在错误相关的数据，具体指标如下所示。

此报告中显示的错误会触发隔离过程。 有关隔离管理的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++了解有关每个类型量度错误划分的更多信息。

* **[!UICONTROL 用户未知]**：投放期间生成的错误类型，指示地址无效。

* **[!UICONTROL 无效域]**：发送投放时生成的错误类型，指示地址的域错误或不存在。

* **[!UICONTROL 邮箱已满]**：在尝试投放五次后生成的错误类型，旨在指示收件人的收件箱中包含的消息过多。

* **[!UICONTROL 帐户已禁用]**：发送投放时生成的错误类型，指示地址不再存在。

* **[!UICONTROL 已拒绝]**：当IAP（互联网访问提供商）拒绝地址时生成的错误类型，例如，应用安全规则（反垃圾邮件软件）之后。

* **[!UICONTROL 不可到达]**：消息分发字符串中发生的错误类型：SMTP中继上的事件、域名暂时不可访问等

* **[!UICONTROL 未连接]**：错误类型，指示收件人的手机在发送时关闭或与网络断开连接。

+++

### 按域细分错误 {#delivery-summary-email-breakdown-per-domain}

此 **[!UICONTROL 每个域的错误细分]** 表格和图形展示了与每个域中潜在错误相关的数据。 指标与以下内容通用 **[!UICONTROL 每种类型的错误细分]** 表格和图形详见上文。

