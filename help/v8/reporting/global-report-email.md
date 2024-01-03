---
audience: end-user
title: 电子邮件渠道的全局报告
description: 了解有关电子邮件渠道全局报告的更多信息
badge: label="有限可用性"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 4%

---

# 电子邮件渠道的全局报告 {#global-report-direct}

全局报告可在渠道级别为用户提供流量和参与量度的全面概述。

导航至 **[!UICONTROL 报表]** 中的菜单 **[!UICONTROL 报表]** 部分。 您可以根据报表日期、文件夹或规则过滤数据。 [了解详情](global-reports.md)

## 投放摘要 {#delivery-summary-email}

### 投放概述 {#delivery-overview-email}

此 **[!UICONTROL 投放概述]** 提供关键绩效指标(KPI)，用于深入分析访客与每次电子邮件投放的交互情况。 这些指标概述如下。

![](assets/global_report_email_delivery_overview.png){align="center"}

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备期间处理的消息总数。

* **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

* **[!UICONTROL 打开次数总计]**：至少打开过一次消息的目标收件人总数。

* **[!UICONTROL 总点击次数]**：在投放中至少点击一次的收件人总数。

* **[!UICONTROL 退回和错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

* **[!UICONTROL 取消订阅]**：点击取消订阅的收件人数量。
+++

### 目标受众 {#delivery-summary-email-initial-target}

表和图表 **[!UICONTROL 目标受众]** 显示与收件人相关的数据，并提供以下详细量度。

![](assets/global_report_email_targeted_audience.png){align="center"}

+++了解有关目标受众量度的更多信息。

* **[!UICONTROL 目标受众]**：定向收件人总数。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 排除项]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

### 投放统计信息 {#delivery-summary-email-exec-stats}

此 **[!UICONTROL 投放统计信息]** 该表提供了每个电子邮件投放成功的明细，详见下面列出的指标。

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

电子邮件错误类型列在 [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## 投放吞吐量 {#delivery-throughput}

![](assets/global_report_email_delivery_throughput.png){align="center"}

此报表提供有关指定时间范围内的投放吞吐量的全面详细信息。

## 投放失败 {#non-deliverables-email}

### 按类型细分错误 {#delivery-summary-email-breakdown-per-type}

![](assets/global_report_email_breakdown_type.png){align="center"}

此 **[!UICONTROL 每种类型的错误细分]** 表和图表显示了与各个域中遇到的潜在错误相关的数据，具体指标如下所示。

此报告中显示的错误会触发隔离过程。 有关隔离管理的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++了解有关每个类型量度错误划分的更多信息。

* **[!UICONTROL 用户未知]**：投放期间生成的错误类型，指示电子邮件地址无效。

* **[!UICONTROL 无效域]**：发送投放时生成的错误类型，指示电子邮件地址的域错误或不存在。

* **[!UICONTROL 邮箱已满]**：在尝试投放五次后生成的错误类型，旨在指示收件人的收件箱中包含的消息过多。

* **[!UICONTROL 帐户已禁用]**：发送投放时生成的错误类型，指示地址不再存在。

* **[!UICONTROL 已拒绝]**：当IAP（互联网访问提供商）拒绝地址时生成的错误类型，例如，应用安全规则（反垃圾邮件软件）之后。

* **[!UICONTROL 不可到达]**：消息分发字符串中发生的错误类型：SMTP中继上的事件、域名暂时不可访问等

* **[!UICONTROL 未连接]**：错误类型，指示收件人的手机在发送时关闭或与网络断开连接。

+++

### 按域细分错误 {#delivery-summary-email-breakdown-per-domain}

![](assets/global_report_email_breakdown_domain.png){align="center"}

此 **[!UICONTROL 每个域的错误细分]** 表格和图形展示了与每个域中潜在错误相关的数据。 指标与以下内容通用 **[!UICONTROL 每种类型的错误细分]** 表格和图形详见上文。

## 跟踪指标 {#tracking-indicators-email}

### 投放统计信息 {#delivery-summary-email-statistics}

此 **[!UICONTROL 投放统计信息]** 量度提供关键绩效指标(KPI)，用于提供有关与每个电子邮件投放关联的数据的详细信息。 有关这些指标的更多详细信息如下。

![](assets/global_report_email_delivery_statistics_tracking.png){align="center"}

+++了解有关投放统计量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备期间处理的消息总数。

* **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

* **[!UICONTROL 独特打开次数]**：至少打开过一次消息的目标收件人总数。

* **[!UICONTROL 打开次数总计]**：此域中至少打开过一次消息的不同目标收件人的数量。

* **[!UICONTROL 选择退出链接的点击量]**：取消订阅链接的点击次数。

* **[!UICONTROL 单击镜像链接]**：单击指向镜像页面的链接的次数。

* **[!UICONTROL 转发数量估计]**：估计目标收件人转发的电子邮件数量。
+++

### 打开和点进率 {#delivery-summary-open-rate}

此 **[!UICONTROL 打开率和点进率]** 表格会显示与收件人相关的数据。 指标详见下文。

![](assets/global_report_email_opens.png){align="center"}

+++了解有关打开率和点进率指标的更多信息。

* **[!UICONTROL 已发送]**：发送的消息总数。

* **[!UICONTROL 投诉]**：此域中已被收件人报告为不受欢迎的消息的数量和百分比。

* **[!UICONTROL 独特打开次数]**：此域中至少打开过一次消息的不同目标收件人的数量和百分比。

* **[!UICONTROL 独特点击]**：至少在同一个投放中点击过一次的不同目标收件人的数量和百分比。

* **[!UICONTROL 原始反应度]**：与至少打开一次投放的收件人数量相比，已至少点击一次投放的收件人数量的百分比。
+++

## URL 和点击流 {#url-email}

### URL和点击流KPI {#url-email-kpis}

此 **[!UICONTROL URL和点击流]** 报告提供关键绩效指标(KPI)，用于详细分析投放期间获得最多点击次数的URL。 指标详见下文。

![](assets/campaign_report_email_9.png){align="center"}

+++了解有关URL和点击流量度的更多信息。

* **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之间的比率。

* **[!UICONTROL 独特点击]**：在投放中至少点击一次的不同收件人的总数。

* **[!UICONTROL 总点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 平台平均值]** ：在每个比率（反应性、非重复点击和累计点击）下显示的平均比率，用于计算过去六个月发送的投放数量。 只考虑具有相同类型和相同渠道的投放。 排除验证。
+++

### 访问量排名前 10 的链接 {#top10-campaign-report-email}

此 **[!UICONTROL 前10个访问次数最多的链接]** 图形和表包含每个链接的收件人行为的可用数据。 指标详见下文。

![](assets/global_report_email_top10.png){align="center"}

+++了解有关10个最常访问的链接量度的更多信息。

* **[!UICONTROL 总点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 百分比]**：与投放交互的用户百分比。

+++

### 随时间推移的点击次数细分 {#campaign-report-email-breakdown-clicks}

此 **[!UICONTROL 随时间细分的点击量]** 图形包含每个链接的收件人行为的可用数据。

![](assets/global_report_email_breakdown_clicks.png){align="center"}

## 用户活动 {#user-activities-email}

此 **[!UICONTROL 用户活动]** 报告以图表的形式显示打开数和点击数的划分情况。 此报告的量度详述如下。

![](assets/global_report_email_user.png){align="center"}

+++了解有关用户活动量度的更多信息。

* **[!UICONTROL 总点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 打开次数总计]**：此域中至少打开过一次消息的不同目标收件人的总数。

+++
