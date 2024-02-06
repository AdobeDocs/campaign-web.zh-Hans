---
audience: end-user
title: Campaign Web用户界面/客户端控制台功能矩阵
description: Campaign Web用户界面中支持的功能列表
hide: true
hidefromtoc: true
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: c7ced55fff91a480b58e033cc9a3d03d8f9f4115
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 8%

---

# Campaign Web用户界面/客户端控制台功能矩阵 {#capabilities-matrix}

以下功能只能从Campaign客户端控制台访问。 部分内容将在更高版本的Campaign Web用户界面中提供。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Campaign 管理 {#campaign-mgt-capabilities}

借助Campaign Web用户界面，您可以创建详细的跨渠道营销活动 [在此部分中](../campaigns/gs-campaigns.md). 在当前版本中，以下功能仅在Campaign客户端控制台中可用。 无法在Campaign Web用户界面中访问它们，但可以从以下位置查看它们： [资源管理器菜单](user-interface.md#user-interface-explorer).

使用提供的链接浏览Campaign v8（客户端控制台）文档，并了解如何使用这些功能。

* 营销日历。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* 计划和计划。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* 供应商、预算和成本管理。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* 分布式营销（中央/地方营销）。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=zh-Hans){target="_blank"}
* 营销资源管理(MRM)、目标、模拟和成本控制。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* 任务管理。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## 通信渠道 {#channels-capabilities}

借助Campaign Web用户界面，您可以创建、设计和发送电子邮件、短信和推送通知，并使用各种专用报告衡量其影响，如所详述 [在此部分中](../msg/gs-messages.md). 但是，以下渠道在此版本中不可用。

使用提供的链接浏览Campaign v8（客户端控制台）文档并了解有关这些渠道的更多信息。

* 直邮。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html){target="_blank"}
* LINE消息。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* 呼叫中心和自定义渠道。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* 通过X (Twitter)进行社交媒体营销。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html){target="_blank"}

## 登陆页面和Web应用程序 {#Webapps-capabilities}

Adobe Campaign允许您创建、设计和共享登陆页面。  在Campaign Web用户界面中了解有关登陆页面的更多信息 [在此部分中](../landing-pages/get-started-lp.md).

在Campaign Web用户界面中，登陆页面进行了彻底重新设计。 因此，在Campaign客户端控制台中，您无法编辑、更新或修改在Web界面中创建的登陆页面，反之亦然。

此外，以下类型的Web应用程序在Campaign Web用户界面中不可用。 但是，它们会在登陆页面列表中可见。 使用提供的链接浏览Campaign Classicv7文档并了解有关这些Web应用程序的更多信息。

* Web应用程序。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* Web窗体。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=zh-Hans){target="_blank"}
* 在线调查。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## 用户档案、测试用户档案和受众 {#profiles-audiences-capabilities}

您可以在Campaign客户端控制台和Campaign Web用户界面中创建、管理和更新用户档案和测试用户档案。 在一个UI中执行的所有更改在另一个UI中可见。 请注意，在新的Web用户界面中，“recipient”一词已更改为“profile”。 但是，新的Campaign Web用户界面中可能缺少某些特定的收件人设置和高级参数。

受众构成是Campaign Web用户界面随附的一项新功能。 因此，在Campaign客户端控制台中，您无法编辑、更新或修改 [使用查询建模器创建的受众](../query/query-modeler-overview.md). 在Campaign客户端控制台或Adobe Experience Platform中创建的所有受众都可以在Campaign Web用户界面中使用。

一次性导入/导出作业，如中所述 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} 在Campaign Web用户界面中不可用。 <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## 事务性消息传递 {#mc-capabilities}

在此版本的新Campaign Web用户界面中，消息中心产品包附带的事务性消息传送功能不可用。 浏览 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} 并了解关于实时消息传送功能的更多信息，例如：

* 在电子邮件、短信和推送上实时创作并执行信息
* 消息扩充和个性化
* 触发器（Adobe Analytics 购物车放弃）
* 报告和监控交易型消息

## 内容设计 {#content-capabilities}

通过Adobe Campaign Web用户界面提供的新Email Designer，您可以通过直观的拖放界面轻松创建引人入胜的单独定制电子邮件。 无论您是从头开始、导入现有内容还是利用现有模板，都可以设计和优化每封电子邮件的所有内容。 [了解详情](../email/edit-content.md)

