---
audience: end-user
title: Campaign Web 用户界面/客户端控制台功能矩阵
description: Campaign Web 用户界面中支持的功能列表
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '2102'
ht-degree: 50%

---

# Campaign Web 和 Campaign 客户端控制台 {#capabilities-matrix}

Campaign Web用户界面中提供了重要的Campaign功能。 此界面主要供营销人员规划、发布和衡量其营销活动。 此页面](../rn/whats-new.md)上列出了所有功能[。

Campaign基于业务和数据需求以及与其他系统的连接进行平台自定义，是在Campaign客户端控制台中进行管理的。 因此，某些设置和功能只能从Campaign客户端控制台访问、创建或管理。 在稍后更新的Campaign Web用户界面中将提供其中一些组件。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## 营销活动管理 {#campaign-mgt-capabilities}

使用Campaign Web用户界面，您可以创建跨渠道营销活动，如本节](../campaigns/gs-campaigns.md)中详述[。 以下功能仅在Campaign客户端控制台中可用。 无法在Campaign Web用户界面中访问它们，但可从[Explorer菜单](user-interface.md#user-interface-explorer)看到某些内容。

使用提供的链接浏览 Campaign v8（客户端控制台）文档，并了解如何使用这些功能。

* **营销日历**。营销活动日历显示全局时间线中的所有项目、计划、营销活动和投放。 此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hans#campaign-calendar){target="_blank"}
* **项目和计划**。每个营销策划都属于属于一个项目，而该项目属于一个计划。 在Campaign Web用户界面中，所有营销策划都与默认的内置计划和项目相关联。 只能在客户端控制台中创建和管理计划与项目。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hans#work-with-plan-and-program){target="_blank"}
* **提供商、预算和成本管理**。 您可以配置在营销活动中执行的作业中涉及的服务提供商（包括成本结构），并管理每个项目和营销活动的预算。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=zh-Hans){target="_blank"}
* **分布式营销**（中央/地方营销）。Adobe Campaign提供了一个分布式营销应用程序，用于在中央实体（总部、营销部门等）和地方实体（销售点、区域机构等）之间实施合作活动。 此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=zh-Hans){target="_blank"}
* **营销资源管理** (MRM)、目标、模拟、和成本控制。Adobe Campaign提供了一个营销资源管理(MRM)应用程序，通过使用该应用程序，您可以对涉及的任务、预算和营销资源进行完整管理和实时跟踪，从而在协作模式下控制营销操作。 此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=zh-Hans){target="_blank"}
* **任务管理**。作为 MRM 应用程序的一部分，可通过营销活动仪表板创建、分配、跟踪和监控 Campaign 任务。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=zh-Hans){target="_blank"}

## 通信渠道 {#channels-capabilities}

借助Campaign Web用户界面，您可以创建、设计和发送&#x200B;**电子邮件**、**短信**、**推送通知**、**直邮**，并使用各种专用报告衡量其影响，如本节](../msg/gs-messages.md)中详述[。 但是，以下渠道目前&#x200B;**不**&#x200B;可用：应用程序内、LINE、呼叫中心/自定义渠道、通过 X (Twitter) 进行的社交媒体营销。

使用提供的链接浏览 Campaign v8（客户端控制台）文档，并了解有关这些渠道的更多信息。

