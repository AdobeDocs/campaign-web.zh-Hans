---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 4%

---

# 启动和监测工作流 {#start-monitor}

创建工作流并设计要在画布中执行的任务后，即可启动工作流并监控其执行情况。

## 启动工作流 {#start}

要启动工作流，请导航到&#x200B;**[!UICONTROL 工作流]**&#x200B;菜单或关联的营销活动，然后单击画布右上角的&#x200B;**[!UICONTROL 开始]**&#x200B;按钮。

工作流运行后，将按顺序执行画布中的每个活动，直到到达工作流结尾为止。

您可以使用可视流量实时跟踪目标用户档案的进度。 这允许您快速识别每个活动的状态以及它们之间转换的用户档案数。

![](assets/workflow-execution.png){zoomable="yes"}

## 工作流过渡 {#transitions}

在工作流中，通过过渡从一个活动传输到另一个活动的数据存储在临时工作表中。 可以为每个过渡显示此数据。 要实现此目的，请选择过渡以在屏幕右侧打开其属性。

* 单击&#x200B;**[!UICONTROL 预览架构]**&#x200B;以显示工作表的架构。
* 单击&#x200B;**[!UICONTROL 预览结果]**&#x200B;以可视化在所选过渡中传输的数据。

![](assets/transition.png){zoomable="yes"}

## 监测活动执行 {#activities}

通过每个活动框右上角的视觉指示器，可检查其执行情况：

| 视觉指示器 | 说明 |
|-----|------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | 当前正在执行活动。 |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | 该活动需要您注意。 这可能涉及确认发送投放或采取必要操作。 |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | 活动遇到错误。 要解决此问题，请打开工作流日志以获取更多信息。 |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | 已成功执行活动。 |

## 监测日志和任务 {#logs-tasks}

监测工作流日志和任务是分析工作流并确保其正常运行的关键步骤。 可从操作工具栏中提供的&#x200B;**[!UICONTROL 日志]**&#x200B;图标以及每个活动的属性窗格中访问它们。

**[!UICONTROL 日志和任务]**&#x200B;菜单提供工作流执行的历史记录，记录所有用户操作和遇到的错误。 此历史记录会保存至工作流[执行选项](workflow-settings.md)中指定的持续时间。 在此持续时间内，将保存所有消息，即使重新启动工作流后也是如此。 如果不想保存上一次执行的消息，请单击&#x200B;**[!UICONTROL 清除历史记录]**&#x200B;按钮。

![](assets/workflow-logs.png){zoomable="yes"}

提供了两种类型的信息：

* **[!UICONTROL 日志]**&#x200B;选项卡包含所有工作流活动的执行历史记录。 它按时间顺序对执行的操作和执行错误进行索引。
* **[!UICONTROL 任务]**&#x200B;选项卡详细列出了活动的执行顺序。

在这两个选项卡中，您可以选择显示的列及其顺序，应用过滤器，并使用搜索字段快速查找所需信息。

## 工作流执行命令 {#execution-commands}

右上角的操作栏提供了用于管理工作流执行的命令。 您可以：

* **[!UICONTROL 开始]** / **[!UICONTROL 恢复]**&#x200B;工作流执行，工作流执行后会进入“进行中”状态。 如果工作流已暂停，则会恢复它，否则会启动它并激活初始活动。

* **[!UICONTROL 暂停]**&#x200B;工作流执行，该工作流随后会呈现“已暂停”状态。 在恢复之前，不会激活任何新活动，但不会暂停正在进行的操作。

* **[!UICONTROL 停止]**&#x200B;正在执行的工作流，该工作流随后将呈现“已完成”状态。 如果可能，正在执行的操作会被中断。 您不能从工作流停止的位置恢复工作流。
