---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用Adobe Campaign Web创建工作流
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 18%

---

# 创建工作流 {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="营销活动中工作流的列表"
>abstract="**工作流**&#x200B;选项卡列出链接到当前营销活动的所有工作流。单击工作流的名称以编辑该工作流。使用&#x200B;**创建工作流**&#x200B;按钮为此营销活动添加新工作流。"

您可以在营销策划中创建独立的工作流或工作流。 第一步是选择模板并定义其常规属性。 然后，您可以根据需要配置其他设置。

为此，请执行以下步骤：

1. 要创建&#x200B;**独立工作流**，请浏览到&#x200B;**工作流**&#x200B;菜单。 要创建&#x200B;**营销活动工作流**，请浏览到&#x200B;**营销活动**&#x200B;菜单，然后打开要为其创建新工作流的营销活动。

1. 单击屏幕右上角的&#x200B;**[!UICONTROL 创建工作流]**&#x200B;按钮。

   ![屏幕右上角显示“创建工作流”按钮的屏幕快照。](assets/workflow-create.png){zoomable="yes"}

1. 在工作流&#x200B;**属性**&#x200B;对话框中，选择要用于创建工作流的模板（也可以使用默认的内置模板）。 [了解有关工作流模板的更多信息](#workflow-templates)。

1. 输入工作流的标签。 此外，在屏幕的&#x200B;**[!UICONTROL 其他选项]**&#x200B;部分的专用字段中向工作流添加描述。

1. 展开&#x200B;**[!UICONTROL 其他选项]**&#x200B;部分以配置工作流的其他设置。 了解如何在[此页面](workflow-settings.md#properties)中配置工作流属性。

   ![显示用于配置工作流设置的“其他选项”部分的屏幕截图。](assets/workflow-additional-options.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 创建工作流]**&#x200B;按钮以确认创建工作流。

您的工作流现已创建并在工作流列表中可用。 您可以访问其可视画布，并开始添加、配置和编排它将执行的任务。 [了解如何编排工作流活动](orchestrate-activities.md)。

## 使用工作流模板 {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="工作流模板"
>abstract="工作流模板包含可重用于创建新工作流的预先配置的设置和活动。"

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="工作流属性"
>abstract="工作流模板包含可重用于创建新工作流的预先配置的设置和活动。在此屏幕中，输入工作流模板的标签并配置其设置，例如其内部名称、文件夹和执行文件夹、时区和主管组。"

工作流模板包含可重用于创建新工作流的预先配置的设置和活动。创建工作流时，请从工作流属性中选择工作流的模板。 默认情况下，会提供一个空模板。

您可以从现有工作流创建模板，或从头开始创建新模板。 这两种方法详见下文。

>[!BEGINTABS]

>[!TAB 从现有工作流创建模板]

要从现有工作流创建工作流模板，请执行以下步骤：

1. 打开&#x200B;**工作流**&#x200B;菜单并浏览到要另存为模板的工作流。
1. 单击工作流名称右侧的三个圆点，然后选择&#x200B;**复制为模板**。

   ![在工作流菜单中显示“复制为模板”选项的屏幕快照。](assets/wf-copy-as-template.png){zoomable="yes"}

1. 在弹出窗口中，确认创建模板。
1. 在工作流模板画布中，根据需要检查、添加和配置活动。
1. 从&#x200B;**设置**&#x200B;按钮浏览到设置以更改工作流模板的名称，并输入说明。
1. 选择模板的&#x200B;**文件夹**&#x200B;和&#x200B;**执行文件夹**。 文件夹是保存工作流模板的位置。 执行文件夹是保存基于此模板创建的工作流的文件夹。

   ![显示工作流模板中文件夹和执行文件夹的设置的屏幕截图。](assets/wf-settings-template.png){zoomable="yes"}

   其他属性与工作流通用。 请参阅[此页面](workflow-settings.md#properties)以了解详情。

1. 保存您的更改。

现在，模板列表中提供了工作流模板。 您可以基于此模板创建工作流。 此工作流将使用该模板中定义的设置和活动进行预配置。

>[!TAB 从头开始创建模板]

要从头开始创建工作流模板，请执行以下步骤：

1. 打开&#x200B;**工作流**&#x200B;菜单并浏览到&#x200B;**模板**&#x200B;选项卡。 您可以查看可用工作流模板的列表。
1. 单击屏幕右上角的&#x200B;**[!UICONTROL 创建模板]**&#x200B;按钮。
1. 输入标签并打开附加选项，以输入工作流模板的描述。
1. 选择模板的文件夹和执行文件夹。 文件夹是保存工作流模板的位置。 执行文件夹是保存基于此模板创建的工作流的文件夹。

   ![显示创建具有文件夹和执行文件夹设置的新工作流模板的屏幕截图。](assets/new-wf-template.png){zoomable="yes"}

   其他属性与工作流通用。 请参阅[此页面](workflow-settings.md#properties)以了解详情。

1. 单击&#x200B;**创建**&#x200B;按钮确认您的设置。
1. 在工作流模板画布中，根据需要添加和配置活动。

   ![显示用于添加和配置活动的工作流模板画布的屏幕截图。](assets/wf-template-activities.png){zoomable="yes"}

1. 保存您的更改。

现在，模板列表中提供了工作流模板。 您可以基于此模板创建工作流。 此工作流将使用该模板中定义的设置和活动进行预配置。

>[!ENDTABS]