* **LINE 消息传递**。LINE是一款免费即时消息、语音和视频呼叫应用程序，可在所有移动设备和个人电脑上使用。 Adobe Campaign 仅允许从客户端控制台发送 LINE 消息。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=zh-Hans){target="_blank"}
* **呼叫中心和自定义渠道**。可以在 Campaign 环境中实施呼叫中心和其他自定义渠道。这些渠道仅可在客户端控制台中使用。[请参阅 Campaign Classic v7 文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=zh-Hans#other-channels){target="_blank"}
* 通过 X (Twitter) 进行&#x200B;**社交媒体营销**。通过发布消息和发送私信来通过 X (Twitter) 与客户互动。此功能与社交营销加载项一起提供，只能从客户端控制台中使用。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=zh-Hans){target="_blank"}

## 登陆页面和 Web 应用程序 {#Webapps-capabilities}

可使用 Adobe Campaign 创建、设计和共享登陆页面。在新界面中，登录页面体验已完全重新设计。在此部分](../landing-pages/get-started-lp.md)中了解如何在Campaign Web用户界面[中创建、设计和发布登陆页面。

因此，在Campaign客户端控制台中，您无法编辑、更新或修改在Web界面中创建的登陆页面，反之亦然。 Campaign Web用户界面中没有以下类型的Web应用程序。 但是，这些应用程序会在显示登陆页面列表中。使用提供的链接浏览 Campaign Classic v7 文档并了解有关这些 Web 应用程序的更多信息：

* **Web 应用程序**。Adobe Campaign允许您创建和发布动态和交互式Web应用程序，其中预加载的数据来自数据库，内容根据所连接用户的权限进行调整。 此功能仅在客户端控制台中可用。[请参阅 Campaign Classic v7 文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=zh-Hans){target="_blank"}
* **Web 窗体**。在 Campaign Web 用户界面中可以看到在客户端控制台中设计的 Web 和登陆页面，但无法编辑或修改。客户端控制台网页设计人员和随Campaign Web用户界面提供的登陆页面设计人员之间的某些选项可能不同。 [请参阅 Campaign Classic v7 文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=zh-Hans){target="_blank"}
* **在线调查**。仅可从客户端控制台创建在线调查并收集答案。此功能在Campaign Web用户界面中不可用。 ·[请参阅 Campaign Classic v7 文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=zh-Hans){target="_blank"}

## 轮廓、测试轮廓和受众 {#profiles-audiences-capabilities}

您可以在Campaign客户端控制台和Campaign Web用户界面中创建、管理和更新用户档案和测试用户档案。 在一个界面中执行的所有更改在另一个界面中均可见。 但是，新的Campaign Web用户界面中可能缺少某些特定的收件人设置和高级参数。

请注意，在新的Web用户界面中，“收件人”一词已更改为“profile”，而“种子地址”现在是“测试用户档案”。

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

在Campaign客户端控制台或Adobe Experience Platform中创建的所有受众均可在Campaign Web用户界面中使用。

如[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=zh-Hans#import-jobs){target="_blank"}中所述，一次性导入/导出作业在Campaign Web用户界面中不可用。<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## 内容设计 {#content-capabilities}

Adobe Campaign Web 用户界面带有全新的电子邮件设计器，通过其直观的拖放界面，可轻松创建富有吸引力、个性化定制的电子邮件。无论您是从头开始、导入现有内容还是利用现有模板，都可以设计和优化每封电子邮件的所有内容。 [了解详情](../email/edit-content.md)

利用此新用户界面，您可以从Adobe Experience Manager管理电子邮件模板同步并与Adobe Experience Manager as a Cloud Service集成。

请注意，以下功能暂时在Campaign Web用户界面中不可用。 使用提供的链接浏览 Campaign v8（客户端控制台）文档并了解有关这些功能的更多信息。

* **自定义个性化块创建**。除了默认的个性化块之外，还可从客户端控制台创建自定义块。此功能在Campaign Web用户界面中不可用。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=zh-Hans#create-custom-personalization-blocks){target="_blank"}
* **来自自定义表单的内容**。使用内容管理模块，可创建和管理表单，以便在 Campaign 中创建内容时为用户提供帮助。此功能仅在客户端控制台中可用。[请参阅 Campaign Classic v7 文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=zh-Hans){target="_blank"}
* **用于电子邮件的 AMP**。通过AMP for Email格式，您可以在邮件中包含AMP组件，并通过丰富的可操作内容改善电子邮件体验。 此功能仅在客户端控制台中可用。[请参阅 Campaign Classic v7 文档以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=zh-Hans){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## 类型和类型规则 {#rules-capabilities}

分类是在准备阶段执行的一系列分类规则，以便一次性轻松地将多个筛选规则应用于投放。 借助这些工具，营销人员可以通过控制、筛选投放内容并安排投放发送优先级，从而标准化所有投放的业务实践。

可在Campaign Web用户界面中为投放或投放模板选择类型规则，如本节](../advanced-settings/delivery-settings.md#typology)中详述[。 但是，规则和类型规则的创建、管理和自定义仅在Campaign客户端控制台中可用。

使用提供的链接浏览 Campaign v8（客户端控制台）文档并了解有关类型规则的更多信息：

* 创建控制规则。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=zh-Hans){target="_blank"}
* 疲劳/压力规则创建。 [了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hans){target="_blank"}
* 创建过滤规则。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=zh-Hans){target="_blank"}
* 管理类型规则。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=zh-Hans){target="_blank"}
* 营销活动模拟。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=zh-Hans){target="_blank"}
* 用于创作类型规则的 JavaScript 编码。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hans#use-cases-on-pressure-rules){target="_blank"}

## 工作流 {#wf-capabilities}

新的 Campaign Web 用户界面提供了重新设计的工作流画布界面，可用于设计和管理您的流程。关键工作流活动已在新设计中提供，其中一些活动将在未来更新中提供。 在本节](../get-started/guardrails.md)中了解有关工作流功能（包括护栏和限制）的详细信息[。

请注意，以下功能仅在 Campaign 客户端控制台中可用：

* 工作流中的脚本
* ETL 活动：导出、编辑架构、数据加载、数据提取、SQL 代码

请参阅[此处](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=zh-Hans){target="_blank"}的 Adobe Campaign v8（控制台）工作流文档，了解有关工作流活动的更多信息。

## 产品建议管理 {#offer-capabilities}

可在通过 Adobe Campaign Web 用户界面创建的投放中发送产品建议。须在客户端控制台中使用&#x200B;**[!UICONTROL 互动]**&#x200B;模块创建这些产品建议。选件设计、资格规则和选件管理仅在Campaign客户端控制台中可用。 [了解详情](../msg/offers.md)

在 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hans){target="_blank"}中了解如何管理产品建议目录。

