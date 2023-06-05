---
audience: end-user
title: 使用短信工作流活动
description: 了解如何使用短信工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: c0e5902d3ee504aa5aa4e55f18416facfe4020b1
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 5%

---


# 短信 {#sms}

此 **短信** 活动提供了在工作流中发送短信消息的功能。 它允许向在同一工作流中确定的特定目标自动发送短信。

要定义短信的收件人，您可以使用构建受众活动，在工作流中的短信投放活动之前设置这些收件人。 了解详情。

1. 创建和配置新工作流后，添加构建受众活动以选择现有受众，或使用规则生成器定义您自己的查询。

1. 在工作流中添加短信渠道活动。

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. 选择您的活动。 从投放菜单中，选择要用于此投放的模板。 了解有关模板的更多信息

1. 单击创建投放以配置短信投放。 有关短信投放的更多信息，请参阅此页面。

1. 准备好发送投放后，导航回工作流，然后单击“开始”以启动工作流。

1. 默认情况下，启动投放工作流会触发消息准备阶段，而不会立即发送消息。

   单击短信活动高级菜单中的审核并发送以确认发送。

1. 在短信投放仪表板中，单击发送。
