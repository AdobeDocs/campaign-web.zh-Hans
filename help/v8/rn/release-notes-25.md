---
title: Campaign v8 Web 用户界面早期发行说明
description: 2025 Campaign Web 用户界面发布
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: ht
source-wordcount: '1604'
ht-degree: 100%

---

# 2025 年发行说明 {#2025-release}

本页列出了 **2025 年版本**&#x200B;的所有变更和改进。最新发布说明可在 [此页面](release-notes.md)中查看。

## 2025 年 6 月版本 {#25-6-release}

### 改进 {#25-6-improvements}

* “投放摘要”报告现已适用于呼叫中心和自定义渠道。[了解详情](../reporting/direct-mail.md)

* 在配置短信投放时，您现在可以访问特定的短信参数。这些参数与客户端控制台中提供的参数相同。[了解详情](../advanced-settings/delivery-settings.md#sms-tab)

* 您收藏的文件夹现在会显示在资源管理器页面左侧面板的顶部，方便快速访问。[了解详情](../get-started/work-with-folders.md#favorite-folders)

* 规则构建器现已支持拖放操作，使您能够更高效地重新排列查询组件。[了解详情](../query/build-query.md#drag-and-drop)

* 规则构建器中的“人工条件”功能已得到优化。这是您规则的书面简明语言版本，显示在屏幕底部：

   * 属性现在会高亮显示，并会展示其关联的架构。
   * 您可以点击这些元素以查看更详细的信息。
   * 您现在可以使用相应的按钮复制“人工条件”内容。

* 为防止查看，“技术工作流”和“自动创建的对象”文件夹的访问权限现已受到限制。[了解详情](../get-started/work-with-folders.md#about-folders)

## 2025 年 5 月版本 {#25-5-release}

自 5 月版本开始，所有用户都可以使用以下功能。

<table>
<thead>
<tr>
<th><strong>品牌一致性得分 (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>品牌一致性得分功能可直接在电子邮件设计器中提供清晰的反馈，帮助您了解内容是否符合品牌的基调、风格和指南。Beta 测试版提供此功能。</p>
<p>有关更多信息，请参阅<a href="../content/brands-score.md">详细文档</a>。</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>自定义外部投放渠道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接从 Adobe Campaign Web UI 根据自定义外部渠道协调和执行投放。这些投放可以是独立的，也可以是工作流的一部分。与第三方集成的自定义外部渠道在控制台中创建。</p>
<p>注意：自定义渠道的 Web UI 中不提供报告。您必须在浏览器中前往客户端控制台才能访问报告。</p>
<p>有关更多信息，请参阅<a href="../call-center/gs-custom-channel.md">详细文档</a>。</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### 改进 {#25-5-improvements}

类型规则创建屏幕已更新，以方便选择规则类型。

## 2025 年 4 月版本 {#25-4-release}

**发布日期**：2025 年 4 月 29 日

### 新增功能 {#25-4-features}

自 4 月版本开始，所有用户都可以使用以下功能。

<table>
<thead>
<tr>
<th><strong>呼叫中心渠道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign Web 用户界面中现在提供呼叫中心渠道。此渠道是指用于管理和跟踪通过呼叫中心处理的通信或交互的通信方法——通常是代理给客户或潜在客户拨打电话。</p>
<p>注意：呼叫中心渠道的 Web UI 中不提供报告。您必须在浏览器中前往客户端控制台才能访问报告。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>有关更多信息，请参阅<a href="../call-center/gs-call-center.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新的规则生成器</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>现在可以使用新的规则生成器来帮助您在改进的用户界面中定义复杂的条件。您可以根据需要从旧规则生成器切换到新规则生成器。</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>有关更多信息，请参阅<a href="../query/query-modeler-overview.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部帐户创作</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>作为 Campaign 管理员，您现在可以从 Campaign Web 用户界面建立与外部系统的新连接。
您还可以查看、更新和管理现有的外部帐户。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#25-4-improvements}

**通用界面改进**

* 现在，用户界面中可以更清楚地看到架构属性的字段描述、添加到收藏夹和值分配三个选项。有关更多信息，请参阅[详细文档](../get-started/attributes.md)。
* 在界面中，现在根据 Experience League 偏好设置中设置的主要语言显示日期和时间。此改进仅适用于几种语言。要查看受支持语言的完整列表，请参阅[详细文档](https://experienceleague.adobe.com/zh-hans/docs/core-services/interface/features/browser-language){target=_blank}。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**电子邮件编辑器**：为了增强 Campaign Web UI 的可访问性，电子邮件设计器中现在提供两个新字段：它们涉及电子邮件内容的 `title` 元素和 `html` 元素中的 lang 属性。除了邮件引文字段之外，您还可以在电子邮件正文部分定义这些设置。有关更多信息，请参阅[详细文档](../email/metadata.md)。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**架构**

* 您现在可以从 Campaign Web 用户界面为列表编辑临时架构。有关更多信息，请参阅[详细文档](../audience/manage-audience.md)。
* 您现在可以在示例屏幕中预览架构的自定义字段。有关更多信息，请参阅[详细文档](../administration/custom-fields.md#add)。
* 您现在可以使用拖放功能移动列表中的自定义字段。有关更多信息，请参阅[详细文档](../administration/custom-fields.md#add)。


### 有限可用性版本中的新功能 {#25-4-features-la}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。使用这些功能必须将 Campaign 服务器升级到 v8.7.4。
>
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8](../rn/acs-migration.md) 以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hans)。

* **创建多语言投放** - 您现在可以在 Adobe Campaign Web 用户界面中使用不同语言发送多个电子邮件投放。多语言投放功能允许您选择投放的默认语言以及可以发送投放的不同语言。您还可以使用您选择的语言预览这些投放内容。有关更多信息，请参阅[详细文档](../email/edit-content.md)。

* **多语言的动态报告** - 动态报告现可用于多语言电子邮件投放。有关更多信息，请参阅[详细文档](../reporting/global-reports.md)。

* **SMS REST API 支持 (LA)** - 事务性消息传递 REST API 现可用于 SMS 渠道。当负载中同时存在电子邮件和移动电话时，您可以使用“wishedChannel”字段来指定渠道。如果未提供，则默认使用电子邮件，除非 wishedChannel 明确请求 SMS。有关更多信息，请参阅[详细文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target=_blank}。

## 2025 年 2 月版本 {#25-2-release}

**发行日期**：2025 年 2 月 18 日

自 2 月版本开始可以使用以下功能和改进。

### 功能 {#25-2-features}

<table>
<thead>
<tr>
<th><strong>创建业务规则（类型规则）</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Adobe Campaign Web 用户界面中创建类型和类型规则。使用类型，您可以控制和筛选投放的发送并确定其优先顺序。类型用于验证投放是否始终包含强制组件（如退订链接或主题行）或过滤规则，以从您的受众中排除群组（如取消订阅者、竞争对手或非忠诚客户）。</p>
<img src="assets/do-not-localize/typology.gif">
<p>有关更多信息，请参阅<a href="../administration/typologies.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>目标映射</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Campaign Web 用户界面中创建目标映射。目标映射定义了不同的投放渠道（电子邮件、SMS、推送）如何链接到一个架构的数据字段。目标映射有助于您定义目标受众：个人资料、合同受益人、运营商、订阅者、潜在客户等。</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>有关更多信息，请参阅<a href="../administration/target-mappings.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>架构详细信息</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>现在，您可以通过在列表中选择某个架构的名称来访问该架构的详细信息。现在可以通过架构详细信息中的<b>编辑自定义字段</b>按钮访问自定义字段版本。</p>
<img src="assets/do-not-localize/schemas.gif">
<p>有关更多信息，请参阅<a href="../administration/schemas.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

## 2025 年 1 月版本 {#25-1-release}

**发行日期**：2025 年 2 月 5 日

自 1 月版本开始可以使用以下功能和改进。

### 功能 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>创建并使用视觉片段</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>视觉片段是预定义的视觉块，您可以在多个电子邮件投放或内容模板中重复使用。此功能现已可供运行服务器版本 8.6.4 及更高版本的所有客户使用。</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>有关更多信息，请参阅<a href="../content/use-visual-fragments.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用第三方系统进行投放</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Campaign 网络界面中定义外部投放和外部投放模板。在这种模式下，消息会被编译成一个输出文件，并可以与外部提供商共享。默认情况下，直邮渠道使用外部投放模式。</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>有关更多信息，请参阅<a href="../msg/send-external-deliveries.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>管理您的枚举</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接通过 Adobe Campaign 网络用户界面创建枚举。枚举是系统建议填充字段的值列表。使用枚举来标准化这些字段的值，有助于数据输入或在查询中使用。</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>有关更多信息，请参阅<a href="../administration/enumerations.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>创建自定义选项</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Adobe Campaign 网络用户界面中访问技术选项，并通过创建自己的自定义选项来满足您的需求。在使用 JavaScript 代码工作流活动存储中间数据时，这一点特别有用。</p>
<img src="assets/do-not-localize/options.gif">
<p>有关更多信息，请参阅<a href="../administration/options.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>定义并调用 Javascript 代码</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Adobe Campaign 网络用户界面中创建 JavaScript 代码。这允许您创建可跨工作流使用的可重用函数，类似于库。</p>
<img src="assets/do-not-localize/javascript.gif">
<p>有关更多信息，请参阅<a href="../administration/javascript-codes.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用 AI 助手生成登陆页面</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>AI 助手现在可用于您的登陆页面投放，使您能够生成文本、图像或完整的页面布局。</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>有关 AI 助手的更多信息，请参阅<a href="../email/generative-lp.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


### 改进 {#25-1-improvements}

* 定制界面中自定义字段的显示：

   * 您现在可以选择在界面中显示其他自定义字段
   * 现在，您可以设置显示链接类型自定义字段的规则，例如根据另一个字段的输入限制列表值
   * 现在，您可以更灵活地排列界面中的字段：字段可以跨越单个列，也可以分组到子部分中以更好地组织
   * 现在，您可以将特定字段设置为只读

* 最近和收藏夹过滤器：要快速重用经常使用的属性，您现在可以将它们添加到收藏夹中。这可以确保它们在未来的任务中易于访问。除了收藏夹，您还可以查看和使用最近选择的属性。

* 外部帐户：在创建新的外部帐户时，可以选择新的&#x200B;**[!UICONTROL 路由]**&#x200B;类型。它允许您配置一个特定的外部帐户，以用于外部投放。[了解详情](../administration/external-account.md#routing)
