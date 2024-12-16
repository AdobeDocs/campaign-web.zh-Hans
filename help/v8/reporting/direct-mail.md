---
audience: end-user
title: 直邮报表
description: 了解如何访问和使用直邮报表
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 23%

---

# 直邮投放报告 {#direct-mail-report}

**直邮投放报告**&#x200B;提供了特定于您的直邮投放的综合见解和数据。 它提供有关个人投放的绩效、效力和结果的详细信息，使您能够全面了解情况。

## 投放摘要 {#delivery-summary-direct-mail}

### 投放概述 {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="投放概述"
>abstract=" **投放概述**&#x200B;提供了关键绩效指标 (KPI)，可深入了解访客与每次直邮投放的互动情况。这些量度概述如下。"

**[!UICONTROL 投放概述]**&#x200B;提供了有关访客如何与每个直邮投放进行交互的详细分析，展示了关键绩效指标(KPI)。  这些量度概述如下。

![](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++了解有关投放概述量度的更多信息。

* **[!UICONTROL 要投放的邮件]**：投放准备期间处理的邮件总数。

* **[!UICONTROL 目标]**：符合直邮消息目标用户档案资格的用户档案数。

* **[!UICONTROL 要排除]**：从目标用户档案中排除且不会接收直邮邮件的用户档案数。
+++

### 初始目标群体 {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="初始目标群体"
>abstract="**初始目标群体**&#x200B;图表按投放准备的结果显示与接收者和消息相关的数据。"

**[!UICONTROL 初始目标群体]**&#x200B;图形显示与收件人相关的数据。 量度在投放准备期间计算并显示：初始受众、要发送的消息数、排除的收件人数。

![](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

将鼠标悬停在图形的一部分上以显示确切数字。

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++了解有关直邮投放报告指标的更多信息。

* **[!UICONTROL 初始受众]**：目标收件人的总数。

* **[!UICONTROL 要投放的邮件]**：投放准备后要投放的邮件总数。

* **[!UICONTROL 排除项]**：从目标群体中排除的收件人总数。
+++

### 投放统计信息 {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="投放统计信息"
>abstract="**投放统计信息**&#x200B;图表详述直邮投放是否成功和发生的错误。"

**[!UICONTROL 投放统计数据]**&#x200B;图提供了投放性能的全面概述，提供了用于衡量成功和效果的详细量度。

![](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++了解有关直邮营销活动报告指标的更多信息。

* **[!UICONTROL 已发送邮件]**：准备传递后要传递的邮件总数。

* **[!UICONTROL 成功]**：已成功处理的邮件数与要传递的邮件数相关。

* **[!UICONTROL 错误]**：投放和自动回弹处理期间累计的错误总数与要投放的消息数相关。

* **[!UICONTROL 新隔离]**：在投放失败（用户未知，域无效）后隔离的地址总数与要投放的消息数相关。

+++

### 排除的原因 {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="投放排除原因"
>abstract=" **排除原因**&#x200B;图表显示了准备投放期间遭到拒绝的邮件的分布情况，并按每项规则进行分类。"

**[!UICONTROL 排除原因]**&#x200B;图形提供了在投放准备过程中消息被拒绝的原因的详细细目。 此划分按各种规则进行整理，可全面了解导致报文排除的因素。 有关排除规则的详情，请参见[Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}。

![](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++了解有关排除量度原因的更多信息。

* 隔离中的&#x200B;**[!UICONTROL 地址]**：将地址置于隔离中时生成错误类型。

* **[!UICONTROL 未指定地址]**：发送投放时生成错误类型以指示地址不存在。

* **[!UICONTROL 质量地址错误]**：当邮政地址质量等级太低时生成错误类型。

* 列入阻止列表 列入阻止列表 **[!UICONTROL 地址]**：执行传递时收件者产生错误类型。

* **[!UICONTROL 双精度型]**：由于键值不唯一而排除收件人时生成的错误类型。

* **[!UICONTROL 控制组]**：收件人的地址是控制组的一部分。

* **[!UICONTROL 目标大小受限]**：已达到收件人的最大投放大小。

+++

### 排除项 {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="排除项"
>abstract=" **[!UICONTROL 排除项]**&#x200B;表格按规则显示在传送投放过程中遭到拒绝的邮件的细分。"

**[!UICONTROL 排除项]**&#x200B;表提供了在投放准备阶段被拒绝的消息按特定规则分类的深入细分。 通过这种全面的细分，可清楚地了解将这些消息排除在投放过程之外的原因。

![](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

可用的量度与上面描述的[排除原因](#direct-mail-delivery-exclusions)的量度相同。
