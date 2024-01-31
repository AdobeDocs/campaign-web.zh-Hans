---
audience: end-user
title: 创建工作流的主要原则
description: 了解使用 Adobe Campaign Web 工作流的关键原则
badge: label="有限发布版"
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: f614919e0ad253aa4625f774e7fe102426e25807
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 91%

---


# 创建工作流的主要原则 {#gs-workflow-creation}

借助Adobe Campaign Web，您可以将工作流构建到可视画布中，以设计跨渠道流程，例如分段、活动执行、文件处理。


## 工作流中有什么？ {#gs-workflow-inside}

工作流图表示应该发生什么。它描述要执行的各种任务及其如何链接在一起。

![](assets/workflow-example.png) {zoomable=&quot;yes&quot;}

每个工作流包含：

* **活动**：活动是要执行的任务。在图上用图标表示各种活动。每个活动都有特定属性和所有活动共有的其他属性。

  在工作流图中，一个给定活动可产生多个任务，尤其是存在循环或重复发生的行动时。

* **过渡**：过渡将源活动链接到目标活动并定义它们的顺序。

* **工作表**：工作表包含了过渡所携带的所有信息。每个工作流均使用多个工作表。在工作流的整个生命周期内均可使用在这些表中传递的数据。

## 创建工作流的关键步骤 {#gs-workflow-steps}


营销活动提供了两种创建工作流的方式：

1. 可从&#x200B;**工作流**&#x200B;菜单创建工作流作为独立的工作流。

   ![](assets/create-a-standalone-wf.png)

1. 可直接在营销活动中从营销活动的&#x200B;**工作流**&#x200B;选项卡创建工作流。当工作流包括在营销活动中时，将它与所有其他营销活动的工作流一起执行，并且报告量度全都集中在营销活动级别。

   ![](assets/create-a-wf-from-a-campaign.png)


创建工作流的关键步骤如下所示：

![](assets/workflow-creation-process.png)

以下部分详细介绍了这些步骤：

1. [创建您的工作流并定义其属性](create-workflow.md)
1. [编排和配置活动](orchestrate-activities.md)
1. [配置工作流高级设置](workflow-settings.md)
1. [启动工作流并监控其执行情况](start-monitor-workflows.md)
