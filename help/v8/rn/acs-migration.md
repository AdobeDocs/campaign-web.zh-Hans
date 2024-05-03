---
audience: end-user
title: 从Campaign Standard过渡到Adobe Campaign Web
description: 了解Campaign Web用户界面
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 8cd743d7feafe9093790c3f631ffbfe19d1413e2
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 7%

---

# Campaign Standard过渡到Campaign v8{#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

欢迎使用Adobe Campaign Managed Cloud Services v8！

我们很高兴地宣布，Adobe Campaign Standard用户现在有资格过渡到Adobe Campaign Managed Cloud Services v8。 这一转变带来了许多好处：

* 强健的IT基础架构：通过托管Cloud Servicev8，客户可以利用更强健的IT基础架构，确保其促销活动的性能、可靠性和可扩展性得到增强。
* 增强的支持：我们的托管Cloud Service团队致力于提供顶级帮助，确保平稳过渡并持续监控您的平台。 从故障诊断到主动维护，我们为您提供全面的服务。
* 与Adobe Experience Platform集成：托管Cloud Servicev8与Adobe Experience Platform无缝连接，使客户能够利用其数据的全部潜力，并在各个渠道之间提供个性化、有影响力的营销活动。
* 一致的用户界面和体验：确保Rest，过渡到托管Cloud Servicev8不会中断您的工作流程。 您将继续享受熟悉的用户界面和用户体验，确保您的团队只需最少的学习曲线即可学习。

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 关键功能 {#key-features}

让我们更深入地了解Campaign v8将为您提供哪些关键功能：

* 现代、友好和统一的体验。 [了解详情](../get-started/connect-to-campaign.md)。
* 新的强大功能和无缝流程。 [了解详情](../get-started/user-interface.md)
* 新的简化且直观的查询建模器。 [了解详情](../query/query-modeler-overview.md)
* 内置的跨渠道营销活动管理功能。 [了解详情](../msg/gs-messages.md)
* 全新和重新设计的活动工作流活动。 [了解详情](../workflows/gs-workflows.md)
* 使用查询建模器定位受众。 [了解详情](../query/query-modeler-overview.md)
* 轻松创建和管理配置文件。 [了解详情](../audience/about-recipients.md)
* 预定义过滤器。 [了解详情](../get-started/predefined-filters.md)
* 用于电子邮件设计的HTML转换器。 [了解详情](../email/existing-content.md)
* 包含选件的短信。 [了解详情](../msg/offers.md)

## 控制台和Web界面 {#console}

作为Campaign v8用户，您将有权访问新的Campaign Web界面和v8控制台。 数据和设置将从一个环境同步到另一个环境。在Campaign Web用户界面中，从Explorer左侧导航栏中可以看到客户端控制台中所有可用的数据和设置。 [了解详情](../get-started/user-interface.md#user-interface-explorer)

Campaign Web用户界面和Campaign客户端控制台之间受支持和不受支持的功能以及互操作性 [本页内容](../get-started/capability-matrix.md)

## 术语 {#terminology}

Campaign Web界面和Campaign Standard中的大多数概念都很相似。 但是，两者之间有一些区别。 以下是Campaign Standard和Campaign Web界面之间术语差异的一些示例：

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* 自定义资源为 **架构** 在Campaign Web用户界面中。
* 营销活动不再存在。
* 消息为 **投放**.
* 用户是 **运算符**.
* 角色为 **已命名权限**.
* 安全组是 **操作员组**.
* 组织单位为 **文件夹权限**

## 新增功能 {#new-features}

为了让您能够进行过渡，我们添加了 [主要功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) 从Campaign Standard到v8：

* **动态报告**：动态报告提供完全可自定义的实时报告以衡量营销活动的影响。 它增加了对用户档案数据的访问权限，从而除了功能电子邮件促销活动数据（如打开数和点击数）之外，还可按用户档案维度（如性别、城市和年龄）进行人口统计分析。 [了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **集中化品牌**：每个公司都有品牌视觉化和技术准则。 使用Adobe Campaign，您可以定义从徽标到技术方面的一系列规定（如电子邮件发件人、URL或域），以便为客户提供一致的品牌。 [了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest API**  — 作为Campaign Stardard迁移的用户，您可以使用Rest API为Adobe Campaign创建集成，并通过将Adobe Campaign与您使用的技术面板连接来构建您自己的生态系统。 [了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **登陆页面**  — 为Campaign v8提供了许多改进，确保您不会丢失任何功能。 在中了解详情 [发行说明](../rn/release-notes.md#new-24-4) 和登陆页面 [文档](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->
