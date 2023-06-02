---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 880f02c460d75c50347fb5716fbcdf7cd3908422
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 8%

---


# 创建工作流 {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="工作流属性"
>abstract="待定"

在Campaign v8 Web中创建工作流的第一步是将其创建为独立工作流或直接在营销策划中创建，并定义其常规属性。 为此，请执行以下步骤：

1. 首先，决定是要创建独立的工作流，还是直接在营销策划中集成该工作流：

   * **独立工作流程**：导航到工作流菜单，然后单击右上角的创建工作流按钮。
   * **营销活动工作流：** 导航到促销活动菜单，然后打开要创建新工作流的促销活动。 单击“工作流”选项卡右上角的创建工作流按钮。

   此时将显示工作流的“属性”对话框。

   ![](assets/workflow-create.png)

1. 选择要用于创建工作流并为工作流提供标签的模板。

   工作流模板包含预配置的活动和全局属性配置，可重复用于创建新工作流。 它们是从客户端控制台创建的。 [了解如何使用模板](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. 展开 **[!UICONTROL 其他选项]** 部分。 [了解如何配置工作流属性](workflow-settings.md)

1. 单击 **[!UICONTROL 创建工作流]** 按钮以确认创建工作流。

创建工作流后，您现在可以开始使用专用可视画布编排工作流将执行的各种任务。 [了解如何编排工作流活动](orchestrate-activities.md)
