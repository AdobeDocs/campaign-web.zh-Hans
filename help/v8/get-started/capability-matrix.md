---
audience: end-user
title: Campaign Web 用户界面/客户端控制台功能矩阵
description: Campaign Web 用户界面中支持的功能列表
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '2134'
ht-degree: 97%

---

# Campaign Web 和 Campaign 客户端控制台 {#capabilities-matrix}

Campaign Web 用户界面中提供了关键的 Campaign 功能。此界面主要供营销人员在规划、启动和衡量其营销活动时使用。[本页](../rn/whats-new.md)中列出了所有功能。

基于业务和数据需求的 Campaign 平台自定义以及与其他系统的连接是在 Campaign 客户端控制台中管理的。因此，对于某些设置和功能，只能从 Campaign 客户端控制台进行访问、创建或管理。其他一些设置和功能将在稍后更新的 Campaign Web 用户界面中提供。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## 营销活动管理 {#campaign-mgt-capabilities}

借助 Campaign Web 用户界面，您可以创建跨渠道营销活动，如[本节](../campaigns/gs-campaigns.md)中所详述。以下功能仅在 Campaign 客户端控制台中可用。它们在 Campaign Web 用户界面中不可访问，但部分可以从[资源管理器菜单](user-interface.md#user-interface-explorer)中查看。

使用提供的链接浏览 Campaign v8（客户端控制台）文档，并了解如何使用这些功能。

* **营销日历**。营销活动日程表在全局时间线中显示所有项目、计划、营销活动和投放。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hans#campaign-calendar){target="_blank"}
* **项目和计划**。每个营销活动都属于一个项目，而项目又属于一个计划。在 Campaign Web 用户界面中，所有营销活动都与默认的内置计划和项目相关联。只能在客户端控制台中创建和管理计划与项目。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=zh-Hans#work-with-plan-and-program){target="_blank"}
* **提供商、预算和成本管理**。您可以配置在营销活动中执行的作业中涉及的服务提供商（包括成本结构），并管理每个项目和营销活动的预算。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=zh-Hans){target="_blank"}
* **分布式营销**（中央/地方营销）。Adobe Campaign 提供分布式营销应用程序，用于在中央实体（总部、营销部门等）和本地实体（销售点、区域代理等）之间实施合作型营销活动。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=zh-Hans){target="_blank"}
* **营销资源管理** (MRM)、目标、模拟、和成本控制。Adobe Campaign 提供了一个营销资源管理 (MRM) 应用程序，可全面管理和实时跟踪所涉及的任务、预算和营销资源，从而让您在协作模式下控制营销操作。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=zh-Hans){target="_blank"}
* **任务管理**。作为 MRM 应用程序的一部分，可通过营销活动仪表板创建、分配、跟踪和监控 Campaign 任务。此功能仅在客户端控制台中可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=zh-Hans){target="_blank"}

## 通信渠道 {#channels-capabilities}

借助 Campaign Web 用户界面，可创建、设计和发送&#x200B;**电子邮件**、**短信**、**推送通知**&#x200B;和&#x200B;**直邮**，并使用各种专门设计的报告衡量其影响，如[本节](../msg/gs-messages.md)中所详述。但是，以下渠道目前&#x200B;**不**&#x200B;可用：应用程序内、LINE、呼叫中心/自定义渠道、通过 X (Twitter) 进行的社交媒体营销。

使用提供的链接浏览 Campaign v8（客户端控制台）文档，并了解有关这些渠道的更多信息。

