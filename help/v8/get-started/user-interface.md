---
audience: end-user
title: 了解界面
description: Campaign v8 Web用户界面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 050d97695dd2012644af4a35eca3e6cd9f5f02af
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 2%

---

# 了解界面 {#user-interface}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="了解界面"
>abstract="新的Campaign v8 Web界面提供了集成、直观且一致的用户体验。"

新的Campaign v8 Web界面提供了现代且直观的用户体验，以简化营销活动的设计和交付。 此新界面已与Adobe Experience Platform集成。

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>此文档经常更新以反映产品用户界面中的最新更改。 但是，某些屏幕截图可能与您的用户界面略有不同。


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## 左侧导航菜单

浏览左侧的链接以访问Campaign v8 Web功能。 多个链接显示可排序和过滤的对象列表。 您还可以配置列以显示所需的所有信息。 请参阅 [部分](#list-screens). 除电子邮件投放列表之外，所有列表屏幕均为只读。 Alpha中不提供单击任何用于编辑/查看的列表项。 所有列表都将在将来的版本中可编辑。 左侧导航菜单中显示的项目取决于您的用户权限。

![](assets/home.png)

### 主页

此屏幕包括快速访问Campaign v8 Web主要功能的关键链接和资源。 的 **收件人** 列表提供了最近创建和修改的投放的快捷方式。 此列表显示了其创建和修改日期及状态。

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

从主页的下部访问Campaign v8 Web键帮助页面。

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### 资源管理器

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="资源管理器"
>abstract="的 **资源管理器** 菜单显示与客户端控制台中文件夹层次结构相同的文件夹层次结构。 浏览所有Campaign v8组件、文件夹和架构。 除电子邮件投放列表之外，所有列表屏幕均为只读。"

的 **资源管理器** 菜单显示与客户端控制台中文件夹层次结构相同的文件夹层次结构。 浏览所有Campaign v8组件、文件夹和架构。 除电子邮件投放列表之外，所有列表屏幕均为只读。

资源管理器中显示的项目取决于您的用户权限。

与在任何列表屏幕中一样，您可以配置列以个性化显示，以查看所需的所有信息。 请参阅 [部分](#list-screens).

有关Campaign资源管理器的详细信息，请参阅此 [文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign 管理

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="活动"
>abstract="这是您的营销活动列表。 您可以查看有用信息，如开始/结束/上次修改日期及其状态。 您可以按状态或开始/结束日期过滤列表。 营销活动模板也可用。 这些列表是只读的。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="投放"
>abstract="浏览投放列表。 您可以查看其状态、上次修改日期以及关键KPI。 您可以按状态、联系日期或渠道过滤列表。 单击电子邮件投放以打开其仪表板。 其他项目为只读。 投放模板也可用。"

* **促销活动**  — 这是营销活动列表。 默认情况下，您可以查看其开始/结束/上次修改日期及其状态。 您可以按状态或开始/结束日期过滤列表。 营销活动模板也可用。 这些列表是只读的。

* **投放**  — 浏览投放列表。 默认情况下，您可以查看其状态、上次修改日期以及关键KPI。 您可以按状态、联系日期或渠道过滤列表。 单击电子邮件投放以打开其仪表板，以获取投放详细信息的概述。 其他渠道上的投放为只读。 投放模板也以只读模式提供。 您可以使用客户端控制台来编辑它们。 请参阅 [文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   使用 **更多操作** 按钮以删除或复制投放。

   ![](assets/more-actions.png){width="70%" align="left"}

### 客户管理

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="收件人"
>abstract="访问收件人数据库。 您可以查看有用信息，如其电子邮件地址、名字和姓氏。 此列表为只读。"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="受众"
>abstract="这是您的受众列表。 您可以查看其类型、来源、创建/上次修改日期和标签。 您可以按来源筛选列表。 此列表为只读。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="订阅列表"
>abstract="浏览订阅列表。 您可以查看其类型、模式和标签。 此列表为只读。"

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="定位工作流"
>abstract="访问Campaign工作流的列表。 您可以查看其状态、上次/下次处理日期和环境。 您可以按状态、上次处理日期和工作流类型过滤列表。 工作流模板也可用。 这些列表是只读的。"

* **收件人**  — 访问收件人数据库。 默认情况下，您可以查看其电子邮件地址、名字和姓氏。 此列表为只读。
* **受众**  — 这是您的受众列表。 默认情况下，您可以查看其类型、来源、创建/上次修改日期和标签。 您可以按来源筛选列表。 此列表为只读。
* **订阅列表**  — 浏览订阅列表。 默认情况下，您可以查看其类型、模式和标签。 此列表为只读。
* **定位工作流**  — 访问Campaign工作流的列表。 默认情况下，您可以查看其状态、上次/下次处理日期和环境。 您可以按状态、上次处理日期和工作流类型过滤列表。 工作流模板也可用。 这些列表是只读的。

### 决策管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="优惠"
>abstract="浏览您的互动选件列表。 默认情况下，您可以查看其状态、开始/结束日期和环境。 您可以按州和开始/结束日期过滤列表。 还提供了选件模板。 这些列表是只读的。"

* **选件**  — 浏览您的互动选件列表。 默认情况下，您可以查看其状态、开始/结束日期和环境。 您可以按州和开始/结束日期过滤列表。 还提供了选件模板。 这些列表是只读的。

## 顶部栏

通过界面的顶栏，您可以：

* 作为Alpha测试器分享您的反馈
* 在组织和实例之间切换
* 在Adobe Experience Cloud应用程序之间切换
* 访问帮助页面、联系支持人员和分享反馈。 您可以从搜索字段搜索帮助文章和视频。

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## 配置列表屏幕 {#list-screens}

例如，左侧导航菜单中的几个链接 **投放** 或 **促销活动**，显示对象列表。 这些列表屏幕是只读的，但电子邮件投放列表除外。

要更快查找项目，您可以使用搜索栏或根据上下文条件筛选列表。

![](assets/filter.png){width="70%" align="left"}

列表以列显示。 您可以通过更改列配置来显示其他信息。 为此，请单击列表右上角的图标。 您可以添加或删除列，并更改列的显示顺序。

![](assets/columns.png){width="70%" align="left"}

您可以通过单击任何列标题对列表中的项目进行排序。 将显示一个箭头（向上或向下），指示列表在该列上排序。 对于数值列或日期列，向上箭头表示列表按升序排序，而向下箭头表示降序。 对于字符串或字母数字列，值按字母顺序列出。

## 情景帮助和入门指南

界面中提供了上下文帮助。 如果可用，请单击 **?** 图标以显示帮助信息和相关文档链接。

![](assets/context-help.png){width="70%" align="left"}

此外，还提供入门指南，帮助您开始使用Campaign v8 Web。 单击右下角的图标，选择可用的分步方案之一，然后按照说明操作即可。

![](assets/onboarding.png){width="70%" align="left"}

## 支持的浏览器 {#browsers}

Campaign v8 Web在最新版本的Google Chrome、Safari和Microsoft Edge中可发挥最佳作用。 在较旧版本或其他浏览器上使用某些功能时，您可能会遇到问题。

## 语言首选项 {#language-pref}

Campaign v8 Web目前提供以下语言版本：

<table>
<tr>
<td>
<p>英语（美国） — 英语</p>
<p>法语 — FR</p>
<p>德语 — DE</p>
<p>意大利语 — IT</p>
</td>
<td>
<p>西班牙语 — ES</p>
<p>葡萄牙语（巴西） — PTBR</p>
<p>日语 — JP</p>
</td>
<td>
<p>朝鲜语 — KR</p>
<p>简体中文 — CHS</p>
<p>繁体中文 — CHT</p>
</td>
</tr>
</table>

您的默认界面语言由用户配置文件中指定的首选语言决定。

要更改语言，请执行以下操作：

1. 单击右上方的配置文件图标，然后选择 **首选项**.

   ![](assets/preferences.png){width="70%" align="left"}

1. 然后，单击电子邮件地址下显示的语言。

   ![](assets/preferences2.png)

1. 选择首选语言并单击 **保存**. 如果您使用的组件未以第一种语言本地化，则可以选择第二种语言。

   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
-->

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="短信报告摘要"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="推送报表摘要"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_import_from_a_file"
>title="从文件导入受众"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_import_from_a_file_formatting"
>title="格式设置"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_import_from_a_file_columns"
>title="列设置"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="推送通知模板"
>abstract="待定"
