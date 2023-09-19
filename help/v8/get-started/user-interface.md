---
audience: end-user
title: 探索界面
description: Campaign v8 Web 用户界面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: 5e2af07f54fae9b0d64d173388be14639e6aaaa2
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 73%

---

# 探索界面 {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="探索界面"
>abstract="新的 Campaign v8 Web 界面提供了集成、直观和一致的用户体验。"

新的 Campaign v8 Web 界面提供了直观的现代用户体验，可简化营销活动的设计和投放。此新界面已与Adobe Experience Cloud应用程序和解决方案集成。


>[!NOTE]
>
>此文档经常更新以反映产品用户界面中的最新更改。但是，某些屏幕快照可能与用户界面略有不同。


## 左侧导航菜单 {#user-interface-left-nav}

浏览左侧链接以访问 Campaign v8 Web 功能。多个链接显示了可排序和筛选的对象的列表。您还可以配置列以显示所需的所有信息。请参阅此[章节](#list-screens)。某些列表屏幕为只读。 左侧导航菜单和列表中显示的项目取决于您的用户权限。 要了解有关权限的更多信息，请参阅 [本节](permissions.md).

![](assets/home.png)

### 主页 {#user-interface-home}

此屏幕包含用于快速访问主要 Campaign v8 Web 功能的关键链接和资源。

**最近项目**&#x200B;列表提供了最近创建和修改的投放的快捷方式。此列表显示了它们的渠道、状态、所有者、创建日期和修改日期。

利用&#x200B;**关键绩效指标 (KPI)**，可以通过常见 KPI 检查平台有效性。要了解有关这些KPI的更多信息，请参阅 [此页面](../reporting/kpis.md).

从主页的&#x200B;**学习**&#x200B;部分访问 Campaign v8 Web 关键帮助页面。

### 探索工具 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="**探索工具**&#x200B;菜单使用与客户端控制台中的文件夹层次结构相同的文件夹层次结构显示所有 Campaign 组件和对象。浏览您的所有 Campaign v8 组件、文件夹和架构，检查关联的权限，然后从此菜单创建文件夹和子文件夹。"

**探索工具**&#x200B;菜单使用与客户端控制台中的文件夹层次结构相同的文件夹层次结构显示所有 Campaign 资源和对象。浏览所有 Campaign v8 组件、文件夹和模式，并创建投放、工作流和营销活动。

中显示的项目 **资源管理器** 取决于您的用户权限。 如果您拥有适当的权限，您还可以添加文件夹和子文件夹。 要了解有关权限的更多信息，请参阅 [本节](permissions.md).

与任何列表屏幕中一样，您可以配置列来个性化显示以查看所需的所有信息。请参阅此[章节](#list-screens)。

有关 Campaign 探索工具、文件夹层次结构和资源的更多信息，请参阅此 [Campaign v8（控制台）文档 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}。

### Campaign 管理 {#user-interface-campaign-management}

在“营销活动管理”部分中，可访问市场营销活动、投放情况和工作流。

* **营销活动** - 这是您的营销活动和营销活动模板的列表。默认情况下，可查看每个营销活动的开始/结束/创建/上次修改日期、当前状态以及创建它的 Campaign 操作员的姓名。可按状态、开始/结束日期和文件夹筛选该列表，也可创建高级筛选器以定义您自己的筛选条件。可[在此部分中](../campaigns/gs-campaigns.md)详细了解营销活动。

* **投放** - 浏览您的投放列表。默认情况下，您可以查看它们的状态、最后修改日期以及关键 KPI。您可以按状态、联系日期或渠道筛选列表。单击电子邮件投放以打开其仪表板来获取投放详细信息的概述。其他渠道上的投放是只读的。可[在此部分中](../msg/gs-messages.md)详细了解投放。

  使用&#x200B;**更多操作**&#x200B;按钮删除或重复投放。

  ![](assets/more-actions.png){width="70%" align="left"}

* **工作流** - 可在此屏幕中访问工作流和工作流模板的完整列表。可检查其状态、上次/下次执行日期，并可创建新的工作流或新的工作流模板。可用与筛选其他对象相同的条件筛选该列表。此外，还可筛选属于或不属于营销活动的工作流。可[在此部分中](../workflows/gs-workflows.md)详细了解工作流。


### 客户管理 {#user-interface-customer-management}

在“客户管理”部分中，您可以查看收件人、受众和订阅。这些列表为只读状态。

* **收件人** - 访问您的收件人数据库。默认情况下，您可以查看他们的电子邮件地址、名字和姓氏。了解有关收件人的更多信息，请参阅 [本节](../audience/about-recipients.md).
* **受众** - 这是您的受众列表。默认情况下，您可以查看它们的类型、来源、创建/最后修改日期和标签。您可以按来源筛选列表。要了解有关受众和列表的更多信息，请参阅 [本节](../audience/about-recipients.md).
* **订阅** - 浏览您的订阅列表。默认情况下，您可以查看它们的类型、模式和标签。请参阅 [Adobe Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}，了解如何管理订阅和退订。

### 决策管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="选件"
>abstract="浏览使用在控制台中创建的选件和选件模板的列表。 **互动** 模块。 这些列表为只读状态。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html" text="将优惠添加到投放"

在决策管理部分，您可以查看优惠和优惠模板。 这些列表为只读状态。

* **选件**  — 浏览在控制台中创建的选件和选件模板的列表，使用 **互动** 模块。 默认情况下，您可以查看它们的状态、开始/结束日期和环境。您可以按状态和开始/结束日期筛选列表。也会提供优惠模板。

了解如何在的电子邮件和短信中创建和发送优惠 [本节](../content/offers.md).

## 顶部栏 {#top-bar}

利用界面的顶部栏，可以：

* 以Beta测试人员身份分享您的反馈
* 在组织和实例之间切换
* 在 Adobe Experience Cloud 应用程序之间切换
* 访问帮助页面、联系支持人员和共享反馈。您可以从搜索字段中搜索帮助文章和视频。

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->


## 情景帮助 {#user-interface-help}

界面中提供了上下文帮助。当 `?` 图标可用时，单击该图标可显示帮助信息和相关文档链接。

![](assets/context-help.png){width="40%" align="left"}

在新的Beta版本中， **具有Gen AI的知识助手** 嵌入在上下文帮助中的内容彻底改变了文档搜索和操作方法问题，您可以轻松地在庞大的文档存储库中筛选，即时查明您所需的精确信息。

借助Campaign Gen AI的功能，此助手可改变您的体验，使信息检索和问题解决变得轻而易举。 无论您是在复杂任务中寻求指导，还是浏览大量文档，我们配备了Gen AI的知识助手都是您的终极伙伴，可在每次交互中提供无与伦比的效率和准确性。

在[此章节](using-ai.md)中了解更多信息。

## 支持的浏览器 {#browsers}

Campaign v8 Web 旨在以最佳状态在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中运行。您可能无法在较旧版本或其他浏览器上使用某些功能。

## 语言偏好设置 {#language-pref}

Campaign v8 Web 目前提供以下语言版本：

* 英语（美国）- EN-US
* 法语 - FR
* 德语 - DE
* 意大利语 - IT
* 西班牙语 - ES
* 葡萄牙语（巴西）- PTBR
* 日语 - JP
* 朝鲜语 - KR
* 简体中文 - CHS
* 繁体中文 - CHT


您的Campaign Web默认语言由用户配置文件中指定的首选语言决定。 它与Campaign服务器和客户端控制台的语言无关。

要更改您的语言，请执行以下操作：

1. 单击右上角的配置文件图标，然后选择&#x200B;**偏好设置**。
1. 然后单击电子邮件地址下方显示的语言链接。
1. 选择您的首选语言并单击&#x200B;**保存**。如果您使用的组件未本地化为您的首选语言，可以选择第二语言。

## 深色主题 {#dark-theme}

您可以从配置文件图标切换到深色主题。 使用 **深色主题** 切换以启用/禁用它。

## 了解详情 {#learn-more}

参阅[此页面](list-filters.md)，了解如何浏览、搜索和筛选 Campaign 环境中可用的列表。


<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建区段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建区段。"

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_reporting_email_exportation"
>title="导出"
>abstract="只能导出所选页面。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全球报告发送"
>abstract="跟踪报表量度在此屏幕中可见"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全球报告跟踪"
>abstract="跟踪报表量度在此屏幕中可见"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Campaign 中的工作流列表"
>abstract="Campaign 中的工作流列表"

<!-- delivery settings-->