* **LINE 消息传递**。LINE 是一款免费即时消息、语音和视频通话应用程序，可在所有移动设备和 PC 上使用。Adobe Campaign 仅允许从客户端控制台发送 LINE 消息。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=zh-Hans){target="_blank"}
* **呼叫中心和自定义渠道**。可以在 Campaign 环境中实施呼叫中心和其他自定义渠道。这些渠道仅可在客户端控制台中使用。[请参阅 Campaign Classic v7 文档，以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=zh-Hans#other-channels){target="_blank"}
* 通过 X (Twitter) 进行&#x200B;**社交媒体营销**。通过发布消息和发送私信来通过 X (Twitter) 与客户互动。此功能随社交营销插件提供，仅可通过客户端控制台使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=zh-Hans){target="_blank"}

## 登陆页面和 Web 应用程序 {#Webapps-capabilities}

可使用 Adobe Campaign 创建、设计和共享登陆页面。在新界面中，登录页面体验已完全重新设计。如需了解如何在 Campaign Web 用户界面中创建、设计和发布登陆页面，请参阅[本节](../landing-pages/get-started-lp.md)。

因此，在 Campaign 客户端控制台中，无法编辑、更新或修改在 Web 界面中创建的登陆页面，反之亦然。Campaign Web 用户界面中尚未提供以下类型的 Web 应用程序。但是，这些应用程序会在显示登陆页面列表中。使用提供的链接浏览 Campaign Classic v7 文档并了解有关这些 Web 应用程序的更多信息：

* **Web 应用程序**。借助 Adobe Campaign，您可以创建和发布动态交互式 Web 应用程序，包含从数据库预加载的数据和根据已连接用户的权限调整的内容。此功能仅在客户端控制台中可用。[请参阅 Campaign Classic v7 文档，以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=zh-Hans){target="_blank"}
* **Web 窗体**。在 Campaign Web 用户界面中可以看到在客户端控制台中设计的 Web 和登陆页面，但无法编辑或修改。客户端控制台网页设计器和 Campaign Web 用户界面附带的登录页面设计器之间的某些选项可能有所不同。[请参阅 Campaign Classic v7 文档，以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=zh-Hans){target="_blank"}
* **在线调查**。仅可从客户端控制台创建在线调查并收集答案。此功能在 Campaign Web 用户界面中不可用。[请参阅 Campaign Classic v7 文档，以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=zh-Hans){target="_blank"}

## 轮廓、测试轮廓和受众 {#profiles-audiences-capabilities}

您可以在 Campaign 客户端控制台和 Campaign Web 用户界面中创建、管理及更新轮廓和测试轮廓。在一个界面中执行的所有更改都会在另一个界面中显示。但是，新的 Campaign Web 用户界面中可能会缺少某些特定的收件人设置和高级参数。

请注意，在新的 Web 用户界面中，“收件人”一词已更改为“轮廓”，而“种子地址”现在改为“测试轮廓”。

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

在 Campaign Web 用户界面中，可以访问在 Campaign 客户端控制台或 Adobe Experience Platform 中创建的所有受众。

在 Campaign Web 用户界面中，无法访问 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=zh-Hans#import-jobs){target="_blank"}中所述的一次性导入/导出作业。<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## 内容设计 {#content-capabilities}

Adobe Campaign Web 用户界面带有全新的电子邮件设计器，通过其直观的拖放界面，可轻松创建富有吸引力、个性化定制的电子邮件。无论是从头开始、导入现有内容还是利用现有模板，均可设计并细化每封电子邮件的所有内容。[了解详情](../email/edit-content.md)

通过此全新用户界面，可从 Adobe Experience Manager 管理电子邮件模板同步，并与 Adobe Experience Manager as a Cloud Service 集成。

请注意，Campaign Web 用户界面暂不提供以下功能。使用提供的链接浏览 Campaign v8（客户端控制台）文档并了解有关这些功能的更多信息。

* **自定义个性化块创建**。除了默认的个性化块之外，还可从客户端控制台创建自定义块。此功能在 Campaign Web 用户界面中不可用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=zh-Hans#create-custom-personalization-blocks){target="_blank"}
* **来自自定义表单的内容**。使用内容管理模块，可创建和管理表单，以便在 Campaign 中创建内容时为用户提供帮助。此功能仅在客户端控制台中可用。[请参阅 Campaign Classic v7 文档，以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=zh-Hans){target="_blank"}
* **用于电子邮件的 AMP**。电子邮件 AMP 格式允许您在邮件中包含 AMP 组件，并通过丰富且可操作的内容提升电子邮件体验。此功能仅在客户端控制台中可用。[请参阅 Campaign Classic v7 文档，以了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=zh-Hans){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## 类型和类型规则 {#rules-capabilities}

类型是在准备阶段执行的一系列类型规则，以便一次性对投放内容轻松应用多个过滤规则。它们允许营销人员通过控制、过滤投放并安排其发送优先级，实现所有投放的业务实践标准化。

可在 Campaign Web 用户界面中为投放或投放模板选择类型规则，具体请参阅[本节](../advanced-settings/delivery-settings.md#typology)。但是，仅可在 Campaign 客户端控制台中创建、管理和自定义规则和类型规则。

使用提供的链接浏览 Campaign v8（客户端控制台）文档并了解有关类型规则的更多信息：

<!--
* Control rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
-->
* 创建疲劳/压力规则。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}
<!--
* Filtering rules creation. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Typology rules management. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
-->
* 营销活动模拟。[了解详情](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
<!--
* JavaScript coding for typology rules authoring. [Learn more](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}
-->

## 工作流 {#wf-capabilities}

新的 Campaign Web 用户界面提供了重新设计的工作流画布界面，可用于设计和管理您的流程。新设计中已经提供了关键的工作流活动，而某些活动将在未来更新中提供。如需详细了解工作流功能（包括护栏和限制），请参阅[本节](../get-started/guardrails.md)。

请注意，以下功能仅在 Campaign 客户端控制台中可用：

<!--
* Scripting in workflows
-->

* ETL 活动：导出、编辑架构、数据加载、数据提取、SQL 代码

请参阅[此处](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=zh-Hans){target="_blank"}的 Adobe Campaign v8（控制台）工作流文档，了解有关工作流活动的更多信息。

## 产品建议管理 {#offer-capabilities}

可在通过 Adobe Campaign Web 用户界面创建的投放中发送产品建议。须在客户端控制台中使用&#x200B;**[!UICONTROL 互动]**&#x200B;模块创建这些产品建议。产品建议设计、资格规则和产品建议管理仅在 Campaign 客户端控制台中可用。[了解详情](../msg/offers.md)

在 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hans){target="_blank"}中了解如何管理产品建议目录。

## 与 Adobe Experience Cloud 解决方案集成 {#exc-capabilities}

这一全新的、现代化的 Campaign UI 简化了营销活动的设计和投放，并实现了与其他 Adobe 解决方案（包括 Adobe Experience Platform 和 Adobe Experience Manager）的一致性。

以下集成功能可在 Campaign 客户端控制台中使用，但在 Campaign Web 用户界面中还无法使用。使用提供的链接浏览 Campaign v8（客户端控制台）文档，并了解有关这些集成的更多信息：

* Adobe Analytics 数据使用和 KPI 共享。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=zh-Hans){target="_blank"}
* 与 Adobe Experience Cloud (Adobe Audience Manager) 共享受众。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=zh-Hans){target="_blank"}
* 与 Adobe Target 集成。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=zh-Hans){target="_blank"}
* 与 Adobe Experience Cloud 触发器集成。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=zh-Hans){target="_blank"}

