---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 385c931c9fae7386c2a2f1ef471a9cd7c4a47696
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 90%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

## 6月发行说明 {#24-6-release}

**发行日期**：2024年6月18日至19日

从6月版开始，所有用户都可以使用以下功能和改进。
<!--
### Visual fragments {#24-6-1}

You can now author, use, and manage **visual** fragments to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process.

### Seed lists {#24-6-2}

A seed list, aka. **Trap group**, is a list of seed addresses. It is used to include specific addresses in your deliveries, and then target profiles who do not match the defined target criteria. This way, recipients who are out of the delivery audience can receive the delivery, as any other target recipient would. You can use seed addresses when sending proofs, or to protect your mailing list.-->

### 投放提醒 {#24-6-3}

投放警报功能是一个警报管理系统，利用该系统可让一组用户自动接收包含其投放执行信息的通知。 [了解更多信息](../msg/delivery-alerting.md)

### 计划和计划 {#24-6-4}

您现在可以创建计划和项目来组织营销策划。 通过定义文件夹层次结构，您可以将营销活动组织到项目中，并将项目组织到项目中。 [了解更多信息](../administration/plans-programs.md)

### 改进 {#improvements-24-6}

* **扩充活动中的协调**：扩充活动现在可用于将来自Campaign数据库架构的数据与来自其他架构的数据进行协调，或与来自临时架构的数据（例如使用加载文件活动上载的数据）进行协调。 例如，您可以使用此选项将用户档案在上传文件中指定的国家/地区与Campaign数据库的专用表中可用的国家/地区之一进行协调。 [了解更多信息](../workflows/activities/enrichment.md)

## 5 月发行说明 {#24-5-release}

**发行日期**：2024 年 5 月 21 日

自 5 月版本开始，所有用户都可以使用以下功能和改进。

### 审核记录  {#24-5-1}

新的&#x200B;**审核记录**&#x200B;功能按时间顺序详细记录了对 Adobe Campaign 实例进行的所有操作和事件。它提供了一种追踪对 Campaign 数据进行的所有更改的简便方法，可解决诸如以下查询：工作流的状态、最近修改工作流的个人或实例内用户执行的活动。[了解更多信息](../reporting/audit-trail.md)

### 自定义字段 {#24-5-2}

**自定义字段**&#x200B;是通过 Adobe Campaign 控制台添加到现成架构的附加属性。在 Campaign Web 用户界面中，这些自定义字段现在可在各个屏幕中看到，例如配置文件或测试配置文件的详细信息。在 Web 用户界面中，您无法创建自定义字段，但现在您可以修改它们的显示方式。[了解更多信息](../administration/custom-fields.md)

### 在表之间创建链接 {#24-5-3}

您现在可以在&#x200B;**扩充**&#x200B;工作流活动中创建与另一个表的链接。使用活动参数中的新&#x200B;**链接定义**&#x200B;部分在工作表数据和 Adobe Campaign 数据库之间创建链接。例如，如果您从包含收件人的帐号、国家/地区和电子邮件的文件中加载数据，则您现在可以创建指向该国家/地区表的链接，以便在其配置文件中更新此信息。[了解更多信息](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### 一般改进 {#improvements-24-5}

* **直邮**：您现在可以利用表达式编辑器来选择要在直邮提取文件中显示的属性。[了解更多信息](../direct-mail/content-direct-mail.md)

* **文件夹管理**：您现在可以创建与父文件夹不同类型的子文件夹。[了解更多信息](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

* **全球化**：作为我们持续努力提供统一用户体验的一部分，我们统一了 Adobe Experience Cloud 产品和应用程序中使用的术语。这会影响德语术语“Titel”，当它与对象名称相关时会更改为“Label”。这些变化将会在 UI 和文档中逐步推出。


## 4 月发行说明 {#april-24-4-release}

**发行日期**：2024 年 5 月 2 日

### 新增功能 {#new-24-4}

自 4 月版本开始，所有用户都可以使用以下功能。

**新工作流活动**

* **更新数据**：使用此活动可以对数据库中的字段执行大规模更新。您可以利用多个选项，以个性化方式更新数据。[了解更多信息](../workflows/activities/update-data.md)
* **订阅服务**：使用此活动可在单个操作中向服务订阅或取消订阅多个配置文件。[了解更多信息](../workflows/activities/subscription-services.md)
* **提取文件**：使用此活动可以将 Adobe Campaign 中的数据作为外部文件导出到另一个系统。[了解更多信息](../workflows/activities/extract-file.md)
* **传输文件**：使用此活动可以接收或发送文件、测试文件是否存在或列出服务器上的文件。使用的协议可以是服务器到服务器协议，也可以是 HTTP 协议。[了解更多信息](../workflows/activities/transfer-file.md)
* **测试**：使用此活动可以根据指定的条件启用过渡。[了解更多信息](../workflows/activities/test.md)
* **JavaScript 代码**：使用此活动可以在工作流的上下文中执行 JavaScript 代码片段。[了解更多信息](../workflows/activities/javascript-code.md)
* **外部信号**：使用此活动可从另一个工作流或 API 调用触发工作流的执行。[了解更多信息](../workflows/activities/external-signal.md)
* **增量查询**：使用此活动可以按计划查询数据库。每次执行此活动时，都会排除先前执行得出的结果。这样可让您仅定向新元素。[了解更多信息](../workflows/activities/incremental-query.md)

**富推送通知**

您现在可以通过 Android 发送富推送通知。富推送通知是移动通知的一种增强形式，它不局限于简单的文本消息，而是融合了图像、交互式按钮或其他富媒体内容等多媒体元素。[了解更多信息](../push/rich-push.md)

请注意，此功能处于&#x200B;**有限可用性** (LA) 状态。


### 有限可用性版本中的新功能 {#acs-24-4}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。
>
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8](../rn/acs-migration.md) 以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hans)。

