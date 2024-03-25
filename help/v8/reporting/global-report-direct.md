---
audience: end-user
title: 直邮渠道的全局报告
description: 详细了解直邮渠道的全局报告
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 33%

---

# 直邮渠道的全局报告 {#global-report-direct}

直邮全局报告可在渠道级别为用户提供流量和参与量度的全面概述。

导航至 **[!UICONTROL 报表]** 中的菜单 **[!UICONTROL 报表]** 部分。 您可以根据报表日期、文件夹或规则过滤数据。 [了解详情](global-reports.md)

## 投放摘要 {#delivery-summary-direct}

### 投放概述 {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="投放概述"
>abstract=" **投放概览**&#x200B;提供了关键绩效指标 (KPI)，可深入了解访客与每次直邮投放的互动情况。这些量度概述如下。"

 **[!UICONTROL 投放概览]**&#x200B;提供了关键绩效指标 (KPI)，可深入了解访客与每次直邮投放的互动情况。这些量度概述如下。

![](assets/global_report_direct_mail_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备期间处理的消息总数。

* **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

* **[!UICONTROL 取消订阅]**：点击取消订阅的收件人数量。
+++

### 目标受众 {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="目标受众"
>abstract="收件人数据和消息信息会在&#x200B;**目标受众**&#x200B;图表中显示，其反映了投放准备分析。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="目标受众"
>abstract="**目标受众**&#x200B;表格根据投放准备过程的结果提供了收件人和相应消息的细分。"

表和图表 **[!UICONTROL 目标受众]** 显示与收件人相关的数据，并提供以下详细量度。

![](assets/global_report_direct_mail_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++了解有关目标受众量度的更多信息。

* **[!UICONTROL 目标受众]**：定向收件人总数。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 排除项]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

### 投放统计信息 {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="投放统计信息"
>abstract=" **投放统计信息**&#x200B;图表有助于您深入了解直邮投放的有效性，其中包括成功的投放和遇到的任何错误。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="投放统计信息"
>abstract="**投放统计信息**&#x200B;表格详述直邮投放是否成功和发生的错误。"

此 **[!UICONTROL 投放统计信息]** 图表提供了每次直邮投放成功的划分以及下面列出的详细量度。

+++了解有关投放统计量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

* **[!UICONTROL 错误/退回]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

* **[!UICONTROL 新隔离]**：在失败的投放（用户未知、域无效）后隔离的地址总数，与要投放的消息数相关。

+++

### 排除的原因 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="排除项"
>abstract=" **排除原因**&#x200B;表格按规则显示在传送投放过程中遭到拒绝的邮件的细分。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="投放排除原因"
>abstract=" **排除原因**&#x200B;图表显示了准备投放期间遭到拒绝的邮件的分布情况，并按每项规则进行分类。"

![](assets/global_report_direct_mail_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

排除项图表和表说明了阻止从目标用户档案排除的用户用户档案接收消息的原因。

+++了解有关排除量度原因的更多信息。

* **[!UICONTROL 隔离地址]**：将地址置于隔离区时生成的错误类型。

* **[!UICONTROL 未指定地址]**：发送投放时生成的错误类型，指示地址不存在。

* **[!UICONTROL 质量不佳的地址]**：当邮政地址质量等级太低时生成的错误类型。

* **[!UICONTROL 列入阻止列表的地址]**：执行投放时列入阻止列表收件人时生成的错误类型。

* **[!UICONTROL 多次]**：由于收件人键值不唯一而被排除时生成的错误类型。

* **[!UICONTROL 对照组]**：收件人的地址是控制组的一部分。

* **[!UICONTROL 目标大小受限]**：已到达收件人的最大投放大小。

+++
