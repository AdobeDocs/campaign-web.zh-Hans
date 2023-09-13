---
audience: end-user
title: Campaign Web v8 新增功能
description: 发现 Campaign Web v8 附带的新功能
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Beta"
source-git-commit: 371055202d9d3e2f4ded9fe4d3c43acd9498728e
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 76%

---


# 新增功能 {#new}


我们很高兴地介绍Adobe Campaign Web UI的BETA版。 我们的最新版本包含直观的功能，旨在简化个性化跨渠道营销活动的创建，加快获得卓越的成果，并使您获得跨所有渠道的竞争优势。

## Beta 版{#beta-release}

这个新的 Campaign Web 界面目前仅适用于 **Beta 从业人员**，并具有以下功能：

**现代、直观且统一的体验**

Campaign 的新 Web UI 提供了新的用户体验，并与所有 Adobe Experience Cloud 解决方案和应用程序保持一致。它提供：

* 通过单一用户会话和共享用户会话来访问新界面和其他 Adobe 解决方案的能力
* 新的导航体验，可从左边栏访问所有菜单和文件夹
* 顶栏中的解决方案和组织切换器
* Unified Shell 集成，可直接访问社区、帮助中心和支持

**新的强大功能和无缝流程**

* 工作流画布界面经过重新设计，用于设计和管理您的流程
* 动态内容，用于向您的受众提供高度针对性和个性化的体验
* 与 Adobe Experience Platform 受众的原生集成
* 工作流、投放、营销活动和内容的模板管理

在[此页面](../get-started/user-interface.md)中详细了解新 UI。

**创建、启动和衡量营销活动**

利用新的 Campaign Web UI，可以：

* 使用电子邮件设计器设计个性化的电子邮件内容 - [了解详情](../content/edit-content.md)
* 发送跨渠道营销活动，包括短信和推送通知。
* 使用规则生成器定义目标受众 - [了解详情](../audience/about-audiences.md)
* 预览、测试和发送电子邮件 - [了解详情](../monitor/prepare-send.md)
* 使用内置报告监控发送和衡量结果 - [了解详情](../reporting/delivery-reports.md)


## 最近更新

**测试版摘要**

* 为受众和个性化启用数据组合（联合）
* 利用AI技术增强电子邮件内容的生成
* 无缝地同步资源和完整的HTML模板
* 高效地组织和管理您的文件夹和资源
* 访问其他活动，如更改维度、重复数据删除和定期投放，以增强活动工作流

**关键的新功能**

* 更多营销活动工作流活动

  使用我们扩展的工作流活动集强化您的营销活动。 发掘新的自动化和优化的可能性，并让您创建更加动态和个性化的客户历程。

  从高级分段到条件触发器，我们的附加工作流活动可让您投放有针对性的消息并增强营销活动效果。

* 针对电子邮件内容的Gen AI

  告别手动内容创建，向高效的、数据驱动的营销活动拜拜Gen AI的强大功能所赐。  我们的生成式 AI 技术采用高级算法来生成极具吸引力的个性化内容。利用生成式 AI 的智能内容生成功能提高打开率、点进率和转化率。

  利用生成式 AI 生成电子邮件内容，保持竞争优势并提升电子邮件营销水平。


* 预定义过滤器管理

  正在引入预定义过滤器管理。 Campaign Web UI现在为您提供用户友好的界面，可轻松管理和自定义预定义过滤器以满足您的特定需求。 创建一次并保存以供将来使用。[了解详情](../personalization/predefined-filters.md)


* 目标受众

  确立投放目标从未如此简单！利用我们最新的规则生成器，您现在可以为收件人或数据库中的任何其他定位维度定义筛选条件。此外，您可以利用AEP (Adobe Experience Platform)受众来进一步优化目标受众，并最大化营销活动的影响。

* 包含短信和推送的优惠

  除了电子邮件之外，新的Web UI现在还允许您将优惠与短信和推送通知集成。 通过移动设备上联系受众，提供促销和及时通知。

  通过在我们的高级Web平台上通过短信和推送通知来利用集成优惠的强大功能，提升您的营销工作。

<!--
* Adobe Experience Manager (AEM) Integration
    
    With our AEM integration extended to web UI, you can easily manage assets and synchronize full HTML templates, empowering you to create captivating digital experiences without any hassle. 
    
    Elevate and streamline your content management capabilities on the web UI with this integration to boost productivity.
-->


## 过渡到 Campaign Web UI

作为 Campaign 用户，您仍可以访问客户端控制台来生成和管理 Campaign 资源和组件。数据和设置将从一个环境同步到另一个环境。在[此章节](../get-started/get-started.md#about-campaign-client-consoleac-client)中了解更多信息。

此外，可以在 Campaign Web UI 中查看您在客户端控制台中可用的所有数据和设置（从探索工具的左侧导航中）。在[此章节](../get-started/user-interface.md#explorer-user-interface-explorer)中详细了解探索工具视图。

随着 Campaign Web Beta 版的发布，用户界面反映了用户的权限。可在[此页面](../get-started/permissions.md)中详细了解权限

## 术语更新 {#terminology-updates}

作为现有 Campaign 用户，请注意，已对一些概念进行重命名以符合最新的术语标准。这些更改仅适用于 Campaign Web UI，并且不会反映在客户端控制台中。下面对它们进行了汇总。

* 验证现在是&#x200B;**测试电子邮件**：要发送验证，请使用电子邮件投放 UI 中的&#x200B;**测试**&#x200B;按钮。校样的目标现在称为&#x200B;**测试配置文件**。[了解详情](../preview-test/test-deliveries.md)。
* 种子地址现在用作&#x200B;**测试配置文件**：将测试电子邮件发送到种子地址，这些地址是数据库中额外的收件人。[了解详情](../preview-test/test-deliveries.md)。
* 投放分析现在是&#x200B;**投放准备**。在需要启动分析时，请单击&#x200B;**准备**&#x200B;按钮。[了解详情](../monitor/prepare-send.md)。
* 现在可通过&#x200B;**模拟内容**&#x200B;按钮使用电子邮件预览。[了解详情](../preview-test/preview-test.md)
* 列表现在称为&#x200B;**受众**。[了解详情](../audience/about-audiences.md)。

## 限制{#limitations-alpha}

以下限制适用于此 Alpha 版本：

* 可编辑的对象为：投放、营销活动、工作流、受众、订阅服务、预定义过滤器和模板。其他对象是只读的。使用筛选器来浏览所有对象。
* 无法保存受众用于将来使用。
* 管理用户界面不可用。
* 报告量度（例如，打开次数和跟踪数据）每小时更新一次。
* 投放仪表板 KPI 每 5 分钟更新一次。- 但投放准备是实时的。
* 顶栏中可用的 Adobe Experience Cloud 通知和统一帮助尚未集成。

