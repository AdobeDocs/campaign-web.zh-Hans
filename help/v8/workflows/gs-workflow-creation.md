---
audience: end-user
title: 创建工作流的主要原则
description: 了解使用 Adobe Campaign Web 工作流的关键原则
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: ht
source-wordcount: '300'
ht-degree: 100%

---

# 创建工作流的主要原则 {#gs-workflow-creation}

借助 Adobe Campaign Web，您可以在可视化画布上构建工作流，设计跨渠道流程，例如分段、营销活动执行和文件处理。

## 工作流中有什么？ {#gs-workflow-inside}

工作流图展示了已规划的流程。它描述要执行的各种任务及其如何链接在一起。

![显示任务及其连接的工作流示例图](assets/workflow-example.png){zoomable="yes"}

每个工作流包含：

* **活动**：活动是要执行的任务。图中的图标代表不同的活动。每个活动既具有特定属性，也包含所有活动通用的属性。

  在工作流图中，一个给定活动可产生多个任务，尤其是存在循环或重复发生的行动时。

* **过渡**：过渡将源活动链接到目标活动并定义它们的顺序。

* **工作表**：工作表包含了过渡所携带的所有信息。每个工作流均使用多个工作表。这些表中的数据可在整个工作流生命周期中使用。

## 创建工作流的关键步骤 {#gs-workflow-steps}

营销活动提供了两种创建工作流的方式：

1. 您可以通过&#x200B;**工作流**&#x200B;菜单创建独立的工作流。

   ![创建独立工作流的界面屏幕快照](assets/create-a-standalone-wf.png){zoomable="yes"}

1. 可直接在营销活动中从营销活动的&#x200B;**工作流**&#x200B;选项卡创建工作流。如果工作流被纳入某个营销活动，它将在该活动的所有工作流中一起执行，并且其报表量度将统一归类到该营销活动下。

   ![在营销活动中创建工作流的界面的屏幕快照](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

创建工作流的关键步骤如下所示：

![工作流创建流程示意图](assets/workflow-creation-process.png){zoomable="yes"}

以下部分详细介绍了这些步骤：

1. [创建您的工作流并定义其属性](create-workflow.md)
1. [编排和配置活动](orchestrate-activities.md)
1. [配置工作流高级设置](workflow-settings.md)
1. [启动工作流并监控其执行情况](start-monitor-workflows.md)