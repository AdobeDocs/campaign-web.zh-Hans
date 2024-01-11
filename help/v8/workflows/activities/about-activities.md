---
audience: end-user
title: 使用工作流活动
description: 了解如何使用工作流活动
badge: label="有限发布版"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 35%

---


# 关于工作流活动 {#workflow-activities}

工作流活动分为三类。根据具体情况，可用的活动可能会有所不同。

以下各章节详细介绍了所有活动：

* [定位和数据管理活动](#targeting)
* [渠道活动](#channel)
* [流量控制活动](#flow-control)

![](../assets/workflow-activities.png)

## 定位和数据管理活动 {#targeting}

这些活动专门针对定位、操纵和丰富人口数据。利用这些活动，您可以通过定义受众并使用交集、并集或差集操作来拆分或合并这些受众，从而构建一个或多个目标。

* 使用 [保存受众](save-audience.md) 活动，用于更新现有受众，或从工作流上游计算的群体中创建新受众。
* 使用 [构建受众](build-audience.md) 用于定义目标群体的活动。 您可以选择现有受众，也可以使用查询建模器定义您自己的查询。
* 使用 [合并](combine.md) 对集客群体执行分段的活动。 您可以使用并集、交集或差集。
* 使用 [Split](split.md) 将传入群体划分为多个子集的活动。
* 使用 [调解](reconciliation.md) 活动，用于定义Adobe Campaign数据库中的数据与工作表中的数据（例如从外部文件加载的数据）之间的链接。
* 使用 [扩充](enrichment.md) 活动，以定义要在工作流中处理的附加数据。 通过此活动，您可以应用集客过渡并配置活动以使用附加数据填写输出过渡。
* 使用 [删除重复项](deduplication.md) 活动，用于删除集客活动结果中的重复项。
* 使用 [更改维度](change-dimension.md) 活动，以在构建工作流时更改定向维度。
* 使用 [加载文件](load-file.md) 活动以使用存储在外部文件中的用户档案和数据。


## 渠道活动 {#channel}

通过Adobe Campaign Web，您可以跨多个渠道自动执行营销活动。 您可以将渠道活动合并到画布中，以创建可以根据客户行为触发操作的跨渠道工作流。 以下各项 **渠道** 可用活动：电子邮件、短信、Android和iOS推送通知。 [了解如何在工作流的上下文中设置投放](channels.md).

## 流量控制活动 {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="结束活动"
>abstract="您可以使用&#x200B;**结束**&#x200B;活动以图形方式标记工作流的终点。此活动没有功能影响，因此是可选的。"

以下活动专用于组织和执行工作流。这些活动的主要任务是协调其他活动：

* 使用 [计划程序](scheduler.md) 工作流启动时计划的活动。
* 使用 [And — 连接](and-join.md) 活动，用于同步工作流的多个执行分支。
* 添加 **结束** 活动，以图形方式标记工作流的结尾。 此活动没有功能影响，因此是可选的。
* 使用 [分支](fork.md) 活动，用于创建叫客过渡以同时启动多个活动。
* 添加 [等待](wait.md) 活动用于暂时暂停执行部分工作流。

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

