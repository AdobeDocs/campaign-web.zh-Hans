---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 33%

---


# 工作流创建的主要原则 {#gs-workflow-creation}

借助Campaign v8 Web，您可以将工作流构建到可视画布中，以设计跨渠道流程，例如分段、活动执行、文件处理。

工作流可以从“工作流”菜单作为独立工作流创建，也可以直接在营销策划中创建，在这种情况下，工作流将链接到营销策划并与所有其他营销策划的工作流一起执行。

## 工作流的内容

工作流图是应发生情况的表示形式。 它描述了要执行的各种任务以及如何将它们链接在一起。

![](assets/workflow-example.png)

每个工作流包含：

* **活动**：活动是要执行的任务。 各种活动在图表中以图标表示。 每个活动都有特定的属性以及所有活动通用的其他属性。

   在工作流图中，一个给定活动可以产生多个任务，特别是当存在循环或定期行动时。

* **过渡**：过渡将源活动链接到目标活动并定义其序列。

* **工作表**：工作表包含了过渡所携带的所有信息。每个工作流均使用多个工作表。这些表中传送的数据可在工作流的整个生命周期中使用。

## 创建工作流的主要步骤

创建工作流的主要步骤如下所示：

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="商机" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>创建工作流</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="不常见" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>编排活动</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="验证" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>配置高级设置（可选）</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="启动和监控工作流" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>启动和监控工作流执行</strong></a>
</div>
<p>
</td>
</tr></table>