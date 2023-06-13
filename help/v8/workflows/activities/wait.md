---
audience: end-user
title: 使用等待工作流活动
description: 了解如何使用等待工作流活动
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 29%

---


# 等待 {#wait}

此 **等待** 活动是 **流量控制** 活动。 它用于在执行的两个活动之间传递一定的时间。 例如，在执行电子邮件投放活动后，等待几天，再分析这期间产生的打开次数和点击次数，然后再执行所有后续操作（提醒电子邮件、创建受众等）。

## 配置

按照以下步骤配置 **等待** 活动：

1. 添加 **等待** 活动添加到工作流中。

1. 指定 **持续时间** 集客过渡和叫客过渡之间的等待时间。

1. 选择时间单位 **期间** 字段：秒、分钟、小时。

## 示例

以下示例说明了 **等待** 活动。 发送某个活动的电子邮件邀请。在发送后24小时，会向同一群体发送短信投放。

![](../assets/workflow-wait-example.png)
