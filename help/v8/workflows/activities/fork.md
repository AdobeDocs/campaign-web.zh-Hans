---
audience: end-user
title: 使用分支工作流活动
description: 了解如何使用分支工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---


# 分叉 {#fork}

此 **分支** 活动是 **流量控制** 活动。 利用此选项可创建叫客过渡以同时启动多个活动。

## 配置

按照以下步骤配置 **分支** 活动：

1. 添加 **分支** 活动添加到工作流。
1. 单击 **添加过渡** 以添加新的叫客过渡。 默认情况下，定义了两个过渡。
1. 为每个过渡添加标签。

## 示例

下面的示例，我们使用两个 **分支** 活动：

* 两个查询前一个，以同时执行它们。
* 在交叉点后一个，向目标群体同时发送电子邮件和短信。

![](../assets/workflow-fork-example.png)

