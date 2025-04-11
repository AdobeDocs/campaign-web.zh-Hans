---
audience: end-user
title: 开始使用营销活动
description: 了解如何开始使用跨渠道营销活动
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 34%

---

# 访问和管理营销活动 {#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="营销活动计划"
>abstract="设置或修改营销活动计划。"

要访问和管理营销活动，请单击左侧导航栏中的&#x200B;**[!UICONTROL 营销活动]**&#x200B;菜单。

## 活动列表 {#access-campaigns}

在营销活动列表中，有两个选项卡可用：

* **浏览**&#x200B;选项卡将列出所有现有的营销活动。您可以单击一个营销活动以打开其仪表板，也可以通过单击&#x200B;**创建营销活动**&#x200B;按钮来创建新的营销活动。请参阅此[章节](create-campaigns.md#create-campaigns)。

* **模板**&#x200B;选项卡将列出所有可用的营销活动模板。您可以查看现有模板或创建新模板。 [了解更多信息](#manage-campaign-templates)。

![描述：营销活动列表屏幕显示“浏览”和“模板”选项卡，以及用于创建或查看营销活动的选项](assets/campaign-list.png)

默认情况下，列表中的每个营销活动都会显示有关其当前状态、开始和结束日期、创建日期、上次修改时间等的信息。

可以通过单击列表右上角的&#x200B;**为自定义版面配置列**&#x200B;图标来自定义显示的列。这允许您在营销活动列表中添加或删除列以及重新排序信息。

此外，还可使用搜索栏和过滤器以便在列表中轻松搜索。[了解详情](../get-started/user-interface.md#list-screens)。

例如，您可以根据营销活动计划进行过滤。打开过滤器面板并使用&#x200B;**开始 - 结束日期**&#x200B;部分：

![描述：过滤器面板显示按开始日期和结束日期过滤促销活动的选项](assets/campaign-filter-on-dates.png)

## 营销活动仪表板 {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="营销活动中的投放的列表"
>abstract="**投放**&#x200B;选项卡列出所有链接到当前营销活动的投放。单击投放的名称以编辑该投放。使用“创建投放”按钮为此营销活动添加新的投放。"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Campaign 中的工作流列表"
>abstract="**工作流**&#x200B;选项卡列出链接到当前营销活动的所有工作流。"

在促销活动列表的&#x200B;**浏览**&#x200B;选项卡中，单击促销活动名称以显示其详细信息。

![描述：营销活动仪表板屏幕显示工作流和投放的状态、计划和选项卡](assets/campaign-dashboard.png)

营销活动的状态和计划显示在屏幕顶部。 使用&#x200B;**设置**&#x200B;按钮更新营销活动的属性，如标签、文件夹和描述。 您还可以从设置屏幕更改营销活动计划。 在[本节](create-campaigns.md#campaign-schedule)中了解有关促销活动计划的更多信息。

在营销活动信息板中，使用&#x200B;**日志**&#x200B;和&#x200B;**报告**&#x200B;按钮监视您的营销活动。 在此[部分](create-campaigns.md#create-campaigns)中了解详情。

对于每个活动，仪表板都显示两个主要选项卡：工作流和投放。

* **工作流**&#x200B;选项卡列出了与营销活动关联的所有工作流。 此选项卡还可让您在营销活动中创建新的工作流。请参阅此[章节](create-campaigns.md#create-campaigns)。

* **投放**&#x200B;选项卡列出了在当前营销活动中创建的所有投放。 您还可以在营销活动中创建新的投放。请参阅此[章节](create-campaigns.md#create-campaigns)。

>[!NOTE]
>
>**投放**&#x200B;选项卡显示所有链接到该营销活动的投放。但是，无法从那里删除在工作流中创建的投放。要删除在工作流上下文中创建的投放，请从工作流中删除该投放活动。 [了解详情](../msg/gs-messages.md#delivery-delete)。

## 删除活动 {#campaign-delete}

您可以通过两种方式删除营销策划：

* 从营销活动列表中，单击省略号按钮，然后选择&#x200B;**删除**。

  ![描述：营销活动列表屏幕显示省略号按钮和删除选项](assets/delete-a-campaign-from-list.png)

* 在营销策划中，单击&#x200B;**更多**&#x200B;按钮，然后选择&#x200B;**删除**。

  ![描述：营销活动仪表板屏幕显示“更多”按钮和“删除”选项](assets/delete-a-campaign-from-dashboard.png)

## 复制营销活动 {#campaign-duplicate}

您可以通过两种方式复制营销策划：

* 从营销活动列表中，单击省略号按钮，然后选择&#x200B;**复制**。

* 在营销策划中，单击&#x200B;**更多**&#x200B;按钮，然后选择&#x200B;**复制**。

在这两种情况下，确认复制以创建新营销策划。 营销活动的标签为&#x200B;**`<label of the initial campaign>`**&#x200B;的副本。 浏览到Campaign设置以更新此标签。

## 使用活动模板 {#manage-campaign-templates}

营销活动模板包含预配置的设置，可重复用于创建新营销活动。 提供了一组内置模板来帮助您入门。 您可以创建和配置活动模板，然后从这些模板创建活动。

活动模板可以存储以下信息：

* 营销活动&#x200B;**设置**
* 营销活动&#x200B;**计划**
* 工作流模板
* 投放模板

要创建营销活动模板，请执行以下步骤：

1. 单击&#x200B;**[!UICONTROL 营销活动]**&#x200B;菜单，浏览到&#x200B;**模板**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 创建模板]**&#x200B;按钮。
1. 选择要使用的&#x200B;**模板**。 这样，您就可以基于之前创建的模板创建新模板。
1. 为模板提供标签。
1. 如果需要，请更改以下&#x200B;**其他选项**：内部名称、文件夹、代理人、说明和性质。
1. 定义营销活动的&#x200B;**计划**。 在[本节](create-campaigns.md#campaign-schedule)中了解如何设置营销活动计划。
1. 单击&#x200B;**创建**。
1. 将工作流和投放模板添加到您的营销活动。