* **品牌化**：作为 Campaign Standard 迁移用户，您的技术管理员现在可以定义一个或多个品牌，以便集中管理影响品牌标识的参数。其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您可以创建这些品牌并将它们链接到消息或登陆页面。此配置在模板中进行管理。[了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=zh-Hans)

* **Rest API** - 作为 Campaign Standard 迁移用户，您可以使用 Rest API 为 Adobe Campaign 创建集成，并通过将 Adobe Campaign 与所使用的技术面板连接来构建自己的生态系统。[了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-Hans)

* **动态报告** - 作为 Campaign Standard 迁移用户，您可以访问动态报告，该功能提供完全可自定义的实时报告来衡量营销活动的影响。它增加了对用户档案数据的访问，除打开数和点击数等功能性电子邮件营销活动数据外，还支持按用户档案维度（如性别、城市和年龄）进行人口统计分析。[了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=zh-Hans)

* **登陆页面**：登陆页面的以下改进仅适用于从 Campaign Standard 过渡的用户：

   * 现在，您可以在配置服务时引用默认订阅/退订登陆页面。在设计电子邮件时，如果您定义了指向该登陆页面的链接，则提交登陆页面表单的用户将会自动订阅或退订此服务。[了解更多信息](../audience/manage-services.md#create-service)
   * 登陆页面配置中的新选项允许匿名访客访问登陆页面。如果取消选择此选项，则只有已识别的用户才能访问和提交表单。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 登陆页面配置中的一个新选项允许在提交登陆页面时存储额外的内部数据。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 新选项允许将一个登陆页面用于多项服务，从而使其具有动态性。在向电子邮件添加链接时，如果您选择动态登陆页面，则可以选择任何服务。如果您选择与特定服务关联的登陆页面，则会自动使用该服务（您不能选择其他服务）。[了解更多信息](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陆页面现在支持条件内容。[了解更多信息](../landing-pages/lp-content.md)

### 一般改进 {#improvements-24-4}

自 4 月版本开始，所有客户均可享受以下改进功能。
<!--**Workflow - Copy/Paste into another tab**: -->

* **加载文件**&#x200B;活动通过几个部分得到了增强，其中允许您上传示例文件、管理错误和拒绝内容，以及在活动执行后删除上传的文件。[了解更多信息](../workflows/activities/load-file.md)


* 您现在可以从不同的浏览器选项卡将活动从一个工作流&#x200B;**复制/粘贴**&#x200B;到另一个工作流。[了解更多信息](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* 现在，所有工作流活动都允许您管理其&#x200B;**执行选项**。这有助于您定义活动的执行模式和出现错误时的行为。[了解更多信息](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* **拆分活动**&#x200B;中的“如果群体为空，则不激活过渡”选项允许您选择当区段结果为空时工作流是否应过渡到下一个活动。[了解更多信息](../workflows/activities/split.md)



## 3 月发行说明 {#24-3-release}

>[!AVAILABILITY]
>
>此版本适用于所有 [Campaign（控制台）v8.6 及更高版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans)的用户。请参阅 [Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hans){target="_blank"}，了解有关 Adobe Campaign 客户端控制台版本和升级的更多信息。

**发布日期**：2024 年 3 月 19–20 日

### 直邮渠道 {#24-3-dm}

**直邮**&#x200B;渠道现在既可在工作流中使用，也可独立投放。直邮是一种离线渠道，允许您创建和生成提取文件、进行个性化设置，并与直邮提供商共享，向客户发送邮件。

### 新的更改数据源工作流活动 {#24-3-change-data-source}

**更改数据源**&#x200B;定位活动允许您更改工作流工作表使用的数据源。这项活动提供了更大的灵活性，使您可以跨不同的数据库管理数据并提高性能。

### 拆分工作流活动改进 {#24-3-split}

现在，您可以使用“**拆分**”工作流活动中的“**在同一表中生成所有子集**”选项，将所有子集分组到单个输出过渡中。

### 查询建模器 {#24-3-query-modeler}

* 查询建模器现在可在电子邮件设计器中使用。它允许您在创建条件内容时构建条件。
* 创建自定义条件时，预定义值现在可用于日期类型属性。
* 无法再在图中的新过渡上添加运算符。运算符只能添加到现有的过渡中，然后再过滤组件将它们组合在一起。
