---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="有限发布版"
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: 6694976596909226cadbb0997c6663ec17a9e39b
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 28%

---

# 访问和管理工作流 {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="工作流"
>abstract="在此屏幕中可访问独立和营销活动工作流的列表、检查工作流的当前状态、上次/下次执行日期以及创建新工作流。浏览到“模板”选项卡以访问可用的工作流模板。"

此 **[!UICONTROL 工作流]** 菜单可让您访问工作流的完整列表。 此列表包含两者 **独立工作流** 已从此屏幕创建，并且 **活动工作流**，这些规则已在营销策划中创建。

![](assets/workflow-list.png)

列表中的每个工作流都会显示其当前工作流程的信息 [状态](#status)、上次执行或修改的时间，以及下一个计划执行日期和时间。

可以通过单击列表右上角的&#x200B;**[!UICONTROL 为自定义版面配置列]**&#x200B;图标来自定义显示的列。这样，您就可以向列表添加其他信息，如每个工作流中出错的最后一个活动或应用的定向维度。

此外，还可使用搜索栏和过滤器以便在列表中轻松搜索。例如，您可以筛选工作流以仅显示属于某个营销策划的工作流，或显示在特定日期范围内处理的工作流。

要复制或删除工作流，请单击省略号按钮，然后选择 **[!UICONTROL 复制]** 或 **[!UICONTROL 删除]**.

>[!NOTE]
>
>您可以复制正在进行的工作流，但无法删除它。

## 工作流的状态 {#status}

工作流可以具有多种状态：

* **[!UICONTROL 草稿]**：已创建并保存工作流。
* **[!UICONTROL 进行中]**：工作流当前正在运行。
* **[!UICONTROL 已完成]**：工作流执行完成。
* **[!UICONTROL 已暂停]**：工作流已暂停。
* **[!UICONTROL 错误]**：工作流遇到错误。 打开工作流并访问日志和任务，以识别错误并解决它。 [了解如何监测日志和任务](start-monitor-workflows.md#logs-tasks)

有关如何启动和监测工作流执行的详细信息，请参阅 [此页面](start-monitor-workflows.md).

## 工作流模板 {#templates}

此 **[!UICONTROL 模板]** 选项卡列出了所有可用的工作流模板。

工作流模板包含预配置的活动和可重复用于创建新工作流的整体属性配置。

您可以从现有工作流创建工作流模板，或从头开始创建工作流模板。 [了解如何创建工作流模板](create-workflow.md#work-with-workflow-templates-workflow-templates)