通过这个新的用户界面，您还可以在电子邮件内容中使用Adobe Experience Manager 6.5中的资产，管理来自Adobe Experience Manager的电子邮件模板同步，以及与Adobe Experience Manager as a Cloud Service集成。

请注意，以下功能在此版本的产品中不可用。 使用提供的链接浏览Campaign v8（客户端控制台）文档，并了解有关这些功能（具有的功能）的更多信息 `*` Campaign客户端控制台也不支持)。

* 电子邮件AMP。  [请参阅Campaign Classicv7文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
* 来自公共资源的内容
* 自定义个性化块创建。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* 自定义表单中的内容（内容管理模块）。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* 来自 URL 的内容`*`
* 将 HTML 内容另存为模板`*`
* 电子邮件片段`*`
* 多变量/多语言用例`*`

## 类型规则 {#rules-capabilities}

可在Campaign Web用户界面中为投放或投放模板选择类型规则，但规则和类型规则的创建、管理和自定义仅在Campaign客户端控制台中可用。

使用提供的链接浏览Campaign v8（客户端控制台）文档并了解有关类型规则的更多信息。

* 控制规则创建。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
* 疲劳/压力规则创建。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hans){target="_blank"}
* 筛选规则创建。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* 类型规则管理。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* 营销活动模拟。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* 用于分类规则创作的Javascript编码。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## 工作流 {#wf-capabilities}

新的Campaign Web用户界面重新设计了工作流画布界面，可用于设计和管理您的流程。 关键工作流活动已在新设计中提供，其中一些活动将在未来版本中提供。 详细了解工作流功能，包括护栏和限制 [在此部分中](../workflows/gs-workflows.md)

请注意，以下功能仅在Campaign客户端控制台中可用：

* 工作流中的脚本
* ETL 活动：导出、编辑架构、数据加载、数据提取、SQL 代码

## 选件管理 {#offer-capabilities}

Adobe Campaign Web允许您使用在控制台中创建的投放选件进行发送。 **[!UICONTROL 互动]** 模块。 选件设计、资格规则和选件管理仅在Campaign客户端控制台中可用。 [了解详情](../msg/offers.md)

了解如何在中管理优惠目录  [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

## 与Adobe Experience Cloud解决方案集成 {#exc-capabilities}

新的Campaign现代UI简化了营销活动的设计和交付，并与其他Adobe解决方案(包括Adobe Experience Platform和Adobe Experience Manager)保持一致。

以下集成可从Adobe Campaign客户端控制台获得，但在此版本的Campaign Web用户界面中尚不可用。

使用提供的链接浏览Campaign v8（客户端控制台）文档并了解有关类型规则的更多信息。

* Adobe Analytics数据使用和KPI共享。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html){target="_blank"}
* 与Adobe Experience Cloud (Adobe Audience Manager)共享受众。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html){target="_blank"}
* 与Adobe Target集成。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html){target="_blank"}
* 与Adobe Experience Cloud Triggers集成。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html){target="_blank"}

## 报告 {#reporting-capabilities}

新的Campaign Web用户界面为所有渠道提供了一组新报告和KPI：投放报告、活动报告和全局报告。 了解详情 [在此部分中](../reporting/gs-reports.md)

某些功能只能从客户端控制台中使用。 浏览提供的链接以浏览 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hans){target="_blank"} 了解更多信息。

* 内置可投放性报告和收件箱呈现。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html){target="_blank"}
* 报表自定义。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html){target="_blank"}
* 描述性分析。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html){target="_blank"}
* 营销活动分析/多维数据集报表。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html){target="_blank"}
* 计划以PDF和CSV或链接形式共享报表。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html){target="_blank"}
* 将报表导出/下载为CSV或PDF文件。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/actions-on-reports.html){target="_blank"}

## 数据建模和数据摄取 {#data-capabilities}

Campaign Web用户界面未显示以下功能。 它们仅在客户端控制台中可用。

* 外部帐户
* 架构扩展
* 数据管理工作流活动：数据加载、提取（文件）、更新数据、编辑架构、导入/导出技术工作流
* 营销活动配置和与外部系统的连接

## 审批 {#approvals-capabilities}

Campaign Web用户界面未显示以下功能。 它们仅在客户端控制台中可用。

* 内容审批
* 投放审批
* 营销活动审批
* 目标审批

