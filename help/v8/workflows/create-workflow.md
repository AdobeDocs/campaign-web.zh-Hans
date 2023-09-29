---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用Adobe Campaign Web创建工作流
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 9272419162d95859147949717e294aa7ae24fc71
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 21%

---


# 创建工作流 {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="工作流属性"
>abstract="在此屏幕中，选择要用于创建工作流的模板并指定标签。展开“其他选项”部分以配置更多设置，例如工作流内部名称、其文件夹、时区和主管组等。强烈建议选择一个主管组，以便如果出错，可提醒操作员。"


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="营销活动中工作流的列表"
>abstract="**工作流**&#x200B;选项卡列出链接到当前营销活动的所有工作流。单击工作流的名称以编辑该工作流。使用&#x200B;**创建工作流**&#x200B;按钮为此营销活动添加新工作流。"


您可以在营销策划中创建独立的工作流或工作流。 第一步是选择模板并定义其常规属性。 然后，您可以根据需要配置其他设置。

为此，请执行以下步骤：

1. 创建 **独立工作流程**，浏览到 **工作流程** 菜单。

   创建 **活动工作流**，浏览到 **营销活动** 菜单，然后打开要为其创建新工作流的营销策划。

1. 单击 **[!UICONTROL 创建工作流]** 按钮来打开屏幕。

   ![](assets/workflow-create.png)

1. 在工作流中 **属性** 对话框，选择用于创建工作流的模板（也可以使用默认的内置模板）。 要了解有关模板的更多信息，请参阅 [以下部分](#work-with-workflow-templates-workflow-templates).

1. 输入工作流的标签。 此外，我们强烈建议您在 **[!UICONTROL 其他选项]** 部分。

1. 展开 **[!UICONTROL 其他选项]** 部分，以便为工作流配置更多设置。 了解如何在中配置工作流属性 [此页面](workflow-settings.md#properties)

   ![](assets/workflow-additional-options.png)

1. 单击 **[!UICONTROL 创建工作流]** 按钮以确认创建工作流。

您的工作流现已创建并可在工作流列表中使用。 您现在可以访问其可视画布并开始添加、配置和编排其将执行的任务。 了解如何在中编排工作流活动 [此页面](orchestrate-activities.md).

## 使用工作流模板 {#workflow-templates}


>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="工作流模板"
>abstract="工作流模板包含可为创建新工作流重用的预先配置的设置和活动。"

工作流模板包含可为创建新工作流重用的预先配置的设置和活动。创建工作流时，您可以从工作流属性中选择工作流的模板。 默认情况下，会提供一个空模板。

您可以从现有工作流创建模板，或从头开始创建新模板。 这两种方法详见下文。


>[!BEGINTABS]

>[!TAB 从现有工作流创建模板]

要从现有工作流创建工作流模板，请执行以下步骤：

1. 打开至 **工作流** 菜单并浏览到工作流以另存为模板。
1. 单击工作流名称右侧的三个圆点，然后选择 **复制为模板**.

   ![](assets/wf-copy-as-template.png)

1. 在弹出窗口中，确认创建模板。
1. 在工作流模板画布中，根据需要检查、添加和配置活动。
1. 浏览到设置，从 **设置** 按钮，以更改工作流模板的名称，并输入说明。
1. 选择 **文件夹** 和 **执行文件夹** 模板的。 文件夹是保存工作流模板的位置。 执行文件夹是保存基于此模板创建的工作流的文件夹。

   ![](assets/wf-settings-template.png)

   其他属性与工作流通用。 请参阅[此页面](workflow-settings.md#properties)以了解详情

1. 保存您的更改。

现在，模板列表中提供了工作流模板。 您可以基于此模板创建工作流。 此工作流将使用该模板中定义的设置和活动进行预配置。


>[!TAB 从头开始创建模板]


要从头开始创建工作流模板，请执行以下步骤：

1. 打开至 **工作流** 并浏览至 **模板** 选项卡。 您可以查看可用工作流模板的列表。
1. 单击 **[!UICONTROL 创建模板]** 按钮来打开屏幕。
1. 输入标签并打开附加选项，以输入工作流模板的描述。
1. 选择模板的文件夹和执行文件夹。 文件夹是保存工作流模板的位置。 执行文件夹是保存基于此模板创建的工作流的文件夹。

   ![](assets/new-wf-template.png)

   其他属性与工作流通用。 请参阅[此页面](workflow-settings.md#properties)以了解详情

1. 单击 **创建** 按钮以确认您的设置。
1. 在工作流模板画布中，根据需要添加和配置活动。

   ![](assets/wf-template-activities.png)

1. 保存您的更改。

现在，模板列表中提供了工作流模板。 您可以基于此模板创建工作流。 此工作流将使用该模板中定义的设置和活动进行预配置。

>[!ENDTABS]
