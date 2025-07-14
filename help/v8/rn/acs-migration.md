---
audience: end-user
title: 从 Campaign Standard 过渡到 Adobe Campaign Web
description: 探索 Campaign Web 用户界面
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: ht
source-wordcount: '587'
ht-degree: 100%

---

# 从 Campaign Standard 过渡至 Campaign v8 {#acs-to-ac}

Adobe Campaign Standard 用户现在有资格过渡到 Adobe Campaign Managed Cloud Services v8。这一过渡可带来诸多益处：

* **强大的 IT 基础设施**：Managed Cloud Services v8 提供更加强大的 IT 基础设施，确保营销活动具有更高的性能、可靠性和可扩展性。
* **增强支持**：Managed Cloud Services 团队提供一流的协助，以确保顺利过渡以及持续的平台监控。支持包括故障排除和主动维护。
* **与 Adobe Experience Platform 集成**：Managed Cloud Services v8 可与 Adobe Experience Platform 无缝连接，使用户能够充分利用其数据，并跨渠道开展个性化、有影响力的活动。
* **一致的用户界面和体验**：过渡到 Managed Cloud Services v8 不会对工作流造成干扰。用户可以继续享受熟悉的界面和体验，从而最大程度地缩短团队的学习曲线。

**对于正在向 Campaign v8 过渡的 Campaign Standard 用户，请[通过本文档](../../adoption/home.md)了解如何开始。**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 关键功能 {#key-features}

Campaign v8 用户可以访问新的 Campaign Web 界面和 v8 控制台。数据和设置在不同环境之间同步。客户端控制台中的所有数据和设置在 Campaign Web 用户界面中均可见，可通过资源管理器左侧导航栏进行访问。[了解详情](../get-started/user-interface.md#user-interface-explorer)

Campaign 网页用户界面专为营销人员设计，可帮助他们轻松构建和安排营销活动。Campaign v8 Web 用户界面的主要功能包括：

* **现代、简便易用且统一的体验**。[了解详情](../get-started/connect-to-campaign.md)。
* **新的强大功能和无缝流程**。[了解详情](../get-started/user-interface.md)。
* **简洁直观的查询建模器**。[了解详情](../query/query-modeler-overview.md)。
* **内置跨渠道营销活动管理功能**。[了解详情](../msg/gs-messages.md)。
* **重新设计的营销活动工作流活动**。[了解详情](../workflows/gs-workflows.md)。
* **轻松创建和管理轮廓**。[了解详情](../audience/about-recipients.md)。
* **预定义过滤器**。[了解详情](../get-started/predefined-filters.md)。
* **用于电子邮件设计的 HTML 转换器**。[了解详情](../email/existing-content.md)。
* **包含产品建议的短信**。[了解详情](../msg/offers.md)。

Campaign 客户端控制台专为管理员和开发人员配置和定制其环境而设计。[本文档](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/new/whats-new){target="_blank"}详细介绍了 Campaign 客户端控制台中提供的关键功能。

>[!NOTE]
>
>要详细了解 Campaign 网页用户界面和 Campaign 客户端控制台支持和不支持的功能以及两者之间的互操作性，请参阅[此页面](../get-started/capability-matrix.md)。

## 术语 {#terminology}

Campaign v8 界面和 Campaign Standard 之间的大多数概念相似。但是，也存在一些术语上的差异。示例包括：

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

为确保顺利过渡到 Campaign v8，我们在 Campaign v8 中添加了主要的 Campaign Standard 功能。[本文档](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target=&quot;_blank}中对这些功能进行了详细说明，并且仅适用于从 Campaign Standard 过渡的用户。

* **动态报告**：动态报告提供可定制的实时报告，用以衡量营销活动所产生的影响。它包括访问轮廓数据，以便按性别、城市和年龄等维度进行人口统计分析，同时还可以访问功能性电子邮件营销活动数据，如打开次数和点击次数。[了解详情](../reporting/dynamic-reporting/get-started-reporting.md)。

* **集中化品牌管理**：Adobe Campaign 允许公司定义品牌视觉和技术指南。用户可以向客户展示一致的品牌形象，从标识到技术细节，如电子邮件发件人、URL 或域名等。[了解详情](../administration/branding/branding-gs.md)。

* **REST API**：Campaign Standard 迁移用户可以使用 REST API 为 Adobe Campaign 创建集成，并通过将 Adobe Campaign 与其他技术对接来构建生态系统。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}。

* **登陆页面**：Campaign v8 登陆页面进行了改进，以确保功能与 Campaign Standard 保持一致。通过[发行说明](../rn/release-notes.md#new-24-4)和登陆页面[文档](../landing-pages/get-started-lp.md)了解详情。

* **视觉片段**：视觉片段是可重复使用的视觉组件，可以在一封或多封电子邮件传递或内容模板中引用。修改一个片段会更新所有使用该片段的内容。此功能允许营销用户预先构建多个自定义内容块，以便在改进的设计过程中快速组装消息。[了解详情](../content/use-visual-fragments.md)。

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->