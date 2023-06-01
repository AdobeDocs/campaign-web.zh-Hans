---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: c842829915784654b7130563d36dea188e84ff3d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 创建工作流 {#create}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="工作流属性"
>abstract="待定"

## 创建工作流 {#create-workflow}

在Campaign v8 Web中创建工作流的第一步是将其创建为独立工作流或直接在营销策划中创建，并定义其常规属性。 为此，请执行以下步骤：

1. 首先，决定是要创建独立的工作流，还是直接在营销策划中集成该工作流：

   * **独立工作流程**：导航到工作流菜单，然后单击右上角的创建工作流按钮。
   * **营销活动工作流：** 导航到促销活动菜单，然后打开要创建新工作流的促销活动。 单击“工作流”选项卡右上角的创建工作流按钮。

   此时将显示工作流的“属性”对话框。

   ![](assets/workflow-create.png)

1. 选择要用于创建工作流并为工作流提供标签的模板。

   工作流模板包含预配置的活动和全局属性配置，可重复用于创建新工作流。 它们是从客户端控制台创建的。 [了解如何使用模板](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. 如果要为工作流配置特定设置（如存储文件夹和时区），请展开其他选项部分。 [了解如何配置工作流属性](workflow-settings.md)

1. 单击创建工作流按钮以确认创建工作流。

创建工作流后，您现在可以开始使用专用可视画布编排工作流将执行的各种任务。 [了解如何编排工作流活动](#build)

## 编排工作流活动 {#build}

一旦您拥有 [已创建工作流](create-workflow.md)，无论是从工作流菜单还是营销策划中，您都可以开始编排它将执行的不同任务。 为此，提供了一个可视画布，允许您构建工作流图。 在此图表中，您可以添加各种活动并按顺序连接它们。

在配置的此阶段，图表会显示一个开始图标，表示工作流的开始。 要添加第一个活动，请单击连接到开始图标的+按钮。

此时会显示可添加到图中的活动列表。 可用的活动取决于您在工作流图中的位置。 例如，添加第一个活动时，您可以通过定位受众、拆分工作流路径或设置等待活动以延迟工作流执行来启动工作流。 另一方面，在构建受众活动后，您可以通过定位活动来优化目标，通过渠道活动向受众发送投放，或通过流控制活动来组织工作流过程。

![](assets/workflow-start.png)

将活动添加到图后，将显示一个右侧窗格，允许您使用特定设置配置新添加的活动。 有关如何配置每个活动的详细信息，请参阅 [本节](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

根据您希望工作流执行的任务，重复此过程，添加所需数量的活动。 请注意，您还可以在两个活动之间插入新活动。 为此，请在活动之间的过渡中单击+按钮，选择所需的活动并在右侧窗格中对其进行配置。

要删除某个活动，请在画布中选择该活动，然后单击活动属性中的删除图标。

>[!TIP]
>
>您可以选择个性化每个活动之间的过渡名称。 要实现此目的，请选择过渡，然后在右窗格中更改其标签。

完成工作流后，在图末尾添加结束活动。 此活动允许您以可视方式标记工作流的结尾，而不会对功能产生影响。

成功设计工作流图后，您可以执行工作流并跟踪其各种任务的进度。 [了解如何启动工作流并监视其执行](start-monitor-workflows.md)