## 与 Adobe Experience Cloud 解决方案集成 {#exc-capabilities}

新的Campaign现代UI简化了营销活动的设计和交付，并与其他Adobe解决方案(包括Adobe Experience Platform和Adobe Experience Manager)保持一致。

以下集成可从Adobe Campaign客户端控制台中获取，但在Campaign Web用户界面中尚不可用。 使用提供的链接浏览 Campaign v8（客户端控制台）文档，并了解有关这些集成的更多信息：

* Adobe Analytics 数据使用和 KPI 共享。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=zh-Hans){target="_blank"}
* 与 Adobe Experience Cloud (Adobe Audience Manager) 共享受众。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=zh-Hans){target="_blank"}
* 与 Adobe Target 集成。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=zh-Hans){target="_blank"}
* 与 Adobe Experience Cloud 触发器集成。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=zh-Hans){target="_blank"}

## 报告 {#reporting-capabilities}

新的Campaign Web用户界面为所有渠道提供了一组新报告和KPI：投放报告、活动报告和全局报告。 可在[此小节](../reporting/gs-reports.md)中了解详情。

某些功能仅在客户端控制台中可用。浏览提供的指向[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hans){target="_blank"}的链接并了解更多信息。

* 内置可投放性报告和收件箱呈现。 [了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=zh-Hans){target="_blank"}
* 报告自定义。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=zh-Hans){target="_blank"}
* 描述性分析。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=zh-Hans){target="_blank"}
* 营销活动分析/多维数据集报表。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=zh-Hans){target="_blank"}
* 按计划以 PDF 和 CSV 或链接形式共享报告。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=zh-Hans){target="_blank"}

## 数据建模和数据摄取 {#data-capabilities}

Campaign Web 用户界面不会显示以下功能。这些仅在客户端控制台中可用：

### 外部帐户 {#external}

Adobe Campaign 提供了一组预定义的外部帐户来与外部系统连接。作为 Campaign 系统管理员，您只能创建和管理外部帐户。[了解详情](../administration/external-account.md)

### 架构创建和扩展 {#schema}

架构创建、修改和扩展都仅面向高级用户。这些功能只能从客户端控制台中使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=zh-Hans){target="_blank"}

### 工作流数据管理功能 {#data}

数据管理通过提供更高效灵活的工具（如数据加载、提取文件、更新数据、编辑架构或导入/导出技术工作流），来结合一系列活动，以解决复杂的定位问题。 [了解客户端控制台中的工作流数据管理功能](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=zh-Hans#data-management){target="_blank"}

>[!NOTE]
>
>虽然其中的某些活动仅在客户端控制台中可用，但某些活动在Campaign Web用户界面中可用，如&#x200B;**扩充**、**加载文件**、**更改数据源**&#x200B;或&#x200B;**更改维度**&#x200B;活动。 [在Campaign Web用户界面中了解有关定位和数据管理活动的更多信息](../workflows/activities/about-activities.md#targeting)

### 联合数据访问配置 {#fda}

Campaign 配置以及与外部系统的连接仅限高级用户使用，并且只能从客户端控制台中使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hans){target="_blank"}

## 审批 {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="审批管理"
>abstract="仅可从客户端控制台进行审批管理。 "

Campaign Web用户界面不会显示内容、投放、工作流、营销活动和目标的审批管理。 这些功能仅在客户端控制台中可用。

在 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=zh-Hans){target="_blank"}中了解如何管理工作流中的审批。

请参阅[Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=zh-Hans){target="_blank"}以了解如何管理营销活动中的投放、内容和目标审批。

## 权限 {#permissions-capabilities}

Campaign用户只能通过Adobe Identity Management System (IMS)使用Adobe ID访问Campaign Web用户界面。 授予用户的权限也适用于Campaign Web用户界面。

权限是在Adobe Admin Console和Adobe Campaign客户端控制台中定义的，详见本节](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=zh-Hans)中的[。 无法从Adobe Campaign Web用户界面执行任何权限操作。

## 监控 {#monitoring-capabilities}

Campaign平台监控功能仅在客户端控制台和Campaign控制面板中可用。 它们不会显示在Campaign Web用户界面中。

浏览提供的 Campaign v8（客户端控制台）文档和控制面板文档的链接，了解更多信息。

* [工作流监控](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=zh-Hans){target="_blank"}
* [工作流热图](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=zh-Hans){target="_blank"}
* [性能监控](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=zh-Hans){target="_blank"}
* [可投放性监控](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=zh-Hans){target="_blank"}