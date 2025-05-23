---
audience: end-user
title: 电子邮件投放报告
description: 了解如何访问和使用电子邮件投放报告
exl-id: 2a0bd3e9-5d75-47c8-bd6a-b3e0b1ce0a01
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '2448'
ht-degree: 37%

---

# 电子邮件投放报告 {#email-report}

**电子邮件投放报告**&#x200B;提供了特定于电子邮件渠道的综合分析和数据。 它提供有关个人投放的绩效、效力和结果的详细信息，使您能够全面了解情况。

## 投放摘要 {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="报告发送"
>abstract="利用报告中的&#x200B;**发送**&#x200B;选项卡，可深入了解访客与投放之间的交互及访客可能遇到的任何潜在错误。"

### 初始目标群体 {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="初始目标群体"
>abstract="**初始目标群体**&#x200B;图表按投放准备的结果显示与接收者和消息相关的数据。"

**[!UICONTROL 初始目标群体]**&#x200B;图形显示与收件人相关的数据。 量度在投放准备期间计算并显示：初始受众、要发送的消息数、排除的收件人数。

![显示数据的图形屏幕截图](assets/reporting_email_1.png){zoomable="yes"}

将鼠标悬停在图形的一部分上以显示确切数字。

![将鼠标悬停在某个部分上的图形屏幕截图可显示确切的数字](assets/reporting_email_1.1.png){zoomable="yes"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 初始受众]**：目标收件人的总数。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* **[!UICONTROL 排除项]**：从目标群体中排除的收件人总数。
+++

### 投放统计信息 {#email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="投放统计信息"
>abstract="**投放统计信息**&#x200B;图表详述投放是否成功和发生的错误。"

**[!UICONTROL 投放统计数据]**&#x200B;图形详细说明了您的投放是否成功。 指标详见下文。

![显示投放统计信息详细信息的图形屏幕截图](assets/reporting_email_2.png){zoomable="yes"}

+++了解有关电子邮件促销活动报告指标的更多信息。

* **[!UICONTROL 已发送邮件]**：准备传递后要传递的邮件总数。

* **[!UICONTROL 成功]**：已成功处理的邮件数与要传递的邮件数相关。

* **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数与要投放的消息数相关。

* **[!UICONTROL 新隔离]**：在投放失败（用户未知，域无效）后隔离的地址总数与要投放的消息数相关。

+++

### 排除的原因  {#email-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="投放排除原因"
>abstract="**排除的原因**&#x200B;图表显示投放准备期间拒绝的消息按规则细分的情况。"

**[!UICONTROL 排除原因]**&#x200B;图形和表显示在投放准备期间拒绝的消息按规则细分。 有关排除规则的详情，请参见[Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=zh-Hans#email-error-types){_blank}。

![排除图表和表的原因屏幕截图](assets/reporting_email_3.png){zoomable="yes"}{align="center" zoomable="yes"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 用户未知]**：在投放期间生成错误类型以指示电子邮件地址无效。

* **[!UICONTROL 无效域]**：发送投放时生成的错误类型，指示电子邮件地址的域错误或不存在。

* **[!UICONTROL 邮箱已满]**：在五次传递尝试后生成的错误类型表示收件人的收件箱包含太多邮件。

* **[!UICONTROL 帐户已禁用]**：发送投放时生成错误类型以指示地址不再存在。

* **[!UICONTROL 已拒绝]**：当地址被IAP（Internet访问提供程序）拒绝时生成的错误类型，例如在应用安全规则（反垃圾邮件软件）之后。

* **[!UICONTROL 不可访问]**：消息分发字符串中出现的错误类型：SMTP中继上的事件、域名暂时不可访问等

* **[!UICONTROL 未连接]**：错误类型表示收件人的手机在发送时关闭或与网络断开。

+++

## 投放吞吐量 {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="投放吞吐量"
>abstract="**投放吞吐量**&#x200B;报告提供有关指定时间范围内整个 Platform 的投放吞吐量的详细信息。"

