---
audience: end-user
title: 营销活动报告
description: 了解如何访问和使用营销活动报告
badge: label="Beta"
source-git-commit: f80a224665e8c70c2efce3af9a8f60a07fadd5dc
workflow-type: tm+mt
source-wordcount: '1853'
ht-degree: 2%

---

# 营销活动报告 {#campaign-reports}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="报告发送"
>abstract="报表中的“发送”选项卡可深入分析访客与投放的交互情况以及他们可能遇到的任何潜在错误。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="报告跟踪"
>abstract="报表中的“发送”选项卡提供了宝贵的数据，包括每个链接的收件人行为、打开和点击的细分，以及有关投放期间最常点击的URL的详细信息。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="投放概述"
>abstract="投放概述提供关键绩效指标(KPI)，用于提供有关访客如何参与电子邮件投放的详细信息。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="初始目标受众统计数据"
>abstract="初始目标受众统计信息表显示与收件人相关的数据"

营销活动报告分为多个不同的小组件，其中详细说明了营销活动的成功和错误。

此时将显示营销活动报告页面，其中包含以下选项卡：

* [电子邮件渠道](#email-channel)
* [短信渠道](#sms-channel)
* [推送渠道](#push-channel)

要访问您的营销活动报表，请在您的营销活动信息板中单击报表。

![](assets/campaign_report_email_13.png)

## 电子邮件渠道 {#email-channel}

### 投放摘要 {#delivery-summary-email}

* **[!UICONTROL 投放概述]** 提供关键绩效指标(KPI)，用于提供关于访客如何参与电子邮件投放的详细信息。

  ![](assets/campaign_report_email_1.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 发送总数]**：投放准备期间处理的消息总数。

   * **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

   * **[!UICONTROL 跳出次数]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

   * **[!UICONTROL 不同打开]**：至少打开过一次消息的目标收件人总数。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

+++

* **[!UICONTROL 初始目标受众统计信息]** 表格显示与收件人相关的数据：

  ![](assets/campaign_report_email_2.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 初始受众]**：定向收件人总数。

   * **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

   * **[!UICONTROL 被规则拒绝]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

* **[!UICONTROL 执行统计信息]** 表详细说明了您的交付是否成功。

  ![](assets/campaign_report_email_3.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

   * **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

   * **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

   * **[!UICONTROL 新隔离]**：在失败的投放（用户未知、域无效）后隔离的地址总数，与要投放的消息数相关。

+++

* **[!UICONTROL 反应统计信息]** 表包含投放的收件人活动的可用数据。

  ![](assets/campaign_report_email_4.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 不同打开]**：至少打开过一次消息的目标收件人总数。

   * **[!UICONTROL 打开次数]**：此域中至少打开过一次消息的不同目标收件人的数量。

   * **[!UICONTROL 取消订阅]**：在相关时段内点击取消订阅的收件人数量。

   * **[!UICONTROL 镜像页面]**：点击镜像页面链接的收件人数量。

   * **[!UICONTROL 转发]**：点击后转发电子邮件的收件人数量。
+++

* **[!UICONTROL 生成的点击流]** 该表显示了与收件人与投放的交互方式相关的数据。

  ![](assets/campaign_report_email_5.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

   * **[!UICONTROL 点击次数]**：投放中链接的点击总数。

   * **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之间的比率。

+++

### 投放失败 {#non-deliverables-email}

* **[!UICONTROL 每种类型的错误细分]** 和 **[!UICONTROL 每个域的错误细分]** 表和图形包含每个域可能遇到的错误的可用数据。

  此报告中显示的错误会触发隔离过程。 有关隔离管理的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

  ![](assets/campaign_report_email_6.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 用户未知]**：投放期间生成的错误类型，指示电子邮件地址无效。

   * **[!UICONTROL 无效域]**：发送投放时生成的错误类型，指示电子邮件地址的域错误或不存在。

   * **[!UICONTROL 邮箱已满]**：在尝试投放五次后生成的错误类型，旨在指示收件人的收件箱中包含的消息过多。

   * **[!UICONTROL 帐户已禁用]**：发送投放时生成的错误类型，指示地址不再存在。

   * **[!UICONTROL 已拒绝]**：当IAP（互联网访问提供商）拒绝地址时生成的错误类型，例如，应用安全规则（反垃圾邮件软件）之后。

   * **[!UICONTROL 不可到达]**：消息分发字符串中发生的错误类型：SMTP中继上的事件、域名暂时不可访问等

   * **[!UICONTROL 未连接]**：错误类型，指示收件人的手机在发送时关闭或与网络断开连接。

+++

### 跟踪指标 {#tracking-indicators-email}

* **[!UICONTROL 投放统计信息]** 提供关键绩效指标(KPI) ，用于提供关于已发送电子邮件可用数据的详细信息。

  ![](assets/campaign_report_email_7.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

   * **[!UICONTROL 不同打开]**：至少打开过一次消息的目标收件人总数。

   * **[!UICONTROL 打开次数]**：此域中至少打开过一次消息的不同目标收件人的数量。

   * **[!UICONTROL 选择退出链接的点击量]**：取消订阅链接的点击次数。

   * **[!UICONTROL 单击镜像链接]**：单击指向镜像页面的链接的次数。

   * **[!UICONTROL 转发数量估计]**：估计目标收件人转发的电子邮件数量。
+++

* **[!UICONTROL 初始目标受众统计信息]** 表格会显示与收件人相关的数据。

  ![](assets/campaign_report_email_8.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 已发送]**：发送的消息总数。

   * **[!UICONTROL 投诉]**：此域被收件人报告为不受欢迎的消息数。

   * **[!UICONTROL 打开次数]**：此域中至少打开过一次消息的不同目标收件人的数量。

   * **[!UICONTROL 点击次数]**：在同一个投放中至少点击一次的不同目标收件人的数量。

   * **[!UICONTROL 原始反应度]**：与至少打开一次投放的收件人数量相比，已至少点击一次投放的收件人数量的百分比。
+++

### URL 和点击流 {#url-email}

* **[!UICONTROL URL和点击流]** 提供关键绩效指标(KPI)，以详细了解投放期间点击次数最多的URL。

  ![](assets/campaign_report_email_9.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之间的比率。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

   * **[!UICONTROL 点击次数]**：投放中链接的点击总数。

   * **[!UICONTROL 平台平均值]** ：在每个比率（反应性、非重复点击和累计点击）下显示的平均比率，用于计算过去六个月发送的投放数量。 只考虑具有相同类型和相同渠道的投放。 排除验证。
+++

* **[!UICONTROL 前10个访问次数最多的链接]** 图形和表包含每个链接的收件人行为的可用数据。

  ![](assets/campaign_report_email_10.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 点击次数]**：投放中链接的点击总数。

   * **[!UICONTROL 百分比]**：与投放交互的用户百分比。

+++

* **[!UICONTROL 随时间细分的点击量]** 图形包含每个链接的收件人行为的可用数据。

  ![](assets/campaign_report_email_11.png)

### 用户活动 {#user-activities-email}

* **[!UICONTROL 用户活动]** 以图表的形式显示打开数和点击数的划分情况。

  ![](assets/campaign_report_email_12.png)

  +++了解有关电子邮件促销活动报告指标的更多信息。

   * **[!UICONTROL 点击次数]**：投放中链接的点击总数。

   * **[!UICONTROL 打开次数]**：此域中至少打开过一次消息的不同目标收件人的数量。

+++

## 短信渠道 {#sms-channel}

### 投放摘要 {#delivery-summary-sms}

* **[!UICONTROL 投放概述]** 提供关键绩效指标(KPI)，用于提供关于访客如何参与短信投放的详细信息。

  ![](assets/campaign_report_sms_1.png)

  +++了解有关短信营销活动报告指标的更多信息。

   * **[!UICONTROL 发送总数]**：投放准备期间处理的消息总数。

   * **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

   * **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

+++

* **[!UICONTROL 初始目标受众统计信息]** 表格显示与收件人相关的数据：

  ![](assets/campaign_report_sms_2.png)

  +++了解有关短信营销活动报告指标的更多信息。

   * **[!UICONTROL 初始受众]**：定向收件人总数。

   * **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

   * **[!UICONTROL 被规则拒绝]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

* **[!UICONTROL 执行统计信息]** 该表详细说明了您的交付是否成功：

  ![](assets/campaign_report_sms_3.png)

  +++了解有关短信营销活动报告指标的更多信息。

   * **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

   * **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

   * **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

   * **[!UICONTROL 新隔离]**：在失败的投放（用户未知、域无效）后隔离的地址总数，与要投放的消息数相关。

+++

* **[!UICONTROL 生成的点击流]** 该表显示了与收件人与投放的交互方式相关的数据：

  ![](assets/campaign_report_sms_4.png)

  +++了解有关短信营销活动报告指标的更多信息。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

   * **[!UICONTROL 点击次数]**：投放中链接的点击总数。

   * **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之间的比率。

+++

## 推送渠道 {#push-channel}

### 投放摘要 {#delivery-summary-push}

* **[!UICONTROL 投放概述]** 提供关键绩效指标(KPI)，用于提供关于访客如何参与推送通知投放的详细信息。

  +++了解有关推送营销活动报告量度的更多信息。

   * **[!UICONTROL 发送总数]**：投放准备期间处理的消息总数。

   * **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

   * **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

+++

* **[!UICONTROL 初始目标受众统计信息]** 表格显示与收件人相关的数据：

  +++了解有关推送营销活动报告量度的更多信息。

   * **[!UICONTROL 初始受众]**：定向收件人总数。

   * **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

   * **[!UICONTROL 被规则拒绝]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

* **[!UICONTROL 执行统计信息]** 该表详细说明了您的交付是否成功：

  +++了解有关推送营销活动报告量度的更多信息。

   * **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

   * **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

   * **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

   * **[!UICONTROL 新隔离]**：在失败的投放（用户未知、域无效）后隔离的地址总数，与要投放的消息数相关。

+++

* **[!UICONTROL 生成的点击流]** 该表显示了与收件人与投放的交互方式相关的数据：

  +++了解有关推送营销活动报告量度的更多信息。

   * **[!UICONTROL 不同点击次数]**：在投放中至少点击一次的不同收件人的总数。

   * **[!UICONTROL 点击次数]**：投放中链接的点击总数。

   * **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之间的比率。

+++
