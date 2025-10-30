---
title: Adobe Campaign v8营销人员入门
description: 探索Campaign v8的主要功能。 它适用于从Campaign Standard迁移到Campaign v8的营销人员。
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 18%

---

# 营销人员入门 {#acs-gs-marketers}

本指南概述了Campaign v8的主要功能，适合从Campaign Standard过渡到Campaign v8的营销人员。

您可以通过客户端控制台或Web用户界面访问Adobe Campaign v8。 通过Web界面，您可以创建、管理和执行关键营销操作。 新的 Adobe Campaign Web 界面提供直观的现代用户体验，可简化营销活动的设计和投放。[了解详情](../../v8/get-started/user-interface.md)。

通过迁移，您从Campaign Standard中的所有数据都会在Campaign v8中导入，从而确保平稳过渡，同时对您正在进行的操作造成的中断最小。

您可以继续使用现有凭据登录并连接到新的Adobe Campaign v8实例。 登录后，您可以找到所有正在迁移的用户档案和工作流，从而继续处理营销策划。

主要区别在于用户界面。 下面是两个界面中相同工作流的比较：

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Adobe Campaign Web用户界面版本在持续交付模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 请定期查看[发行说明](../../v8/rn/release-notes.md)以了解最新更新。

## 了解Campaign Web用户界面 {#acs-gs-marketers-ui}

在下面的视频中，了解如何访问和导航Campaign Web用户界面，以及如何自定义清单列表。

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

有关更多详细信息，请参阅以下文档：

1. [了解Campaign Web用户界面](../../v8/get-started/user-interface.md)

1. [浏览和过滤列表](../../v8/get-started/list-filters.md)


## 创建和管理用户档案和受众 {#acs-gs-marketers-profiles-and-audiences}

在Campaign v8中创建和管理用户档案和受众的一般概念与Adobe Campaign Standard中的相同。 在[本节](../../v8/audience/gs-audiences-recipients.md)中了解如何开始使用用户档案和受众。

您可以在下方找到一些有用的链接，以供您开始使用。

### 管理轮廓 {#acs-gs-marketers-profiles}

在Adobe Campaign中，用户档案是存储在数据库中的记录，充当为投放创建受众并向内容添加个性化数据的关键组件。

1. 在此视频中，了解如何使用Campaign Web用户界面访问、管理和浏览用户档案：

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   请参阅[用户档案入门](../../v8/audience/about-recipients.md)文档以了解详情。

1. 了解如何在Campaign v8中[创建和管理测试用户档案](../../v8/audience/test-profiles.md)。

### 管理受众 {#acs-gs-marketers-audiences}

受众是指一组具有相似行为和/或特征的用户档案。 可生成、选择或加载这组人员。创建受众后，可将其作为您的投放的目标群体。

请在此视频中了解如何构建和管理受众、如何为投放选择受众以及定义控制组：

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

有关详细信息，请参阅[受众入门](../../v8/audience/manage-audience.md){target="_blank"}。

与Campaign Standard中一样，您可以向投放添加控制组。 您可以定义控制组以避免向部分受众发送消息，并将投放后的行为与主目标进行比较。 此选项可帮助您衡量活动的影响。
了解如何[设置控制组](../../v8/audience/control-group.md){target="_blank"}。

>[!AVAILABILITY]
>
>* 在过渡期间，通过Campaign Standard查询活动创建的所有受众都将转换为Campaign v8中的预定义过滤器。 Campaign v8还支持查询活动。
>
>* 读取受众通过[预定义过滤器](../../v8/query/build-query.md)转换为查询活动
>
>* 在受众迁移到Campaign v8后，预定义过滤器仅采用最新值。
>
>* Campaign Standard中的文件类型受众将迁移为不含维度的列表类型。

### 管理订阅 {#acs-gs-marketers-sub}

您可以管理和创建服务（如新闻稿），并检查这些服务的订阅或退订。 关键步骤与Campaign Standard中的步骤大致相同。 请在以下页面中了解详情：

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="不频繁" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>创建订阅服务</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="不频繁" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>管理订阅者<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="验证" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/send-to-subscribers"><strong>向服务的订阅者发送消息</strong></a>
</div>
<p>
</td>
</tr>
</table>

## 使用计划、项目和活动 {#acs-gs-marketers-plans}