## 报告 {#reporting-capabilities}

全新 Campaign Web 用户界面提供了一组新报告和 KPI，适用于所有渠道：投放报告、营销活动报告和全局报告。可在[此小节](../reporting/gs-reports.md)中了解详情。

某些功能仅在客户端控制台中可用。浏览提供的链接，访问 [Campaign v8（客户端控制台）](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hans){target="_blank"}文档，了解更多信息。

* 内置可投放性报告和收件箱呈现功能。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=zh-Hans){target="_blank"}
* 报告自定义设置。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=zh-Hans){target="_blank"}
* 描述性分析。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=zh-Hans){target="_blank"}
* 营销活动分析/多维数据集报告。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=zh-Hans){target="_blank"}
* 按计划以 PDF 和 CSV 或链接形式共享报告。[了解详情](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=zh-Hans){target="_blank"}

## 数据建模和数据摄取 {#data-capabilities}

Campaign Web 用户界面不会显示以下功能。这些仅在客户端控制台中可用：

### 外部帐户 {#external}

Adobe Campaign 提供了一组预定义的外部帐户来与外部系统连接。作为 Campaign 系统管理员，您只能创建和管理外部帐户。[了解详情](../administration/external-account.md)

### 架构创建和扩展 {#schema}

架构创建、修改和扩展都仅面向高级用户。这些功能只能从客户端控制台中使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=zh-Hans){target="_blank"}

### 工作流数据管理功能 {#data}

数据管理通过提供更高效灵活的工具（如数据加载、提取文件、更新数据、编辑架构或导入/导出技术工作流），来结合一系列活动，以解决复杂的定位问题。[了解客户端控制台中的工作流数据管理功能](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=zh-Hans#data-management){target="_blank"}

>[!NOTE]
>
>虽然其中的某些活动仅在客户端控制台中可用，但在 Campaign Web 用户界面中也可进行部分活动，例如&#x200B;**扩充**、**加载文件**、**更改数据源**&#x200B;或&#x200B;**更改维度**&#x200B;活动。[了解关于 Campaign Web 用户界面中的目标市场选择和数据管理活动的更多信息](../workflows/activities/about-activities.md#targeting)

### 联合数据访问配置 {#fda}

Campaign 配置以及与外部系统的连接仅限高级用户使用，并且只能从客户端控制台中使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hans){target="_blank"}

## 审批 {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="审批管理"
>abstract="仅可从客户端控制台进行审批管理。 "

Campaign Web 用户界面不会显示内容、投放、工作流、营销活动和目标的审批管理。这些功能仅在客户端控制台中可用。

通过 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=zh-Hans){target="_blank"}了解如何管理工作流中的审批。

通过 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=zh-Hans){target="_blank"}了解如何管理营销活动中的投放、内容和目标审批。

## 权限 {#permissions-capabilities}

Campaign 用户只能通过 Adobe Identity Management System (IMS) 使用 Adobe ID 访问 Campaign Web 用户界面。授予用户的权限也适用于 Campaign Web 用户界面。

权限是在 Adobe Admin Console 和 Adobe Campaign 客户端控制台中定义的，详情请参阅[本节](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=zh-Hans)。无法从 Adobe Campaign Web 用户界面对权限执行任何操作。

## 监控 {#monitoring-capabilities}

Campaign 平台监控功能仅在客户端控制台和 Campaign 控制面板中可用。它们不会显示在 Campaign Web 用户界面中。

浏览提供的 Campaign v8（客户端控制台）文档和控制面板文档的链接，了解更多信息。

* [工作流监测](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=zh-Hans){target="_blank"}
* [工作流热图](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=zh-Hans){target="_blank"}
* [性能监控](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=zh-Hans){target="_blank"}
* [投放能力监控](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=zh-Hans){target="_blank"}

## 时区管理 {#timezone-management}

Adobe Campaign Web UI基于用户Web浏览器&#x200B;**的**&#x200B;本地时区显示所有日期和时间值。 此行为可能会导致在Web UI和客户端控制台之间比较时间戳时出现差异。

请参阅此[页面](../administration/timezone-management.md)，了解有关&#x200B;**Web UI**、**客户端控制台**&#x200B;和&#x200B;**工作流执行**&#x200B;时区之间差异的更多信息。