此报表可呈现有关指定时间范围内整个平台的投放吞吐量的详细信息。 用于衡量消息投放速度的主要量度是每小时发送的消息数。

![投放吞吐量的屏幕截图](assets/reporting_email_3.1.png){zoomable="yes"}{align="center" zoomable="yes"}


## 广播统计信息 {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="广播统计信息"
>abstract="**广播统计信息**&#x200B;报告包含每个域可能遇到的错误的可用数据。"

**[!UICONTROL 广播统计信息]**&#x200B;表包含每个域可能遇到的错误的可用数据。 指标详见下文。

![广播统计信息的屏幕截图](assets/reporting_email_4.png){zoomable="yes"}{align="center" zoomable="yes"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 已处理的电子邮件]**：投放服务器处理的邮件总数。

* **[!UICONTROL 已投放]**：已成功处理的邮件数与已处理的邮件总数之间的百分比。

* **[!UICONTROL 硬退回]**：“硬”退回、永久错误（如电子邮件地址错误）数量与已处理邮件总数的百分比。

* **[!UICONTROL 软退回]**：“软”退回、临时错误（如收件箱已满）数量与已处理邮件总数的百分比

* **[!UICONTROL 打开次数]**：与成功处理的邮件数相比，至少打开过一次邮件的目标收件人数的百分比。

* **[!UICONTROL 点击次数]**：与成功处理的邮件数相比，至少点击一次投放的用户数的百分比。

* **[!UICONTROL 取消订阅]**：与成功处理的邮件数相比，取消订阅链接的点击数百分比。
+++

## 投放失败 {#non-deliverables-email}

### 按类型细分错误 {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="按类型细分错误"
>abstract="**按类型细分错误**&#x200B;图形包含遇到的每种错误类型的可用数据：用户未知、邮箱已满、域无效等。"

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type_table"
>title="按类型细分错误"
>abstract="**每种类型的错误细分**&#x200B;表提供了每种错误类型发生次数的全面细分。"

每个类型&#x200B;**表和图形的**&#x200B;错误划分包含错误类型的可用数据。 指标详见下文。

此报告中显示的错误会触发隔离过程。 有关隔离管理的更多信息，请参阅[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=zh-Hans){target="_blank"}。

![每个类型的错误划分屏幕截图](assets/campaign_report_email_6.png){zoomable="yes"}{align="left" zoomable="yes"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 用户未知]**：在投放期间生成错误类型以指示电子邮件地址无效。

* **[!UICONTROL 无效域]**：发送投放时生成的错误类型，指示电子邮件地址的域错误或不存在。

* **[!UICONTROL 邮箱已满]**：在五次传递尝试后生成的错误类型表示收件人的收件箱包含太多邮件。

* **[!UICONTROL 帐户已禁用]**：发送投放时生成错误类型以指示地址不再存在。

* **[!UICONTROL 已拒绝]**：当地址被IAP（Internet访问提供程序）拒绝时生成的错误类型，例如在应用安全规则（反垃圾邮件软件）之后。

* **[!UICONTROL 不可访问]**：消息分发字符串中出现的错误类型：SMTP中继上的事件、域名暂时不可访问等

* **[!UICONTROL 未连接]**：错误类型表示收件人的手机在发送时关闭或与网络断开。

+++

### 按域细分错误 {#email-delivery-breakdown-domain}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="按域细分错误"
>abstract="**按域细分错误**&#x200B;图形显示了遇到的每种错误类型的可用数据（按域细分）。"

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain_table"
>title="按域细分错误"
>abstract="**每个域的错误细分**&#x200B;表根据所使用的域提供了每个错误发生次数的全面细分。"

每个域&#x200B;**表和图形的**&#x200B;错误划分显示每个域可能遇到的错误的可用数据。

