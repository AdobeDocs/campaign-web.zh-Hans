---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="Alpha"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 99%

---


# 创建工作流的主要原则 {#gs-workflow-creation}

通过 Campaign v8 Web，可使工作流成为视觉画布的组成部分，以设计跨渠道流程，如分段、执行营销活动和处理文件。

既可以从“工作流”菜单创建独立工作流，也可以直接在营销活动中创建工作流，在后一种情况下，工作流将链接到营销活动，并与所有其他营销活动的工作流一起执行。

## 工作流中有什么？

工作流图表示应该发生什么。它描述要执行的各种任务及其如何链接在一起。

![](assets/workflow-example.png)

每个工作流包含：

* **活动**：活动是要执行的任务。在图上用图标表示各种活动。每个活动都有特定属性和所有活动共有的其他属性。

  在工作流图中，一个给定活动可产生多个任务，尤其是存在循环或重复发生的行动时。

* **过渡**：过渡将源活动链接到目标活动并定义它们的顺序。

* **工作表**：工作表包含了过渡所携带的所有信息。每个工作流均使用多个工作表。这些表中传输的数据可以在整个工作流的生命周期内使用。

## 创建工作流的主要步骤

创建工作流的主要步骤如下所示：

![](assets/workflow-creation-process.png)
