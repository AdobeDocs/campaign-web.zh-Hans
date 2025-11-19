---
audience: end-user
title: 推送渠道的营销活动报表
description: 了解推送渠道的活动报表
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 17%

---

# 推送渠道的营销活动报表 {#campaign-reports-push-channel}

每个营销活动报告都分为不同的小组件，其中详细说明了营销活动的成功和错误。 对于推送渠道，下文将详细介绍相关报表和量度。 在[此页面](campaign-reports.md)上了解如何访问您的营销活动报告。

## 投放摘要 {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="投放概述"
>abstract="**投放概述**&#x200B;报告提供详述访客如何与推送通知投放互动的关键绩效指标 (KPI)。"

**[!UICONTROL 投放概述]**&#x200B;报告提供了关键绩效指标(KPI)，这些指标提供有关访客如何参与推送通知投放的详细信息。 指标详见下文。

![投放概述报告中显示的投放摘要量度](assets/campaign-reporting-push-summary.png){zoomable="yes"}

+++了解有关推送营销活动报表量度的更多信息。

* **[!UICONTROL 要投放的邮件]**：投放准备期间处理的邮件总数。

* **[!UICONTROL 已投放]**：成功发送的邮件数与已发送的邮件总数相关。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息的总数之比。

* **[!UICONTROL 总点击次数]**：在投放中至少点击一次的不同收件人的总数。

+++

### 初始目标受众统计信息 {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="初始目标受众统计信息"
>abstract="**初始目标受众统计数据**&#x200B;表显示有关您的收件人的数据。"

**[!UICONTROL 初始目标受众统计信息]**&#x200B;表显示与收件人相关的数据。 指标详见下文。

![报表中显示的初始目标受众统计信息](assets/campaign-reporting-push-target.png){zoomable="yes"}

+++了解有关推送营销活动报表量度的更多信息。

* **[!UICONTROL 初始受众]**：目标收件人的总数。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* 列入阻止列表 **[!UICONTROL 被规则拒绝]**：应用规则时分析期间忽略的地址总数，例如地址缺失、隔离或。

+++

### 执行统计信息 {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="执行统计信息"
>abstract="**执行统计信息**&#x200B;表详述投放是否成功：要投放的消息数、成功数、错误数和新隔离数。"

**[!UICONTROL 执行统计信息]**&#x200B;表详细说明了您的交付是否成功。 指标详见下文。

![报告中显示的执行统计信息](assets/campaign-reporting-push-exec.png){zoomable="yes"}

+++了解有关推送营销活动报表量度的更多信息。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* **[!UICONTROL 成功]**：已成功处理的邮件数与要传递的邮件数相关。

* **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数相关。

* **[!UICONTROL 新隔离]**：在投放失败（例如无效注册、消息拒绝或有效负载错误）后隔离的地址总数，与要投放的消息数相关。

  推送通知错误类型列在[Adobe Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}中。

+++

### 生成的点击流 {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="生成的点击流"
>abstract="**生成的点击流**&#x200B;表显示有关接收者与投放如何互动的可用数据。"

**[!UICONTROL 生成的点击流]**&#x200B;表显示与收件人与投放交互方式相关的数据。 指标详见下文。

![报表中显示的已生成的点击流](assets/campaign-reporting-push-clicks.png){zoomable="yes"}

+++了解有关推送营销活动报表量度的更多信息。

* **[!UICONTROL 唯一点击次数]**：在投放中至少点击一次的不同收件人的总数。

* **[!UICONTROL 总点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 反应性]**：点击投放的目标收件人数量与打开投放的目标收件人的预计数量之比。

+++