![每个域的错误划分屏幕截图](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

单击每个域名称旁边的图标以查看详细信息。

![每个域的错误划分屏幕截图以及每个域的详细信息](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

可用的量度与上面描述的[按类型](#email-delivery-breakdown-type)划分的错误量度相同。

## 跟踪指标 {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="报告跟踪"
>abstract="报告中的&#x200B;**跟踪**&#x200B;选项卡提供宝贵的数据（包括每个链接的接收者行为、打开和点击的细分）以及有关投放过程中最常点击的 URL 的详细信息。"


### 投放统计信息  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" 投放统计信息"
>abstract="**投放统计信息**&#x200B;报告提供关键绩效指标 (KPI)，这些指标详述对发送电子邮件可用的数据：是否成功、打开次数、点击次数等。"


**[!UICONTROL 投放统计信息]**&#x200B;报告提供了关键性能指标(KPI)，用于提供关于已发送电子邮件可用数据的详细信息。 指标详见下文。

![投放统计信息的屏幕截图](assets/reporting_email_5.png){zoomable="yes"}{align="center"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 成功]**：已成功处理的邮件数与要传递的邮件数相关。

* **[!UICONTROL 不同打开次数]**：至少打开过一次邮件的目标收件人总数。

* **[!UICONTROL 打开次数]**：此域中至少打开过一次邮件的不同目标收件人的数量。

* **[!UICONTROL 点击选择退出链接]**：点击取消订阅链接的次数。

* **[!UICONTROL 镜像链接的点击次数]**：镜像页面链接的点击次数。

* **[!UICONTROL 转发数量估计]**：目标收件人转发的电子邮件数量估计。
+++

### 打开和点进率 {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="打开和点进率"
>abstract="**打开和点进率**&#x200B;表显示有关接收者与投放互动的数据。"



**[!UICONTROL 打开和点进率]**&#x200B;表显示与收件人相关的数据。 指标详见下文。

![打开和点进率表的屏幕截图](assets/reporting_email_6.png){zoomable="yes"}{align="center"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 已发送]**：已发送的邮件总数。

* **[!UICONTROL 投诉]**：此域被收件人报告为不受欢迎的邮件数。

* **[!UICONTROL 打开次数]**：此域中至少打开过一次邮件的不同目标收件人的数量。

* **[!UICONTROL 点击次数]**：在同一个投放中至少点击过一次的不同目标收件人的数量。

* **[!UICONTROL 原始反应性]**：与至少打开一次投放的收件人数量相比，至少点击一次投放的收件人数量的百分比。
+++

## URL 和点击流 {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL 和点击流"
>abstract="**URL 和点击流**&#x200B;报告提供详述投放期间点击次数最多的 URL 的关键绩效指标 (KPI)。"


**[!UICONTROL URL 和点击流]**&#x200B;报告提供详述投放期间点击次数最多的 URL 的关键绩效指标 (KPI)。

![URL和点击流报告的屏幕截图](assets/reporting_email_7.png){zoomable="yes"}{align="center"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之比。

* **[!UICONTROL 非重复点击]**：在投放中至少点击一次的非重复收件人总数。

* **[!UICONTROL 点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 平台平均值]**：计算每个速率（反应性、非重复点击和累计点击）下显示的平均速率，用于计算过去六个月发送的投放数量。 只考虑具有相同类型和相同渠道的投放。 排除验证。

+++

### 访问量排名前 10 的链接 {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="访问量排名前 10 的链接"
>abstract="**访问量排名前 10 的链接**&#x200B;图和表包含每个链接的收件人行为的可用数据。"


**[!UICONTROL 访问量排名前 10 的链接]**&#x200B;图和表包含每个链接的收件人行为的可用数据。

![访问次数前10位的链接图屏幕截图](assets/reporting_email_8.png){zoomable="yes"}{align="center"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 百分比]**：与投放交互的用户百分比。

+++

### 点击次数随时间变化的细分 {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="点击次数随时间变化的细分"
>abstract="**点击次数随时间变化的细分**&#x200B;图表显示每个链接的接收者行为的可用数据。"


**[!UICONTROL 随时间变化的点击细分]**&#x200B;图形包含每个链接的收件人行为的可用数据。

![随时间变化的点击细分屏幕截图](assets/reporting_email_9.png){zoomable="yes"}{align="center"}

## 用户活动 {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="用户活动"
>abstract="**用户活动**&#x200B;图以图表形式显示打开次数和点击次数的细分。可选择时段以锁定数据：过去一天、过去一小时或过去 30 分钟。"

**[!UICONTROL 用户活动]**&#x200B;报告以图表形式显示打开数和点击数的细分。 可选择时段以锁定数据：过去一天、过去一小时或过去 30 分钟。

![用户活动报告的屏幕截图](assets/reporting_email_10.png){zoomable="yes"}{align="center"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 打开次数]**：此域中至少打开过一次邮件的不同目标收件人的数量。

+++

## 跟踪统计数据 {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="跟踪统计数据"
>abstract="**跟踪统计数据**&#x200B;图提供有关打开次数和点击次数的统计信息。可选择特定的时间范围以定位数据。"

**[!UICONTROL 跟踪统计数据]**&#x200B;图提供有关打开次数和点击次数的统计信息。可选择特定的时间范围以定位数据。

![跟踪统计信息图的屏幕截图](assets/reporting_email_11.png){zoomable="yes"}{align="center"}

+++了解有关电子邮件投放报告指标的更多信息。

* **[!UICONTROL 点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 打开次数]**：此域中至少打开过一次邮件的不同目标收件人的数量。

+++

## 打开的细分 {#breakdown-opens}

### 按设备类型细分的打开次数 {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="按设备细分"
>abstract="**按设备细分**&#x200B;报告显示相关时段的按设备类型细分的打开次数。为每个类别使用了两个图表。第一个图表显示有关计算机和移动设备上的打开的统计数据。第二个图表显示每种设备类型的确切数量和百分比。"

“**按设备细分**”报表显示在此期间按设备打开的细分：个人计算机、Android设备、Apple设备或其他。

为每个类别使用了两个图表。第一个图表显示有关计算机和移动设备上的打开的统计数据。第二个图表显示每种设备类型的确切数量和百分比。

![按设备划分的屏幕截图](assets/reporting_email_13.png){zoomable="yes"}{align="center"}


### 按操作系统类型细分的打开次数 {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="按操作系统细分"
>abstract="**按操作系统细分**&#x200B;报告显示相关时段的按操作系统细分的打开次数。第一个图表显示关于在计算机和移动设备上的打开次数的统计信息。第二个图表显示每种操作系统的确切数量和百分比。"

“**按操作系统细分**”报表显示期间按操作系统打开的细分：Windows系统、Android系统、iOS系统或其他。

为每个类别使用了两个图表。第一个显示有关计算机和移动操作系统上打开的统计信息。 第二个显示每个操作系统的确切数量和百分比。

![按操作系统划分报表的屏幕截图](assets/reporting_email_13.1.png){zoomable="yes"}{align="center"}

### 按浏览器类型细分的打开次数 {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="按浏览器细分"
>abstract="**按浏览器细分**&#x200B;显示相关时段的按浏览器细分的打开次数。第一个图表显示关于在计算机和移动设备上的打开次数的统计信息。第二个图表显示每种浏览器的确切数量和百分比。"

**按浏览器细分**&#x200B;报表显示按浏览器打开的细分：Chrome、Safari、Internet Explorer等。

为每个类别使用了两个图表。第一个显示有关计算机和移动操作系统上打开的统计信息。 第二个图表显示每种浏览器的确切数量和百分比。

![按浏览器报告的打开划分屏幕截图](assets/reporting_email_13.2.png){zoomable="yes"}{align="center"}


## 热门点击 {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="热门点击报告"
>abstract="**热门点击**&#x200B;报告显示电子邮件内容（HTML 和/或文本）以及每个链接的点击百分比。个性化块、退订链接、镜像页面链接和产品建议链接计入总累计点击次数，但不显示在报告中。"

此报告显示邮件内容（HTML 和/或文本）以及每个链接的点击百分比。个性化块、退订链接、镜像页面链接和产品建议链接计入总累计点击次数，但不显示在报告中。

![热门点击报告的屏幕截图](assets/reporting11.png){zoomable="yes"}