Adobe Campaign v8允许您为营销计划和项目配置文件夹层次结构。 计划、项目和营销策划功能与Campaign Standard和Campaign v8类似。

请参阅[计划和计划文档](../../v8/administration/plans-programs.md)以了解详情。

您可以在下方找到开始使用的有用链接。 可能会影响用户体验的更改会在可用性注释中突出显示。


### 创建营销活动 {#acs-gs-marketers-campaign}

Adobe Campaign允许您使用内置的营销活动管理功能，轻松编排有针对性的营销计划。 利用定义计划的功能，您可以规划营销活动的持续时间和时间，与战略目标保持一致并最大限度地提高受众参与度。

![营销活动流](assets/campaign-flow.png)

请阅读以下文档，了解有关营销活动的更多信息：

1. [开始使用营销活动](../../v8/campaigns/gs-campaigns.md)
1. [访问和管理营销活动](../../v8/campaigns/manage-campaigns.md)
1. [创建您的第一个营销活动](../../v8/campaigns/create-campaigns.md)


### 创建工作流 {#acs-gs-marketers-wf}

Campaign Web用户界面已完全重新设计，以方便使用、配置、执行和故障排除。 正如您在Campaign Standard中使用工作流所体验的那样，您可以编排各种流程和任务，提高营销活动各个方面（从创建区段、准备消息到投放）的速度和规模。 此外，您可以通过一个易于使用的界面来使渠道同步，以进行营销活动编排。

请在此视频中了解工作流的工作方式以及如何创建定位工作流：

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

通过[工作流文档](../../v8/workflows/gs-workflows.md)获取更多详细信息。

Adobe Campaign Web用户界面在工作流中使用了查询建模器，从而简化了根据各种标准筛选数据库的过程。 [了解有关查询建模器的更多信息](../../v8/query/query-modeler-overview.md)

要了解您的工作流中每个活动的目的和功能，请浏览有关[工作流活动](../../v8/workflows/activities/about-activities.md)的详细信息

通过查看工作流的[护栏和限制](../../v8/get-started/guardrails.md)，最大限度地提高工作流的效率。

