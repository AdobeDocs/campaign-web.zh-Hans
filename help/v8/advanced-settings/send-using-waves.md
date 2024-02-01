---
audience: end-user
title: 使用批次发送
description: 详细了解Campaign Web中的投放设置
badge: label="有限发布版"
source-git-commit: 1d3e2ccbf4db5eb23531351572a4400754982e2d
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 9%

---


# 按波次发送 {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="波次定义"
>abstract="定义波次以将投放分为多个批次，而非同时发送大量消息。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="波次的大小"
>abstract="波次的大小为必填。在大小字段中输入数值（消息数）或百分比 (0-100%)。"

要平衡负荷，您可以将投放分为多个批。 配置批次数量及其相对于整个投放的比例。

>[!NOTE]
>
>您只能定义两个连续波形之间的大小和延迟。 无法配置每个波次的收件人选择标准。

1. 打开 [投放设置](delivery-settings.md#retries) 然后转到 **[!UICONTROL 投放]** 选项卡。
1. 选择 **[!UICONTROL 使用多个批次发送]** 选项，然后单击 **[!UICONTROL 定义批次……]** 链接。

1. 要配置批次，您可以：

   * **[!UICONTROL 计划多个相同大小的批次]**. 例如，如果您输入 **[!UICONTROL 30%]** 在相应的字段中，每个波次将代表投放中所包含报文的30%，但最后一条代表10%的报文。

     在 **[!UICONTROL 间隔]** 部分，指定两个连续批次开始之间的延迟。 例如，如果您输入 **[!UICONTROL 2d]**，第一波立即开始，第二波在两天内开始，第三波在四天内开始，以此类推。

   * **[!UICONTROL 根据日程表计划批次]**.

     在 **[!UICONTROL 开始]** 列，指定两个连续批次开始之间的延迟。 在 **[!UICONTROL 大小]** 列中，输入固定数字或百分比。

     在下面的示例中，第一波表示投放中包含的消息总数的25%，将立即启动。 接下来的两个批次将完成投放，并设置为以六小时间隔开始。

     特定的类型控制规则， **[!UICONTROL 波动计划检查]**，确保最后一个波次的计划时间早于投放有效期限。 促销活动类型及其规则配置于 **[!UICONTROL 类型]** 选项卡进行发送。 在中了解有关控制规则的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html)

     >[!IMPORTANT]
     >
     >确保最后批次不超过投放截止日期，投放截止日期在中定义 **[!UICONTROL 有效期]** 选项卡。 否则，某些消息可能不会发送。 [了解详情](delivery-settings.md#validity)
     >
     >在配置最后批次时，还必须留出足够的时间进行重试。 [了解详情](delivery-settings.md#retries)

1. 要监控您的发送，请转到 [投放日志](../monitor/delivery-logs.md).

您可以看到已在已处理批次中发送的投放(**[!UICONTROL 已发送]** 状态)和要在剩余批次中发送的投放(**[!UICONTROL 待处理]** 状态)。

以下两个示例是使用多个批次的最常见用例。

* **启动过程中**

  使用新平台发送电子邮件时，Internet服务提供商(ISP)会怀疑无法识别的IP地址。 如果突然发送大量电子邮件，ISP通常会将其标记为垃圾邮件。

  要避免被标记为垃圾邮件，您可以逐步增加使用批次发送的数量。 这应该可以确保启动阶段的顺利发展，并帮助您降低地址无效的总比率。

  要执行此操作，请使用 **[!UICONTROL 根据日程表计划批次]** 选项。 例如，将第一个波次设置为10%，将第二个波次设置为15%，以此类推。

* **涉及呼叫中心的营销活动**

  在管理电话忠诚度促销活动时，贵组织处理致电订阅者的能力有限。

  使用批次，您可以将每天的消息数量限制为20，这是呼叫中心的每日处理能力。

  要执行此操作，请选择 **[!UICONTROL 计划多个相同大小的批次]** 选项。 输入 **[!UICONTROL 20]** 因为波浪的大小和 **[!UICONTROL 1d]** 在 **[!UICONTROL 期间]** 字段。