---
title: 从Campaign Standard过渡后的Adobe Campaign v8快速入门
description: 了解开始使用新的Campaign v8应用程序所需的步骤
role: User, Admin, Developer
level: Beginner
exl-id: 39d1f1b6-626b-48a2-92c3-9b593a377d66
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '1560'
ht-degree: 29%

---

# 从 Campaign Standard 到 v8 {#ac-acs}

欢迎使用Adobe Campaign v8！

作为从Campaign Standard过渡到Campaign v8的用户，本参考指南专为您而设计。 它可帮助您熟悉新的Campaign环境，并引导您完成开始使用您的角色所需的步骤。

1. 首先了解[Adobe Campaign v8](#new)的新增功能。

1. 接下来，根据您的角色](#experiences)了解Adobe Campaign Standard与Adobe Campaign v8之间的[体验差异。

## 新增功能 {#new}

在此页面中大致了解Adobe Campaign Web用户界面中的最新增强功能。 有关关键功能和版本更新功能的完整列表，请查看[此部分](../../v8/rn/whats-new.md)。

### Campaign v8的增强功能 {#ac-enhancements}

下面列出了Adobe Campaign v8随附的关键增强功能。

* **Web用户界面**

  Adobe Campaign v8提供了客户端控制台和Web用户界面，可满足不同的用户偏好和需求。 客户端控制台提供了强大的桌面应用程序体验，而Web用户界面设计为直观且可访问，使其成为熟悉Adobe Campaign Standard的营销人员的理想选择。

  Web用户界面与Adobe Campaign Standard有许多相似之处，尽管有些术语可能有所不同。

  您可以[在此处](../../v8/campaign-web-home.md)了解有关Adobe Campaign Web用户界面的更多信息。

  ![](assets/home.png){zoomable="yes"}

  所有新功能和改进均列在[发行说明](../../v8/rn/release-notes.md)中。 Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。


* **性能**

  Adobe Campaign v8利用高级云级数据库技术，从而显着提高性能和效率。 此重新设计的架构可提供几个主要优势：

   * *缩放*：系统现在支持处理能力的大幅提高，批处理吞吐量达到每小时&#x200B;**20百万次操作**。 使用这种新架构，可以管理更高的配置文件，并提供可预测的性能。
   * *速度*：系统已针对任何营销活动得到改进：事务性消息的分段、投放准备或吞吐量，现在为每小时&#x200B;**1百万**。

  完全托管的云服务为用户提供：

   * 实时数据探索：即时访问和分析数据，以实现快速见解和更明智的决策。

   * 快速构建受众：在几分钟内轻松创建目标受众，以实现更高效的活动分段。

  总体而言，Adobe Campaign v8强大的架构为以更快的速度和效率管理广泛而复杂的营销活动提供了强大的基础。

### Adobe Campaign v8的新增功能 {#ac-new-features}

作为迁移到Adobe Campaign v8的Campaign Standard用户，您现在可以使用以下功能：

* **富推送**

  Adobe Campaign v8提供发送富推送通知的功能，该功能可吸引用户的注意并鼓励他们采取行动。 这些通知可以包括各种元素，例如文本、图像、按钮、倒计时器、声音等。

  ![](../../v8/push/assets/rich_push.png){zoomable="yes"}

  为了便于创建这些丰富的通知，Adobe Campaign v8提供了各种模板，让您能够设计和自定义复杂通知的内容，例如轮盘或计时器。

  您可以根据客户的系统定制通知：

   * 对于[Android](../../v8/push/rich-push.md)模板

   * 对于[iOs](../../v8/push/rich-push.md)模板

  推送通知是吸引移动应用程序用户的重要工具，即使用户未主动使用您的应用程序，您也可以通过推送通知联系他们。

* **Adobe Experience Manager as a Cloud Service**

  Adobe Campaign v8与Adobe Experience Manager as a Cloud Service无缝集成，增强了您为客户提供个性化、内容丰富的体验的能力。 此本机集成可简化内容管理，并利用Adobe Experience Manager强大的功能来优化营销工作。

  以下是此集成启用的主要功能：

   * *资源管理*：在Adobe Campaign v8中，电子邮件设计器提供了一个用于访问和管理资源的选取器。 此功能简化了将Adobe Experience Manager中的元素集成到交付中的过程，提高了内容管理的效率。 [了解有关资产管理的更多信息](../../v8/integrations/aem-assets.md)

     ![](../../v8/integrations/assets/assets_6.png){zoomable="yes"}

   * *电子邮件模板导入*： Adobe Campaign v8允许您浏览电子邮件模板，并将其从Adobe Experience Manager直接导入Campaign。 [了解有关电子邮件模板导入的更多信息](../../v8/integrations/aem-content.md)

     ![](../../v8/integrations/assets/aem_6.png){zoomable="yes"}

  Adobe Experience Manager as a Cloud Service提供了云原生的敏捷性，使您能够加快实现价值并适应不断变化的业务需求。 此集成不仅增强了您的内容管理功能，还允许您在所有接触点上向客户提供更加个性化和引人入胜的体验。

* **AI助手 — 内容加速器**

  Campaign AI Assistant可以在电子邮件、短信和推送等渠道中创建和执行营销活动，操作直观、简单且轻松，同时还能节省时间、提高效率和产生更好的结果。

  ![](../../v8/email/assets/full-email-1.png){zoomable="yes"}

  AI Assistant彻底改变了您跨渠道创建专业且品牌一致的内容的方式。 借助高级GenAI模型并深入了解您的品牌准则，AI Assistant可根据营销目标自动生成个性化、引人入胜且有效的内容，其内容针对品牌概述的样式、布局、色调等进行了优化。

  AI Assistant使营销活动的创建和执行变得直观、简单而轻松，同时节省时间、提高效率和产生更好的结果。

  ![](../../v8/email/assets/full-email-2.png){zoomable="yes"}

  它提供电子邮件模板的变体，并生成和重新生成图像。 在[本节](../../v8/email/generative-content.md)中了解有关AI Assistant — 内容加速器的更多信息。 Adobe Campaign v8具有AI助手，可用于[电子邮件](../../v8/email/generative-content.md)、[短信](../../v8/email/generative-sms.md)和[推送](../../v8/email/generative-push.md)。

* **已升级的SMS基础架构 — SMS v2.0**

  SMS的简单性和易用性使其成为非常宝贵的通信渠道，此外，它还具有数十亿终端的无与伦比的稳定性和兼容性。

  Adobe Campaign v8附带了一个新的基础设施，用于改进短信的发送。 [了解有关新短信设置的更多信息](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}。

* **已升级的推送基础结构**

  Adobe Campaign v8正在推出我们最新的推送通知服务，该服务基于现代尖端技术构建的强大框架提供支持。 此服务旨在解锁更高级别的可扩展性，确保您的通知能够以无缝效率接触到更多受众。 通过我们增强的基础架构和优化的流程，您可以期待更高的扩展性和可靠性，使您能够以前所未有的方式吸引移动应用程序用户并与之建立联系。

  [了解有关已升级的推送基础结构的详细信息](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}。


## Managed Services {#ac-managed-services}

Adobe Campaign v8 是一款托管式云服务，提供主动监督、及时发送警报和服务治理功能。Adobe 托管式云服务以较低的总体拥有成本为营销人员提供更加灵活、安全且可扩展性更高的跨渠道营销活动管理解决方案。新产品将各种服务与主动监督和及时发送警报的功能相结合。

## v8中添加了Campaign Standard功能 {#ac-v8-added}

为了让您顺利过渡到 Campaign v8，我们在 Campaign v8 中添加了主要的 Campaign Standard 功能。[本文档](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}中有详细说明。

* **动态报告**：动态报告提供完全可定制的实时报告，用以衡量您的营销活动所产生的影响。它增加了对轮廓数据的访问权限，除了打开和点击等功能性电子邮件活动数据之外，还支持按性别、城市和年龄等轮廓维度进行人口统计分析。[了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html){target="_blank"}。

* **中央品牌化**：每个公司都具有属于自己的品牌视觉和技术准则。通过 Adobe Campaign，您可以定义从徽标到技术方面的一系列规定（如电子邮件发送者、URL 或域名），从而为客户提供一致的品牌形象。[了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest API**：作为 Campaign Standard 迁移用户，您可以使用 Rest API 为 Adobe Campaign 创建集成，并通过将 Adobe Campaign 与您使用的技术面板连接来构建自己的生态系统。[了解详情](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-hans){target="_blank"}。

* **登陆页面** - 对 Campaign v8 登陆页面进行了一些改进，以确保功能与 Campaign Standard 相同。通过[发行说明](../../v8/rn/release-notes.md#new-24-4)和登陆页面 [文档](../../v8/landing-pages/get-started-lp.md)了解详情。

* **视觉片段**  - 视觉片段是可重复使用的视觉组件，可以在一封或多封电子邮件传递或内容模板中引用。当修改片段时，使用它的每个内容都会被更新。此功能用于预构建多个自定义内容块，营销用户可以使用这些内容块在改进的设计过程中快速组装消息内容。[了解详情](../../v8//content/use-visual-fragments.md)

## Campaign Standard和Campaign v8之间的主要差异 {#experiences}

Adobe Campaign v8和Adobe Campaign Standard中的大多数概念都很相似。 但是，有一些不同之处如下所述。

### 术语更改 {#terminology-changes}

以下是Campaign Standard和Campaign v8之间的一些术语差异。

* 自定义资源是&#x200B;**架构**
* 消息被称为&#x200B;**传递**
* 产品用户是&#x200B;**操作员**
* 角色配置有&#x200B;**已命名权限**
* 安全组是&#x200B;**操作员组**
* 组织单位通过&#x200B;**文件夹权限**&#x200B;进行管理

此外，作为现有的Campaign用户，请注意，一些概念已重命名，以符合最新的术语标准。 这些更改仅适用于 Campaign Web 用户界面，并且不会反映在客户端控制台中。下面对它们进行了汇总。

* 收件人现在改为&#x200B;**轮廓**。[了解详情](../../v8/audience/gs-audiences-recipients.md)。
* 种子地址现在改为&#x200B;**测试轮廓**。[了解详情](../../v8/preview-test/test-deliveries.md)。
* 投放分析现在是&#x200B;**投放准备工作**。在需要启动消息准备时，请单击&#x200B;**准备**&#x200B;按钮。[了解详情](../../v8/monitor/prepare-send.md)。
* 现在可通过&#x200B;**模拟内容**&#x200B;按钮使用电子邮件预览。[了解详情](../../v8/preview-test/preview-test.md)
* 列表现在称为&#x200B;**受众**。[了解详情](../../v8/audience/gs-audiences-recipients.md)。

## 新用户体验

访问您的角色的相关参考指南，了解Adobe Campaign v8的新用户体验。

<table>
<tr>
  <td>
    <a href="marketers.md">
      <img alt="营销活动管理器"src="./assets/digital_marketing.jpeg"/>
    </a>
    <div>
  </td>
  <td>
  <a href="admin-developers.md">
    <img alt="管理员或开发人员" src="./assets/admin.jpeg"/>
    </a>
    <div>
  </td>
  </tr>
  <tr>
    <td>
    <a href="marketers.md">
    <strong>营销人员</strong>
    </a>
    </td>
    <td>
      <a href="admin-developers.md">
      <strong>管理员或开发人员</strong>
      </a>
    </td>
  </tr>
    <td>
    <em>营销活动经理，媒体营销专家</em>
    </td>
    <td>
      <em>系统管理员，技术营销专家</em>
    </td>
  <tr>
    <td>
    <b>主要任务/职责包括：</b>
    </td>
      <td>
    <b>主要任务/职责包括：</b>
    </td>
  </tr>
  <tr>
    <td>
      <li>创建营销活动
      <li>设计工作流
      <li>测试和执行活动
      <li>部署多渠道营销活动
      <li>优化活动
      <li>优化自动化活动
    </td>
    <td>
        <li>访问管理
        <li>系统配置
        <li>系统自定义
    </td>
</tr>
</table>
</div>

<!--
## Deprecated items

Adobe constantly evaluates product capabilities to identify older features that should be replaced with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility.

Please refer to [this documentation for information on deprecated items](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features).-->
