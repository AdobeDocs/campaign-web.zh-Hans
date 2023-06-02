---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="Alpha" type="Positive"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
source-git-commit: 880f02c460d75c50347fb5716fbcdf7cd3908422
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 7%

---

# 访问和监控工作流 {#access-monitor}


>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="工作流"
>abstract="在此屏幕中，您可以访问工作流的完整列表，检查其状态、上次/下次执行日期，以及创建新工作流。 浏览到“模板”选项卡以访问可用的工作流模板。"

## 访问和管理工作流 {#access}

此 **[!UICONTROL 工作流]** 菜单可让您访问工作流的完整列表。 此列表包含两者 **独立工作流** 已从此屏幕创建，并且 **活动工作流**，这些资源已在营销策划中创建。

![](assets/workflow-list.png)

列表中的每个工作流都会显示其当前工作流程的信息 [状态](#status)、上次执行或修改的时间，以及下一个计划执行日期和时间。

您可以通过单击 **[!UICONTROL 为自定义布局配置列]** 图标图标。 这样，您就可以向列表中添加其他信息，例如每个工作流中出错的最后一个活动或应用的定向维度。

此外，还提供搜索栏和过滤器，以便于在列表中轻松搜索。 例如，您可以筛选工作流以仅显示属于某个促销活动的工作流，或显示在特定日期范围内处理的工作流。

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

工作流模板包含预配置的活动和全局属性配置，可重复用于创建新工作流。 它们是从客户端控制台创建的。 [了解如何使用模板](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)
