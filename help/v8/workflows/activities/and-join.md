---
audience: end-user
title: 使用AND-join工作流活动
description: 了解如何使用“与”连接工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: bdf569913dfcf9bee549c6ae3252f5a92a5f34e8
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 3%

---


# AND-连接 {#join}

此 **And — 连接** 活动是 **流量控制** 活动。 它允许您同步工作流的多个执行分支。

一旦激活所有集客过渡，换言之，一旦完成所有先行工作，此活动就会触发其叫客过渡。 这允许您在继续执行工作流之前确保某些活动已完成。

## 配置

按照以下步骤配置 **AND — 连接** 活动：

1. 添加多个活动（如渠道活动）以形成至少两个不同的执行分支。
1. 添加 **AND — 连接** 活动到任何分支。
1. 在 **合并选项** 部分，检查您之前希望加入的所有活动。
1. 在 **主集** 下拉列表中，选择要保留的集客过渡群体。 叫客过渡只能包含其中一个集客过渡群体。

## 示例

下方的示例显示了两个工作流分支，其中包含电子邮件和短信投放。 启用两个集客过渡后，将触发AND-join。 然后，推送通知将仅在两个投放均完成后发送。

![](../assets/workflow-andjoin-example.png)