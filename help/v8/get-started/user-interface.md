---
audience: end-user
title: 探索界面
description: Campaign v8 Web 用户界面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha" type="Positive"
source-git-commit: c801a96605eac09cd1b1753c3a22e4b61f81e97e
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 98%

---

# 探索界面 {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="探索界面"
>abstract="新的 Campaign v8 Web 界面提供了集成、直观和一致的用户体验。"

新的 Campaign v8 Web 界面提供了直观的现代用户体验，可简化营销活动的设计和投放。此新界面与 Adobe Experience Platform 集成。

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>此文档经常更新以反映产品用户界面中的最新更改。但是，某些屏幕快照可能与用户界面略有不同。


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## 左侧导航菜单

浏览左侧链接以访问 Campaign v8 Web 功能。多个链接显示了可排序和筛选的对象的列表。您还可以配置列以显示所需的所有信息。请参阅此[章节](#list-screens)。除了电子邮件投放列表之外的所有列表屏幕均为只读。单击任意列表项以进行编辑/无法在 Alpha 中进行查看。在将来版本中，所有列表都是可编辑的。左侧导航菜单中显示的项目取决于您的用户权限。

![](assets/home.png)

### 主页

此屏幕包含用于快速访问主要 Campaign v8 Web 功能的关键链接和资源。**最近项目**&#x200B;列表提供了最近创建和修改的投放的快捷方式。此列表显示了它们的创建和修改日期及状态。

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

从主页的下方部分访问 Campaign v8 Web 关键帮助页面。

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### 资源管理器

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="资源管理器"
>abstract="**资源管理器**&#x200B;菜单显示的文件夹层次结构与客户端控制台中的文件夹层次结构相同。浏览所有 Campaign v8 组件、文件夹和架构。除了电子邮件投放列表之外的所有列表屏幕均为只读。"

**资源管理器**&#x200B;菜单显示的文件夹层次结构与客户端控制台中的文件夹层次结构相同。浏览所有 Campaign v8 组件、文件夹和架构。

资源管理器中显示的项目取决于您的用户权限。

与任何列表屏幕中一样，您可以配置列来个性化显示以查看所需的所有信息。请参阅此[章节](#list-screens)。

有关Campaign资源管理器的更多信息，请参阅此 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign 管理

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="营销活动"
>abstract="这是您的营销活动列表。其中可显示有用的信息，例如它们的开始/结束/最后修改日期，以及它们的状态。您可以按状态或开始/结束日期筛选列表。单击“创建营销活动”按钮以添加新的营销活动。选择营销活动以查看其内容、投放情况和详细信息。浏览到“模板”选项卡以查看和创建模板。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="投放"
>abstract="浏览您的投放列表。可查看其状态、联系人、修改日期和关键 KPI。可按状态、联系日期或渠道筛选该列表。单击“创建投放”按钮以添加新投放。选择投放以查看其内容、受众和详细信息。"

在“营销活动管理”部分中，可访问市场营销活动、投放情况和工作流。

* **营销活动** - 这是您的营销活动和营销活动模板的列表。默认情况下，可查看每个营销活动的开始/结束/创建/上次修改日期、当前状态以及创建它的 Campaign 操作员的姓名。可按状态、开始/结束日期和文件夹筛选该列表，也可创建高级筛选器以定义您自己的筛选条件。可[在此部分中](../campaigns/gs-campaigns.md)详细了解营销活动。

* **投放** - 浏览您的投放列表。默认情况下，您可以查看它们的状态、最后修改日期以及关键 KPI。可按状态、联系日期或渠道筛选该列表。单击电子邮件投放以打开其仪表板来获取投放详细信息的概述。其他渠道上的投放是只读的。可[在此部分中](../msg/gs-messages.md)详细了解投放。

  使用&#x200B;**更多操作**&#x200B;按钮删除或重复投放。

  ![](assets/more-actions.png){width="70%" align="left"}

* **工作流** - 可在此屏幕中访问工作流和工作流模板的完整列表。可检查其状态、上次/下次执行日期，并可创建新的工作流或新的工作流模板。可用与筛选其他对象相同的条件筛选该列表。此外，还可筛选属于或不属于营销活动的工作流。可[在此部分中](../workflows/gs-workflows.md)详细了解工作流。


### 客户管理

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="收件人"
>abstract="访问您的收件人数据库。您可以查看有用的信息，例如他们的电子邮件地址、名字和姓氏。此列表为只读。"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="受众"
>abstract="这是您的受众列表。您可以查看它们的类型、来源、创建/最后修改日期和标签。您可以按来源筛选列表。此列表为只读。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="订阅列表"
>abstract="浏览您的订阅列表。您可以查看它们的类型、模式和标签。此列表为只读。"

* **收件人** - 访问您的收件人数据库。默认情况下，您可以查看他们的电子邮件地址、名字和姓氏。此列表为只读。
* **受众** - 这是您的受众列表。默认情况下，您可以查看它们的类型、来源、创建/最后修改日期和标签。您可以按来源筛选列表。此列表为只读。
* **订阅列表** - 浏览您的订阅列表。默认情况下，您可以查看它们的类型、模式和标签。此列表为只读。

### 决策管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="选件"
>abstract="浏览您的交互优惠列表。默认情况下，您可以查看它们的状态、开始/结束日期和环境。您可以按状态和开始/结束日期筛选列表。也会提供优惠模板。这些列表为只读状态。"

* **优惠** - 浏览您的交互优惠列表。默认情况下，您可以查看它们的状态、开始/结束日期和环境。您可以按状态和开始/结束日期筛选列表。也会提供优惠模板。这些列表为只读状态。

## 顶部栏

利用界面的顶部栏，您可以：

* 作为 Alpha 测试人员共享您的反馈
* 在组织和实例之间切换
* 在 Adobe Experience Cloud 应用程序之间切换
* 访问帮助页面、联系支持人员和共享反馈。您可以从搜索字段中搜索帮助文章和视频。

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## 配置列表屏幕 {#list-screens}

左侧导航菜单中的多个链接（例如&#x200B;**投放**&#x200B;或&#x200B;**营销活动**）显示对象列表。这些列表屏幕都是只读的，但电子邮件投放列表除外。

要更快地找到项目，您可以使用搜索栏或按上下文条件筛选列表。

![](assets/filter.png){width="70%" align="left"}

列表将以列的形式显示。可以更改列配置来显示其他信息。为此，请单击列表右上角的图标。您可以添加或删除列，并更改它们的显示顺序。

![](assets/columns.png){width="70%" align="left"}

您可以单击任意列标题来对列表中的项目进行排序。将显示一个箭头（向上或向下），指示列表已按该列排序。对于数字或日期列，向上箭头表示列表按升序排序，向下箭头表示列表按降序排序。对于字符串或字母数字列，值将按字母顺序列出。

## 上下文帮助和操作入门指南 {#contextual-help}

界面中提供了上下文帮助。在可用时，单击 **?** 图标以显示帮助信息和相关文档链接。

![](assets/context-help.png){width="70%" align="left"}

还提供了操作入门指南，帮助您开始使用 Campaign v8 Web。单击右下角的图标，选择一个可用的分步方案，然后按照说明进行操作。

![](assets/onboarding.png){width="70%" align="left"}

## 支持的浏览器 {#browsers}

Campaign v8 Web 旨在以最佳状态在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中运行。您可能无法在较旧版本或其他浏览器上使用某些功能。

## 语言偏好设置 {#language-pref}

Campaign v8 Web 目前提供以下语言版本：

<table>
<tr>
<td>
<p>英语（美国）- EN-US</p>
<p>法语 - FR</p>
<p>德语 - DE</p>
<p>意大利语 - IT</p>
</td>
<td>
<p>西班牙语 - ES</p>
<p>葡萄牙语（巴西）- PTBR</p>
<p>日语 - JP</p>
</td>
<td>
<p>朝鲜语 - KR</p>
<p>简体中文 - CHS</p>
<p>繁体中文 - CHT</p>
</td>
</tr>
</table>

默认界面语言由您在用户配置文件中指定的首选语言决定。

要更改您的语言，请执行以下操作：

1. 单击右上角的配置文件图标，然后选择&#x200B;**偏好设置**。

   ![](assets/preferences.png){width="70%" align="left"}

1. 然后单击电子邮件地址下方显示的语言。

   ![](assets/preferences2.png)

1. 选择您的首选语言并单击&#x200B;**保存**。如果您使用的组件未本地化为您的首选语言，可以选择第二语言。

   ![](assets/select-language.png)



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="规则生成器高级属性"
>abstract="使用高级属性定义您的规则。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="已发送数指标"
>abstract="投放的电子邮件数量。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="错误数指标"
>abstract="处于出错状态的电子邮件数量。"

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="测试群体"
>abstract="选择测试群体模式。"

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="预览模式"
>abstract="通过将测试群体包括在主目标中而预览和测试消息。"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="扩充数据"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="个性化"
>abstract="待定"


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="报告发送"
>abstract="请查阅营销活动报告的发送标志。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="报告跟踪"
>abstract="请查阅营销活动报告的跟踪标志。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="报告概述"
>abstract="您的投放的关键指标。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="报告目标统计数据"
>abstract="此部分根据受众显示特定指标。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="投放的汇总报告"
>abstract="选择至少两个投放以供显示汇总数据报告。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="删除重复项字段"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="删除重复项设置"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="删除重复项补充"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="维度补充"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建区段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建区段。"

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="属性选取器高级字段"
>abstract="为列配置高级字段。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="规则生成器高级字段"
>abstract="为列配置高级字段。"



>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新的隔离指标"
>abstract="新的隔离指标。"


>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="已送达"
>abstract="已投放KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="打开"
>abstract="打开KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="单击次数"
>abstract="点击次数KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="取消订阅"
>abstract="退订KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="垃圾邮件"
>abstract="垃圾邮件KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="错误"
>abstract="错误KPI"
