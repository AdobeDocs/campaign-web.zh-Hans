---
title: 开始使用面向管理员和开发人员的Adobe Campaign v8。
description: 本教程概述了Campaign v8的主要管理和数据管理功能。 它面向从Campaign Standard迁移到Campaign v8的管理员和技术营销人员。
role: Admin, Developer
level: Beginner, Experienced
source-git-commit: 5323f3db8b29376b15b400a67765c6c0eda37479
workflow-type: tm+mt
source-wordcount: '2657'
ht-degree: 7%

---


# 管理员和开发人员快速入门 {#acs-gs-admin}

此页面概述了Campaign v8的主要管理和数据管理功能。 它适用于从Campaign Standard过渡到Campaign v8的管理员和技术营销人员。

您所做的主要更改是引入了客户端控制台，该控制台是与Adobe Campaign应用程序服务器通信的本机应用程序。

Campaign客户端控制台可集中所有功能和设置。 它与Campaign Web用户界面同步，确保两个环境的一致性。

![](assets/client_console.png){zoomable="yes"}

[了解有关Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"}客户端控制台用户界面的更多信息。

## Campaign v8架构 {#acs-gs-admi-archi}

Campaign v8（控制台）文档中详细介绍了Campaign架构。 在[此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}中了解基础知识。

供您开始使用的有用链接：

* [此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"}中介绍了Adobe Campaign组件和全局架构。

* 请参阅[Campaign架构入门](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"}，了解Campaign架构，然后再开始构建实例。

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* 事务性消息传递（消息中心）是用于管理触发消息的Campaign v8模块。 它依赖于特定体系结构模型，此模型在[此部分](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"}中有详细说明。

## Campaign客户端控制台 {#acs-gs-console}

### 安装客户端控制台 {#acs-gs-admin-console}

管理和配置任务在客户端控制台中执行。 第一步是设置环境。

Campaign客户端控制台是一个本机应用程序，它通过标准互联网协议(如SOAP和HTTP)与Adobe Campaign应用程序服务器进行通信。 Campaign客户端控制台集中了所有功能和设置，并且由于依赖本地缓存，因此需要的带宽最少。 Campaign客户端控制台专为轻松部署而设计，可从互联网浏览器部署并自动更新，无需任何特定的网络配置，因为它只生成HTTP(S)流量。

以下视频介绍如何下载和安装Adobe Campaign客户端控制台以及管理与实例的连接。

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

有关详细信息，请参阅[使用客户端控制台连接到Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect){target="_blank"}。

请注意，客户端控制台必须安装在受支持的环境中。 在[Campaign v8 （控制台）兼容性矩阵](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}中了解详情。

### 了解客户端控制台界面  {#acs-gs-ui}

通过本教程视频了解Adobe Campaign V8用户界面以及如何导航主要功能。

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

有关详细信息，请参阅[使用客户端控制台](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"}。

## 管理环境 {#acs-gs-admin-env}

安装客户端控制台后，请按照本文档中的步骤创建与应用程序服务器的连接： [与应用程序服务器文档的连接](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}。

安全实践深深地植入到我们的内部软件开发与运行流程和工具中，我们的跨职能团队严格遵循这些惯例，以预防、检测事件并快速做出响应。 请参阅[Campaign安全最佳实践](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"}以了解详情。

### 访问权限和权限 {#acs-gs-admin-rights}

Adobe Campaign允许您定义和管理分配给用户的权限。 这些权限是通过组合操作员组权限、命名权限和文件夹权限来定义的。

作为过渡到Campaign v8的Campaign Standard用户，您的权限和访问权限保持不变。 安全组已按Adobe移动到Campaign v8操作员组，并且您的每个组织单位的权限已转换为文件夹权限。 Campaign用户   使用他们的Adobe ID连接到Campaign v8，然后可以使用与Campaign Standard中相同的登录和密码。

Campaign [文件夹](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"}是客户端控制台资源管理器树中的节点。 它们根据其类型，包含特定类型的数据。 项目由Campaign v8中的文件夹具体化。 您可以创建文件夹并管理对它们的权限以限制访问。 [了解详情](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}。

请参阅[用户权限文档](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}以了解详情。


### Campaign 控制面板 {#acs-gs-admin-cp}

对于Campaign Standard，您可以使用控制面板管理环境。 请注意，对于v8，控制面板提供了其他功能。

Campaign 控制面板允许管理每个实例的设置并跟踪使用情况，从而帮助 Adobe Campaign 产品管理员提高工作效率。其直观的界面可让您轻松监控关键资产的使用情况，并执行管理任务，如将 IP 地址添加到允许列表、SFTP 存储监控、密钥管理等。

在[控制面板教程](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"}和[控制面板文档](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=zh-Hans){target="_blank"}中了解详情。

* **添加IP地址** - Campaign控制面板允许您通过将IP地址范围添加到允许列表来设置与实例的新连接。 请参阅[IP允许列表文档](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}以了解详情

* **子域配置** — 您可以配置域的子部分（技术上称为“DNS区域”）以与Adobe Campaign一起使用。
请参阅[子域委派文档](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}以了解详情

* **管理SFTP服务器** — 在控制面板中，您可以与连接到您有权访问的Campaign实例的所有SFTP服务器进行交互。 请参阅[SFTP管理文档](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}以了解详情


### 审核记录 {#acs-gs-admin-audit-trail}

如在Campaign Standard中已经可用，可以在Campaign v8中使用审核跟踪来访问实例中所做更改的完整历史记录。

在Adobe Campaign Web用户界面中，审核记录功能使用户能够完全了解对实例中的重要实体所做的所有修改，通常是对实例的顺利操作产生重大影响的修改。 请参阅[审核记录文档](../../v8/reporting/audit-trail.md)以了解详情

### 数据包 {#acs-gs-admin-audit-packages}

与Campaign Standard中可以实现的类似，管理员可以定义资源包，以通过结构化XML文件在不同的Adobe Campaign实例之间交换资源。 资源包可以是配置参数或数据。

您可以使用数据包导出和导入平台自定义设置和数据。 资源包可以包含不同类型的配置和组件，无论是否进行了过滤。 请参阅[本文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/packages){target="_blank"}以了解如何在Campaign v8中使用数据包。

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### 个性化用户界面 {#acs-gs-admin-ui}

在客户端控制台中，您可以使用多个选项来自定义用户界面，例如：

* **列表和数据显示** — 此文档提供了管理用户界面设置（如列表、单位或数据显示）的准则： [用户界面设置文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **文件夹管理** — 文件夹是Adobe Campaign中的对象，可用于组织组件和数据。 它们还用于管理权限。 了解如何[使用文件夹](../../v8/get-started/work-with-folders.md)。

* **自定义字段** — 自定义字段是通过Adobe Campaign控制台添加到现成架构的其他属性。 这些自定义字段会显示在各种屏幕中，例如用户档案或测试用户档案的详细信息。 请参阅[自定义字段配置文档](../../v8/administration/custom-fields.md)以了解详情。

## 配置品牌 {#acs-gs-admin-branding}

每家公司都有定义视觉元素和技术细节的品牌准则。 对于Adobe Campaign Standard，Adobe Campaign v8可帮助您集中管理这些准则，这样您就可以在所执行的所有操作（从电子邮件中的徽标到营销活动中使用的URL和域）中向客户展示一致的品牌形象。 作为技术管理员，您可以在Adobe Campaign中创建和管理多个品牌。

在[品牌推广文档](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}中了解详情

## 了解数据模型创建 {#acs-gs-admin-data-model-creation}

与Campaign Standard类似，Adobe Campaign v8附带其预定义的数据模型。 Adobe Campaign依赖于包含链接在一起的表的云数据库。 在[数据模型文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}中了解详情。

架构是与数据库表关联的XML文档。 它定义数据结构并描述表的SQL定义。 请参阅[架构创建文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

请在此视频中了解如何在Campaign v8中创建架构以及如何扩展现有架构：

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

与Campaign Standard中提供的功能类似，您可以创建自定义资源。 在Campaign v8中，自定义资源是自定义或扩展&#x200B;**架构**。

* 在[此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}中了解如何使用架构。

* 了解如何在[此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}中扩展现有架构。

* 了解如何在[此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}中创建新架构。

* 创建或扩展架构时，需要创建或修改关联的输入表单，以使最终用户能够看到这些更改。 利用输入表单，您可以从Adobe Campaign客户端控制台编辑与数据架构关联的实例。 该表单由其名称和命名空间进行标识。 请参阅[输入表单创建文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}。

## 工作流和数据管理 {#acs-gs-admin-data-management}

与Adobe Campaign Standard相同，Adobe Campaign v8包括一个工作流模块，允许您在应用程序服务器的不同模块之间编排所有流程和任务。 通过这个全面的图形环境，您可以设计各种流程，包括分段、活动执行、文件处理、人员参与等。 工作流引擎会执行并跟踪这些流程。 请参阅[本文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}以了解如何在Campaign v8中开始使用工作流。

请参阅下面的指向其他有用资源的链接：

* 请在此视频中了解什么是定位维度和工作表，以及Adobe Campaign如何管理不同数据源的数据：

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Campaign 可帮助您将联系人添加到云数据库。您可以加载文件、计划和自动更新多个联系人、在Web上收集数据，或直接在收件人表格中输入用户档案信息。  请参阅[导入数据（控制台）文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}以了解详情。

* 您可以轻松地将其他报表导出为PDF或CSV格式，这允许您共享、处理或打印这些报表。 请参阅[导出数据文档](../../v8/reporting/export-reports.md)以了解详情。

## REST API {#acs-gs-admin-apis}

Campaign REST API旨在通过将Adobe Campaign与您使用的技术面板连接，让您为Adobe Campaign创建集成，并构建您自己的生态系统。

作为过渡到Campaign v8的Campaign Standard用户，您可以使用REST API。

请参阅[Rest API文档](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}以了解详情。

请注意，从Campaign Standard过渡到Campaign v8时，一些建议和限制适用于REST API。 它们列在[此页面](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"}中。 在过渡到Campaign v8时，如以下可用性说明中所列，特定限制也适用：

>[!AVAILABILITY]
>
>* 现有Campaign Standard实例和已迁移的Campaign v8实例之间的PKEY值发生变化。 如果PKEY存储在外部数据库中，则实施需要进行更改，即需要调用Adobe Campaign v8主API（它提供带PKEY的pkeys/hrefs链接），后续的API调用需要通过使用先前API调用中的pkeys/hrefs来动态形成&#x200B;。
>
>* 在Campaign v8中，对于车辆链接到用户档案的同一主体，&#x200B;我们会收到一个错误firstName属性，该属性对`cusVehicle`无效，但仅具有不含链接的属性的请求主体可正常工作。`{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* 时区作为`profileAndServicesExt/profile` REST API调用的一部分显示给用户，而不是`profileAndServices/profile` REST API调用显示给用户，因为它作为数据迁移的一部分被添加到扩展架构中&#x200B;。
>
>* `ccpaOptOut`仅作为`profileAndServicesExt/profile` REST API调用的一部分显示给用户，而不作为`profileAndServices/profile` REST API调用显示给用户，因为它作为数据迁移的一部分被添加到扩展架构中。
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## 订阅服务 {#acs-gs-admin-sub}

与Campaign Standard一样，管理员可以创建订阅服务，营销人员可以向其订阅者发送消息。 关键概念和实施步骤与Campaign Standard保持一致。 您可以在下面找到有用的链接和视频。

了解如何设置和管理订阅和定位订阅者。

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* 请参阅订阅服务[Web用户界面文档](../../v8/audience/manage-subscribers.md)。

* 另请参阅文档以在[此部分](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"}中设置客户端控制台中的订阅服务。

## 消息和投放{#acs-gs-msg}

### 配置投放渠道 {#acs-gs-admin-channels}

作为Campaign Standard，Adobe Campaign v8可帮助您发送跨渠道营销活动，包括电子邮件、短信、推送通知和直邮，并使用各种专门的报告衡量其有效性。 设计消息后通过投放发送这些消息，并可为每个收件人个性化这些消息。核心功能包括定位、消息定义和个性化、通信执行和相关的运营报告。主要功能接入点是投放助手。此接入点可导向 Adobe Campaign 涵盖的多种功能。

作为管理员，您必须定义渠道配置。 请参阅下面的链接以了解详情。

* **电子邮件** - [此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"}中详细介绍了电子邮件设置。
* **短信** — 请参阅[本文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}以了解如何配置短信渠道。
* **推送通知** — 此部分](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}中详细介绍了[配置推送通知渠道的步骤。
* **事务性消息传递** — 本节中详细介绍了[在Campaign v8中配置[事务性消息传递](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"}的步骤](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### 外部帐户 {#acs-gs-ext-accounts}

作为管理员，您负责配置和管理Campaign外部帐户。 与Campaign Standard一样，技术工作流或营销策划工作流等技术流程也会使用外部帐户。

过渡到Campaign v8的过程会照顾到您现有的Campaign Standard外部帐户。

请参阅[外部帐户文档](../../v8/administration/external-account.md)以了解详情。


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### 动态内容 {#acs-gs-dyn-content}

使用 Campaign 创建动态内容并发送个性化消息。可以结合个性化功能来改进您的消息并创建自定义用户体验。

借助Campaign v8，管理员可以在以下视频中定义动态内容块以及如何使用动态内容块将电子邮件投放内容个性化：

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

有用的链接：

* [开始个性化](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [使用个性化块](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [创建条件内容](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [Personalization数据源](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### 投放模板 {#acs-gs-templates}

在Campaign v8中，需要使用投放模板，例如Campaign Standard。

为了加快并改进设计过程，请创建投放模板以轻松地在营销活动中重复使用自定义内容和设置。 此功能使您能够标准化创意外观，以便更快地执行和启动营销活动。 了解如何在[Campaign Web用户界面](../../v8/msg/delivery-template.md)中创建投放模板。 另请参阅[本节](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/create-templates){target="_blank"}中的如何在客户端控制台中创建投放模板。

### 类型规则 {#acs-gs-admin-rules}

作为管理员，您负责为投放创建和维护分类规则。 与Adobe Campaign Standard中相同，在Campaign v8中，分类规则是业务规则，允许您在发送消息之前对消息执行检查和过滤。

从Campaign Standard环境过渡到Campaign v8时，您的分类规则将移至Campaign v8。

在Campaign v8中，分类规则带有特定的活动优化附件。 此模块允许您控制、过滤和监控投放的发送。 为了避免活动之间发生冲突，Adobe Campaign 可以应用特定的限制规则来测试各种活动组合。这可确保所发送的邮件符合客户的需求与期望以及公司的通信政策。 请参阅[类型规则文档](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}以了解详情。

### 隔离管理 {#acs-gs-admin-quarantine}

所有隔离的地址和隔离规则已从Campaign Standard环境迁移到Campaign v8。 隔离管理无需执行任何特定操作。

作为管理员，从[此页面](../../v8/audience/quarantine.md)开始熟悉Campaign v8中的隔离管理。 另请参阅客户端控制台有关[此部分](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"}中隔离管理的详细文档。


## 管理Adobe Campaign集成 {#acs-gs-integrations}

您可以将Campaign实例与Adobe Experience Cloud解决方案连接以组合功能。 Adobe Campaign附带几个连接器，允许您与外部应用程序通信、连接到数据库引擎、共享和同步数据。 请参阅[本文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"}以了解如何组合解决方案。

作为迁移到Campaign v8的Campaign Standard用户，以下内容适用于您：

* 如果您将这些集成与Campaign Standard一起使用，则Adobe已迁移您的&#x200B;**Adobe Analytics**&#x200B;和&#x200B;**Audience Manager**&#x200B;配置及数据。
* 如果您的Campaign Standard环境已与&#x200B;**Adobe Experience Manager**&#x200B;集成，Adobe建议您改用&#x200B;**Adobe Experience Manager as a Cloud Service**，以便能够在Campaign Web用户界面中设计电子邮件时使用此功能，并简化直接在Adobe Experience Manager环境中管理电子邮件投放内容和表单的过程。 在[此页面](../../v8/integrations/aem-content.md)中了解详情。
请注意，Campaign还可以与Adobe Experience Manager 6.5集成。要配置此集成，请参阅[此文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}。
* 如果您的Campaign Standard环境与&#x200B;**触发器**&#x200B;集成，则必须在Campaign v8中设置并配置此集成，如[此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}中所述。
* 如果您的Campaign Standard环境与&#x200B;**Adobe Target**&#x200B;集成，则必须在Campaign v8中设置并配置此集成，如[此页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}中所述。

