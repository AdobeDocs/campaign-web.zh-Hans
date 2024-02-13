---
audience: end-user
title: 推送渠道的营销活动报表
description: 了解推送渠道的活动报表
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 18%

---

# 推送渠道的营销活动报表 {#campaign-reports-push-channel}

每个营销活动报告都分为不同的小组件，其中详细说明了营销活动的成功和错误。 对于推送渠道，下文将详细介绍相关报表和量度。 了解如何在中访问您的营销活动报告 [此页面](campaign-reports.md).

## 投放摘要 {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="投放概述"
>abstract="**投放概述**&#x200B;报告提供详述访客如何与推送通知投放互动的关键绩效指标 (KPI)。"

此 **[!UICONTROL 投放概述]** 报告提供关键绩效指标(KPI)，这些指标提供关于访客如何参与推送通知投放的详细信息。 指标详见下文。

![](assets/campaign-reporting-push-summary.png){zoomable=&quot;yes&quot;}


+++了解有关推送营销活动报告量度的更多信息。

* **[!UICONTROL 发送总数]**：投放准备期间处理的消息总数。

* **[!UICONTROL 已投放]**：成功发送的消息数，与已发送消息的总数相关。

* **[!UICONTROL 错误]**：投放和自动返回处理期间累计的错误总数与已发送消息总数相关。

* **[!UICONTROL 总点击次数]**：在投放中至少点击一次的不同收件人的总数。

+++

### 初始目标受众统计信息 {#delivery-summary-push-initial-target}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="初始目标受众统计信息"
>abstract="**初始目标受众统计信息**&#x200B;表显示有关您的收件人的数据"

此 **[!UICONTROL 初始目标受众统计信息]** 表格会显示与收件人相关的数据。 指标详见下文。

![](assets/campaign-reporting-push-target.png){zoomable=&quot;yes&quot;}


+++了解有关推送营销活动报告量度的更多信息。

* **[!UICONTROL 初始受众]**：定向收件人总数。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 被规则拒绝]**：应用规则时分析期间忽略的地址总数：地址缺失、隔离、阻止列表等。

+++

### 执行统计信息 {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="执行统计信息"
>abstract="**执行统计信息**&#x200B;表详述投放是否成功：要投放的消息数、成功数、错误数和新隔离数。"

此 **[!UICONTROL 执行统计信息]** 表详细说明了您的交付是否成功。 指标详见下文。

![](assets/campaign-reporting-push-exec.png){zoomable=&quot;yes&quot;}


+++了解有关推送营销活动报告量度的更多信息。

* **[!UICONTROL 要投放的消息]**：投放准备后要投放的消息总数。

* **[!UICONTROL 成功]**：成功处理的消息数与要投放的消息数相关。

* **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数，与要投放的消息数量相关。

* **[!UICONTROL 新隔离]**：投放失败后隔离的地址总数（注册无效、消息拒绝、有效负载错误等） 与要投放的消息数相关。

  推送通知错误类型列在 [Adobe Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### 生成的点击流 {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="生成的点击流"
>abstract="**生成的点击流**&#x200B;表显示有关接收者与投放如何互动的可用数据。"

此 **[!UICONTROL 生成的点击流]** 该表显示了与收件人与投放的交互方式相关的数据。 指标详见下文。

![](assets/campaign-reporting-push-clicks.png){zoomable=&quot;yes&quot;}

+++了解有关推送营销活动报告量度的更多信息。

* **[!UICONTROL 独特点击]**：在投放中至少点击一次的不同收件人的总数。

* **[!UICONTROL 总点击次数]**：投放中链接的点击总数。

* **[!UICONTROL 反应性]**：已点击投放的目标收件人数量与已打开投放的目标收件人的估计数量之间的比率。

+++
