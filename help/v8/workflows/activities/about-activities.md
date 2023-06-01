---
audience: end-user
title: 使用工作流活动
description: 了解如何工作流活动
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c842829915784654b7130563d36dea188e84ff3d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 关于工作流活动 {#workflow-activities}

工作流活动分为三个类别。 根据上下文的不同，可用的活动可能会有所不同。

以下各节详细介绍了所有活动：

* [定位活动](#targeting)
* [渠道活动](#channel)
* [流量控制活动](#flow-control)

![](../assets/wokflow-activities.png)

## 定位活动 {#targeting}

这些活动专门用于定位、操纵和丰富人口数据。 通过定义受众，并使用交集、并集或排除操作拆分或组合这些受众，可让您构建一个或多个目标。

* 此 [构建受众](build-audience.md) 利用活动，可定义目标群体。 您可以选择现有受众，也可以使用规则生成器定义您自己的查询。
* 此 [合并](combine.md) 活动允许对集客群体执行分段。 您可以使用并集、交集或排除项。
* 此 [扩充](enrichment.md) 活动允许您定义要在工作流中处理的附加数据。 通过此活动，您可以利用集客过渡并配置活动以使用附加数据完成输出过渡。

## 渠道活动 {#channel}

通过Adobe Campaign Web，您可以跨多个渠道（如电子邮件、短信或推送）自动执行营销活动。 借助Adobe Campaign工作流，您可以将渠道活动合并到画布中，以创建可根据客户行为触发操作的跨渠道工作流。

例如，您可以创建一个欢迎电子邮件促销活动，其中包含跨不同渠道的一系列消息，例如电子邮件、短信和推送。 您还可以在客户完成购买后发送跟进电子邮件，或通过短信向客户发送个性化的生日消息。

通过使用渠道活动，您可以创建全面的个性化营销活动，在多个接触点吸引客户并促进转化。

* [电子邮件](email.md)
* [推送](push.md)
* [短信](sms.md)

## 流量控制活动 {#flow-control}

以下活动特定于组织和执行工作流。 他们的主要任务是协调其他活动：

* 此 [And — 连接](and-join.md) 利用活动，可同步工作流的多个执行分支。
* 此 [结束](end.md) 活动允许您以图形方式标记工作流的结尾。 这些活动没有功能影响，因此是可选的。
* 此 [分支](fork.md) 利用活动，可创建叫客过渡以同时开始多个活动。
* 此 [等待](wait.md) 活动可暂停执行部分工作流。

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