>[!AVAILABILITY]
>
>* Adobe Campaign v8中提供了工作流执行[历史记录和日志](../../v8/workflows/start-monitor-workflows.md#logs-tasks)。
>
>* 在Campaign Standard实例上执行的工作流的历史日志不会迁移到Campaign v8。
>
>* 组织单位会映射到文件夹的概念，以便映射并确保类似的访问控制。
>

## 创建和管理投放 {#acs-gs-marketers-deliveries}

借助Campaign Web用户界面，营销人员可以从左侧菜单&#x200B;**投放**&#x200B;创建独立投放，或在工作流上下文中创建投放，无论是否包含在营销活动中。 关键步骤与先前在Campaign Standard中的体验保持一致。 在以下部分中了解如何创建投放：[投放创建和管理文档](../../v8/msg/gs-deliveries.md)。

有用的链接：

* **投放模板** — 为了加快并改进设计过程，您可以创建投放模板以在营销活动中轻松重复使用自定义内容和设置。 此功能可让您标准化创意外观，以便更快地执行和启动营销活动/在[投放模板](../../v8/msg/delivery-template.md)页面中了解详情。

* **投放设置** — 投放设置是在投放模板中定义的技术投放参数。 每次投放都会使其过载。 可通过编辑投放或投放模板时提供的“设置”按钮使用这些设置。 在[投放设置](../../v8/advanced-settings/delivery-settings.md)部分了解详情。

* **动态内容** - Adobe Campaign Web动态内容功能允许您根据所收集的有关收件人的信息自定义内容。 通过使用动态内容，您可以确保营销工作更具相关性，避免推广不需要或不必要的产品或服务。在[动态内容](../../v8/personalization/gs-personalization.md)部分了解详情。

* **测试和验证** — 定义投放内容后，您可以使用用户档案和测试用户档案，在发送邮件之前预览和测试该内容。 此步骤对于确保此步骤准确且无内容和个性化设置错误至关重要。 查看[预览和测试](../../v8/preview-test/preview-test.md)。

* **正在计划** — 您可以设置发送消息的日期和确切时间。 通过选择最适合您的营销消息的时间，可尽量提高打开率。

   * 了解如何[计划独立投放](../../v8/msg/gs-deliveries.md#gs-schedule)
   * 了解如何[在工作流中计划投放](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

* **添加优惠** — 您可以在Adobe Campaign Web用户界面中将优惠添加到投放。 这些选件可从左侧选件菜单中获取，通过该菜单可访问选件列表。  了解如何[将优惠添加到您的消息](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* 处于草稿状态或已完成状态的投放已迁移。
>
>* 处于以下状态之一的投放已迁移到Adobe Campaign v8，但必须再次准备：正在传输/进行中/已取消/正在重试/准备错误。
>
>* 处于以下状态之一的投放已迁移为已取消的投放：对于已取消/正在重试。
>
>* 跟踪链接、镜像页面URL链接、订阅/退订链接的工作方式与Campaign Standard中相同。
>
>另请参阅以下部分：Adobe Campaign中的[跟踪和监控](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}、[品牌](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}。

### 电子邮件投放 {#acs-gs-marketers-email}

通过此视频了解如何从头开始创建电子邮件投放、定义受众、设计内容、模拟预览和发送校样：

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

在[创建您的第一个电子邮件文档](../../v8/email/create-email.md)中了解如何创建您的第一个定向电子邮件

在Campaign v8中，创建、测试和发送电子邮件投放的详细步骤类似于Campaign Standard。

1. **设计和定义内容**

   Campaign v8电子邮件设计工具与Campaign Standard中提供的设计工具类似。 提醒您，几年前已弃用Campaign Standard[旧版电子邮件编辑器](https://experienceleague.adobe.com/zh-hans/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}。 您应该已经过渡到Campaign电子邮件Designer ，以创建电子邮件内容并对电子邮件内容进行个性化设置。

   了解如何在电子邮件设计器中导航。请在以下视频中了解如何从头开始结构和设计电子邮件、如何个性化和测试电子邮件：

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   电子邮件设计器通过直观的拖放界面，让您能够创建引人入胜且量身定制的电子邮件。请参阅[电子邮件Designer文档](../../v8/email/get-started-email-designer.md)以了解详情

   请在此视频中了解如何通过上传HTML创建电子邮件、如何使其与Email Designer兼容以及如何将其转换为模板：

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   内容片段是可重复使用的组件，可以在一条或多条消息中引用。了解有关[内容片段](../../v8/content/fragments.md)的更多信息，以简化电子邮件投放的创建。

   为了加快并改进设计过程，您可以创建独立的模板，以轻松地在Adobe Campaign中重用自定义内容。 查看[创建电子邮件模板](../../v8/content/create-email-templates.md)

1. **预览和测试**

   在此视频中，了解如何预览电子邮件内容和个性化、发送测试投放（验证）以及检查常用桌面、移动和基于Web的客户端中的电子邮件渲染：

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **发送电子邮件并检查日志**

   定义内容、受众和计划后，便可以准备电子邮件投放。 请在以下部分中了解详情：

   * [准备并发送电子邮件](../../v8/monitor/prepare-send.md)
   * [监控投放日志](../../v8/monitor/delivery-logs.md)


### 短信投放 {#acs-gs-marketers-sms}

短信投放提供一种将短信发送到客户的移动设备的实用而又高效的方式。通过此功能，可创建基于文本的消息、使其个性化和预览基于文本的消息以进行有效的通信。

在Campaign v8中，创建、测试和发送短信投放的详细步骤类似于Campaign Standard。


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="潜在客户" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/sms/create-sms"><strong>创建短信投放</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="不频繁" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/sms/content-sms"><strong>设计短信投放<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="验证" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/sms/send-sms"><strong>预览和发送SMS投放</strong></a>
</div>
<p>
</td>
</tr></table>

### 推送通知 {#acs-gs-marketers-push}

推送通知对于联系移动应用程序用户至关重要，即使他们并未主动使用您的应用程序也是如此。它们有多种用途，如提供更新、推动特定操作和通知交易。

在Campaign v8中，创建、测试和发送推送通知投放的详细步骤类似于Campaign Standard。


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/push/create-push">
<img alt="潜在客户" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/push/create-push"><strong>创建推送投放</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/push/content-push">
<img alt="不频繁" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/push/content-push"><strong>设计推送投放<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/push/send-push">
<img alt="验证" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/msg/push/send-push"><strong>预览并发送推送投放</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8支持Android和iOS推送渠道。 要使用推送渠道过渡现有工作流和投放，请联系Adobe Campaign过渡经理。 了解有关[渠道设置](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}的更多信息。
>
>* 请注意，适用于移动设备应用程序的SDK V4几年前在Campaign Standard[中被弃用。 &#x200B;](https://experienceleague.adobe.com/zh-hans/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}您应该已经过渡到Adobe Experience Platform SDK，该版本与Campaign v8中的版本相同。
> 

### 直邮 {#acs-gs-marketers-direct-mail}

直邮是一种线下渠道，使用它可以制作文件，以批量向客户发送个性化信件，例如明信片、传单或产品样本。在创建直邮投放时，Adobe Campaign 会自动生成一个提取文件，其中包含所有的目标轮廓和选定数据，例如邮政地址和轮廓属性。

在Campaign v8中，创建、测试和发送直邮投放的详细步骤类似于Campaign Standard。


1. [创建直邮投放](../../v8/direct-mail/create-direct-mail.md)
1. [定义提取文件](../../v8/direct-mail/content-direct-mail.md)
1. [预览并发送](../../v8/direct-mail/send-direct-mail.md)

### 应用程序内渠道 {#acs-gs-marketers-in-app}

请注意，应用程序内渠道在Campaign v8中不可用。 如果您需要发送应用程序内通知，请联系您的Adobe代表。

## 创建和管理登陆页面 {#acs-gs-marketers-lp}

Adobe Campaign v8 Web用户界面重新设计了登陆页面的用户体验。 Campaign允许您创建、设计和共享登陆页面。 借助登陆页面，可将用户定向到在线表单，用户可从中更新其数据，选择启用/禁用接收通信，或订阅特定服务（如新闻稿）。

作为迁移到Campaign v8的Campaign Standard用户，您的现有登陆页面已迁移到Campaign Web用户界面。 您可以访问相同的功能范围。

请在以下部分中了解有关登陆页面的更多信息：

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="潜在客户" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/landing-pages/create-lp"><strong>创建登陆页面</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="验证" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/landing-pages/lp-content"><strong>设计登陆页面</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="验证" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/landing-pages/lp-templates"><strong>使用登陆页面模板</strong></a>
</div>
<p>
</td>
</tr></table>


## 报告 {#acs-gs-marketers-reporting}

Adobe Campaign提供一组[报告工具](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}。 作为管理员，您可以创建和配置报告以与其他Campaign用户共享。

Adobe Campaign报表工具套件提供了有关营销工作有效性的宝贵见解，从而允许您优化营销活动以发挥最大影响。 请参阅[报告文档](../../v8/reporting/gs-reports.md)以了解详情。

此外，根据Adobe Campaign Standard的体验，您可以在Campaign v8中使用动态报告来发送电子邮件。 它提供完全可自定义的实时报表以衡量营销活动的影响。 它增加了对轮廓数据的访问，除打开数和点击数等功能性电子邮件营销活动数据外，还支持按轮廓维度（如性别、城市和年龄）进行人口统计分析。在[动态报告文档](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}中了解详情

>[!AVAILABILITY]
>
>* [动态报告](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}可用于报告电子邮件投放、包含电子邮件投放的营销活动和事务型消息。 此外，还提供了按用户档案维度进行的人口统计分析。
>
> * [Adobe Campaign Web用户界面报表](../../v8/reporting/campaign-reports.md)也可用于从Adobe Campaign Standard过渡到Adobe Campaign v8的所有用户。

Adobe Campaign 提供三种不同的报告：

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="验证" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>营销活动报告</strong></a>
</div>
<p>
<div>
<p>提供有关各个投放的绩效、效果和结果的详细信息，为您提供全面的概述。</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="潜在客户" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>投放报告</strong>
</div>
<p>
<div>
<p>对每个渠道的每次投放的性能提供彻底的分析：成功率、受众参与和其他基本量度。 通过这些报告，可评估营销活动的整体有效性和影响力。</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="全局报告" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports"><strong>全局报告</strong></a>
</div>
<p>
<div>
<p>提供Campaign实例中每个渠道的流量和参与量度的综合整体摘要。 这些报告由各种小组件组成，每个小组件都提供您的营销活动或投放效果的一个独特视角。</p>
</div>
<p>
</td>
</tr>
</table>
