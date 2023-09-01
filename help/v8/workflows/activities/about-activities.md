---
audience: end-user
title: 使用工作流活动
description: 了解如何使用工作流活动
badge: label="Beta"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 100%

---


# 关于工作流活动 {#workflow-activities}

工作流活动分为三类。根据具体情况，可用的活动可能会有所不同。

以下各章节详细介绍了所有活动：

* [定位活动](#targeting)
* [渠道活动](#channel)
* [流量控制活动](#flow-control)

![](../assets/workflow-activities.png)

## 定位活动 {#targeting}

这些活动专门针对定位、操纵和丰富人口数据。利用这些活动，您可以通过定义受众并使用交集、并集或差集操作来拆分或合并这些受众，从而构建一个或多个目标。

* [生成受众](build-audience.md)活动允许您定义目标人群。您可以选择现有受众或使用规则生成器来定义您自己的查询。
* [合并](combine.md)活动允许对集客群体进行分段。您可以使用并集、交集或差集。
* [扩充](enrichment.md)活动允许您定义要在工作流中处理的其他数据。通过此活动，您可以应用集客过渡并配置活动以使用附加数据填写输出过渡。
* [拆分](split.md)活动允许您将传入群体划分为几个子集。

## 渠道活动 {#channel}

Adobe Campaign Web 允许您跨多个渠道（例如电子邮件、短信或推送消息）自动化和执行营销活动。您可以将渠道活动组合到画布中，以创建可根据客户行为触发操作的跨渠道工作流。

以下&#x200B;**渠道**&#x200B;活动可用：

* 电子邮件
* 推送
* 短信

请参阅此[章节](enrichment.md)。

## 流量控制活动 {#flow-control}

以下活动专用于组织和执行工作流。这些活动的主要任务是协调其他活动：

* 利用 [And-连接](and-join.md)活动，可同步工作流的多个执行分支。
* 您可以使用&#x200B;**结束**&#x200B;活动以图形方式标记工作流的终点。此活动没有功能影响，因此是可选的。
* 利用[分叉](fork.md)活动，可创建叫客过渡以同时开始多个活动。
* [等待](wait.md)活动可暂停执行部分工作流。

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

