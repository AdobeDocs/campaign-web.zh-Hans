---
title: Campaign v8 Web 用户界面早期发行说明
description: 2024 Campaign Web 用户界面发布
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: ht
source-wordcount: '2501'
ht-degree: 100%

---

# 2024 年发行说明 {#2024-release}

本页列出了 **2024 年版本**&#x200B;的所有变更和改进。最新发布说明可在 [此页面](release-notes.md)中查看。


## 2024 年 10 月版本 {#24-10-release}

**发行日期**：2024 年 10 月 29 日

自 10 月版本开始提供以下功能和改进。

### 功能

<table>
<thead>
<tr>
<th><strong>外部帐户</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接通过 Adobe Campaign Web 用户界面设置和管理外部帐户。此新功能可以轻松配置不同类型的外部帐户，例如退回电子邮件（POP3）或执行实例。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>交易型消息传递</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>交易消息传递（消息中心）现已在 Campaign 网络用户界面中提供。此附加组件用于触发由信息系统触发的事件生成的消息，可以是：发票、订单确认、发货确认、密码更改、产品不可用通知、帐户报表、网站帐户创建等等。</p>
<p>有关更多信息，请参阅<a href="../transactional-messaging/transactional.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


### 改进

* **工作流活动** - 您现在可以将活动及其所有子节点从工作流中的一个过渡移动到另一个过渡。活动的属性窗格中有一个专用的 **移动** 按钮可以执行此操作。[了解详情](../workflows/orchestrate-activities.md#move)

* **工作流扩充活动**

   * 现在，您可以在 **扩充** 活动中创建新字段时定义别名和标签。[了解详情](../workflows/activities/enrichment.md#collection-settings)
   * 您现在可以在 **扩充** 活动中为每个轮廓添加产品建议。[了解详情](../workflows/activities/enrichment.md##add-offers)

* **值的分布**：当访问个性化字段列表时，您现在可以检查每个字段的值是如何分布的。专用的弹出窗口显示每个值的数字和百分比。[了解详情](../query/build-query.md#distribution-values-query)

* **版本和系统信息** - 您现在可以访问有关实例版本的详细信息，包括客户端控制台和 Web 用户界面。此新部分还列出了您的环境中安装的所有内置包。[了解详情](../get-started/user-interface.md#user-interface-about)

* **列表** - 您现在可以轻松地重新排序列表的值。[了解详情](../get-started/work-with-folders.md)

* **投放** - 现在可以从个性化字段访问投放变量。[了解详情](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## 9 月更新 {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI 助手</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您的定制信息制作完成后，使用 Adobe Campaign Web 中的 AI 助手将其提升到一个新水平。使用这一功能强大的工具，您可以生成一系列引人入胜的文本、主标题以及在视觉上富有吸引力的图像来优化内容的影响力。</p>
<p>通过<a href="https://experienceleague.adobe.com/zh-hans/apps/journey-optimizer/ai-assistant-content-accelerator">我们的实时功能预览</a>，享受沉浸式的实践体验，让您亲自探索其功能并充分了解其能力</a>。</p>
<p>有关更多信息，请参阅<a href="../email/generative-gs.md">详细文档</a>。</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>发行日期：9 月 12 日</p>
</td>
</tr>
</tbody>
</table>

## 8 月版本 {#24-8-release}

**发布日期**：2024 年 9 月 3 日

自 8 月版本开始提供以下功能和改进。

* **SMTP 参数** - SMTP 设置现在可在电子邮件传递设置中使用。[了解详情](../advanced-settings/delivery-settings.md#smtp)

* **全局变量** - 您现在可以定义全局变量来定义您的投放的值。[了解详情](../advanced-settings/delivery-settings.md#variables-delivery)

### 有限可用性版本中的新功能 {#acs-24-8}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。
>
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8](../rn/acs-migration.md) 以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hans){target="_blank"}。

* **直邮的品牌化**：您的技术管理员现在可以定义一个或多个品牌，以便集中管理影响品牌标识的参数。其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您现在可以创建这些品牌并将它们链接到消息或登陆页面。此配置在模板中进行管理。[了解详情](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/branding/branding-assign)

* **带有登陆页面的订阅** - 您现在可以将登陆页面链接到服务，并在用户验证时发送确认消息。[了解详情](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **视觉片段**：您现在可以对视觉内容片段进行存档。[了解详情](../content/create-fragment.md#archive)

* **登陆页面中的验证码**：您现在可以使用 Google reCAPTCHA 机制保护您的登陆页面免受机器人造成的垃圾邮件和滥用的影响。对于您的客户而言，这是非侵入式的，因为它不需要与客户进行任何交互，并且基于与您网站的交互。[了解详情](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-Hans){target="_blank"}.-->


## 7 月份发行说明 {#24-7-release}

**发布日期**：2024 年 7 月 30-31 日

自 7 月版本开始可以使用以下功能和改进。

### 内容片段 {#24-7-1}

您现在可以创建和使用内容片段。内容片段是可重复使用的组件，可以在一条或多条消息中引用。当修改片段时，使用它的每个内容都会被更新。此功能用于预构建多个自定义内容块，营销用户可以使用这些块在改进的设计过程中快速组装消息内容。

有两种类型的片段可用：

* **表达式片段** 是预定义表达式，可从表达式编辑器中的专用条目中获取。
* **视觉片段** 是预定义的视觉块，您可以在多个电子邮件传递或内容模板中重复使用。[了解详情](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**视觉片段** 处于有限可用性（LA）。该功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。

### 陷印组 {#24-7-2}

**陷印组**&#x200B;是种子地址列表。它用于在您的投放中包含特定地址，然后定位不符合定义的目标标准的轮廓。这样，不在投放受众内的收件人就可以像其他目标收件人一样收到投放内容。您可以在发送校样或保护您的邮件列表时使用种子地址。[了解详情](../audience/trap-group.md)

### 富推送通知模板 {#24-7-3}

您现在可以发送富推送通知。富推送通知是移动通知的一种增强形式，它不局限于简单的文本消息，而是融合了图像、交互式按钮或其他富媒体内容等多媒体元素。在此版本中，您可以为您的 iOS 和 Android 应用程序提供一组丰富的推送通知模板。

[了解详情](../push/rich-push.md)

>[!AVAILABILITY]
>
>此功能需要更新至 Campaign v8.6.3 <!--or v8.7.2-->。若要了解更多信息，请参阅 Campaign v8 客户端控制台[发行说明](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/releases/release-notes){target="_blank"}。

### 改进 {#improvements-24-7}

**文件夹管理** - 您现在可以管理文件夹的权限和限制。

## 6 月发行说明 {#24-6-release}

**发行日期**：2024 年 6 月 18-19 日

自 6 月版本开始，所有用户都可以使用以下功能和改进。

### 投放警报 {#24-6-3}

投放警报功能是一个警报管理系统，利用该系统可让一组用户自动接收包含其投放执行信息的通知。[了解更多信息](../msg/delivery-alerting.md)

### 计划和项目 {#24-6-4}

您现在可以通过创建计划和项目来组织您的营销活动。通过定义文件夹层级，您可以将营销活动组织成项目，并将项目组织成计划。[了解更多信息](../administration/plans-programs.md)

### 改进 {#improvements-24-6}

* **扩充活动中的协调**：**扩充**&#x200B;活动现在可用于协调来自 Campaign 数据库架构的数据与来自另一个架构的数据，或来自临时架构的数据（例如使用“加载”文件活动上传的数据）。例如，您可以使用此选项将上传文件中指定的轮廓的国家/地区与 Campaign 数据库专用表中可用的国家/地区之一进行协调。[了解更多信息](../workflows/activities/enrichment.md)

## 5 月发行说明 {#24-5-release}

**发行日期**：2024 年 5 月 21 日

自 5 月版本开始，所有用户都可以使用以下功能和改进。

### 审核记录  {#24-5-1}

新的&#x200B;**审核记录**&#x200B;功能按时间顺序详细记录了对 Adobe Campaign 实例进行的所有操作和事件。它提供了一种追踪对 Campaign 数据进行的所有更改的简便方法，可解决诸如以下查询：工作流的状态、最近修改工作流的个人或实例内用户执行的活动。[了解更多信息](../reporting/audit-trail.md)

### 自定义字段 {#24-5-2}

**自定义字段**&#x200B;是通过 Adobe Campaign 控制台添加到现成架构的附加属性。在 Campaign Web 用户界面中，这些自定义字段现在可在各个屏幕中看到，例如轮廓或测试轮廓的详细信息。在 Web 用户界面中，您无法创建自定义字段，但现在您可以修改它们的显示方式。[了解更多信息](../administration/custom-fields.md)

### 在表之间创建链接 {#24-5-3}

您现在可以在&#x200B;**扩充**&#x200B;工作流活动中创建与另一个表的链接。使用活动参数中的新&#x200B;**链接定义**&#x200B;部分在工作表数据和 Adobe Campaign 数据库之间创建链接。例如，如果您从包含收件人的帐号、国家/地区和电子邮件的文件中加载数据，则您现在可以创建指向该国家/地区表的链接，以便在其轮廓中更新此信息。[了解更多信息](../workflows/activities/enrichment.md#create-links)

### 一般改进 {#improvements-24-5}

* **直邮**：您现在可以利用表达式编辑器来选择要在直邮提取文件中显示的属性。[了解更多信息](../direct-mail/content-direct-mail.md)

* **文件夹管理**：您现在可以创建与父文件夹不同类型的子文件夹。[了解更多信息](../get-started/permissions.md#folders)

* **全球化**：作为我们持续努力提供统一用户体验的一部分，我们统一了 Adobe Experience Cloud 产品和应用程序中使用的术语。这会影响德语术语“Titel”，当它与对象名称相关时会更改为“Label”。这些变化将会在 UI 和文档中逐步推出。


## 4 月发行说明 {#april-24-4-release}

**发行日期**：2024 年 5 月 2 日

### 新增功能 {#new-24-4}

自 4 月版本开始，所有用户都可以使用以下功能。

**新工作流活动**

* **更新数据**：使用此活动可以对数据库中的字段执行大规模更新。您可以利用多个选项，以个性化方式更新数据。[了解更多信息](../workflows/activities/update-data.md)
* **订阅服务**：使用此活动可在单个操作中向服务订阅或取消订阅多个轮廓。[了解更多信息](../workflows/activities/subscription-services.md)
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
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8](../rn/acs-migration.md) 以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hans)。

* **品牌化**：作为 Campaign Standard 迁移用户，您的技术管理员现在可以定义一个或多个品牌，以便集中管理影响品牌标识的参数。其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您可以创建这些品牌并将它们链接到消息或登陆页面。此配置在模板中进行管理。[了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=zh-hans)

* **Rest API** - 作为 Campaign Standard 迁移用户，您可以使用 Rest API 为 Adobe Campaign 创建集成，并通过将 Adobe Campaign 与所使用的技术面板连接来构建自己的生态系统。[了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-hans)

* **动态报告** - 作为 Campaign Standard 迁移用户，您可以访问动态报告，该功能提供完全可自定义的实时报告来衡量营销活动的影响。它增加了对轮廓数据的访问，除打开数和点击数等功能性电子邮件营销活动数据外，还支持按轮廓维度（如性别、城市和年龄）进行人口统计分析。[了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=zh-hans)

* **登陆页面**：登陆页面的以下改进仅适用于从 Campaign Standard 过渡的用户：

   * 现在，您可以在配置服务时引用默认订阅/退订登陆页面。在设计电子邮件时，如果您定义了指向该登陆页面的链接，则提交登陆页面表单的用户将会自动订阅或退订此服务。[了解更多信息](../audience/manage-services.md#create-service)
   * 登陆页面配置中的新选项允许匿名访客访问登陆页面。如果取消选择此选项，则只有已识别的用户才能访问和提交表单。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 登陆页面配置中的一个新选项允许在提交登陆页面时存储额外的内部数据。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 新选项允许将一个登陆页面用于多项服务，从而使其具有动态性。在向电子邮件添加链接时，如果您选择动态登陆页面，则可以选择任何服务。如果您选择与特定服务关联的登陆页面，则会自动使用该服务（您不能选择其他服务）。[了解更多信息](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陆页面现在支持条件内容。[了解更多信息](../landing-pages/lp-content.md)

### 一般改进 {#improvements-24-4}

自 4 月版本开始，所有客户均可享受以下改进功能。

* **加载文件**&#x200B;活动通过几个部分得到了增强，其中允许您上传示例文件、管理错误和拒绝内容，以及在活动执行后删除上传的文件。[了解更多信息](../workflows/activities/load-file.md)


* 您现在可以从不同的浏览器选项卡将活动从一个工作流&#x200B;**复制/粘贴**&#x200B;到另一个工作流。[了解更多信息](../workflows/orchestrate-activities.md#copy-activities-copy)

* 现在，所有工作流活动都允许您管理其&#x200B;**执行选项**。这有助于您定义活动的执行模式和出现错误时的行为。[了解更多信息](../workflows/orchestrate-activities.md#execution-options-execution)

* **拆分活动**&#x200B;中的“如果群体为空，则不激活过渡”选项允许您选择当区段结果为空时工作流是否应过渡到下一个活动。[了解更多信息](../workflows/activities/split.md)

## 3 月发行说明 {#24-3-release}

>[!AVAILABILITY]
>
>此版本适用于所有 [Campaign（控制台）v8.6 及更高版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-hans)的用户。请参阅 [Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-hans){target="_blank"}，了解有关 Adobe Campaign 客户端控制台版本和升级方面的更多信息。

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