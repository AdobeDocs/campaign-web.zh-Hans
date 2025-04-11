---
audience: end-user
title: 从 Campaign Standard 过渡到 Adobe Campaign Web
description: 探索 Campaign Web 用户界面
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# 从 Campaign Standard 过渡至 Campaign v8 {#acs-to-ac}

Adobe Campaign Standard用户现在有资格过渡到Adobe Campaign Managed Cloud Services v8。 此过渡可提供以下几项好处：

* **强大的IT基础架构**： Managed Cloud Services v8提供了更强大的IT基础架构，确保为营销活动提供增强的性能、可靠性和可扩展性。
* **增强型支持**：托管云服务团队提供顶级协助，确保顺利过渡和持续的平台监控。 支持包括故障排除和主动维护。
* **与Adobe Experience Platform集成**： Managed Cloud Services v8与Adobe Experience Platform无缝连接，使用户能够充分利用其数据并在各个渠道之间提供个性化、有影响力的营销活动。
* **一致的用户界面和体验**：过渡到托管云服务v8不会中断工作流。 用户会继续享受熟悉的界面和体验，从而最大限度地减少团队的学习过程。

**对于正在向 Campaign v8 过渡的 Campaign Standard 用户，请[通过本文档](../../adoption/home.md)了解如何开始。**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 关键功能 {#key-features}

Campaign v8用户可以访问新的Campaign Web界面和v8控制台。 数据和设置会在环境之间同步。 所有可在客户端控制台中找到的数据和设置均显示在Campaign Web用户界面中，该用户界面可从Explorer左侧导航栏访问。 [了解详情](../get-started/user-interface.md#user-interface-explorer)

Campaign Web用户界面专为营销人员设计，以便轻松构建和编排营销活动。 Campaign v8 Web用户界面的主要功能包括：

* **现代、友好和统一的体验**。 [了解详情](../get-started/connect-to-campaign.md)。
* **新的强大功能和无缝流程**。 [了解详情](../get-started/user-interface.md)。
* **简化且直观的查询建模器**。 [了解详情](../query/query-modeler-overview.md)。
* **内置的跨渠道营销活动管理功能**。 [了解详情](../msg/gs-messages.md)。
* **重新设计了营销活动工作流活动**。 [了解详情](../workflows/gs-workflows.md)。
* **轻松创建和管理配置文件**。 [了解详情](../audience/about-recipients.md)。
* **预定义过滤器**。 [了解详情](../get-started/predefined-filters.md)。
* 用于电子邮件设计的&#x200B;**HTML转换器**。 [了解详情](../email/existing-content.md)。
* 包含选件的&#x200B;**短信**。 [了解详情](../msg/offers.md)。

Campaign客户端控制台专为管理员和开发人员而设计，用于配置和自定义其环境。 [本文档](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/new/whats-new){target="_blank"}中详细介绍了Campaign客户端控制台中可用的关键功能。

>[!NOTE]
>
>在此页面](../get-started/capability-matrix.md)中了解有关受支持和不受支持的功能以及Campaign Web用户界面与Campaign客户端控制台[之间的互操作性的更多信息。

## 术语 {#terminology}

Campaign v8 界面和 Campaign Standard 之间的大多数概念相似。但是，术语有一些差异。 示例包括：

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## 具体功能 {#new-features}

为了确保顺利过渡到Campaign v8，已在Campaign v8中添加了关键Campaign Standard功能。 [此文档](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank}中详细介绍了这些功能，这些功能仅适用于从Campaign Standard过渡的用户。

* **动态报告**：动态报告提供可自定义的实时报告以衡量营销活动的影响。 它包括访问用户档案数据以便按性别、城市和年龄等维度进行人口统计分析，以及访问功能电子邮件促销活动数据（如打开数和点击数）。 [了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html){target="_blank"}。

* **集中品牌**：Adobe Campaign允许企业定义品牌视觉和技术准则。 从徽标到技术方面（如电子邮件发件人、URL或域），用户可以向客户展示一致的品牌。 [了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)。

* **REST API**： Campaign Standard迁移的用户可以使用REST API为Adobe Campaign创建集成，并通过将Adobe Campaign与其他技术连接来构建生态系统。 [了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}。

* **登陆页面**： Campaign v8登陆页面包含多项改进，可确保与Campaign Standard的功能对等性。 通过[发行说明](../rn/release-notes.md#new-24-4)和登陆页面 [文档](../landing-pages/get-started-lp.md)了解详情。

* **可视化片段**：可视化片段是在一个或多个电子邮件投放或内容模板中引用的可重用可视化组件。 修改片段会更新使用它的所有内容。 此功能允许营销用户预构建多个自定义内容块，以便在改进的设计过程中快速汇编消息。 [了解详情](../content/use-visual-fragments.md)。

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->