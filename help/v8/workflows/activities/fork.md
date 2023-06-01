---
audience: end-user
title: 使用分支工作流活动
description: 了解如何使用分支工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 5%

---


# 分叉 {#fork}

此 **分支** 利用活动，可创建叫客过渡以同时开始多个活动。

此 **分支** 利用活动，可在同一工作流中独立地执行多个不同的活动。

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

