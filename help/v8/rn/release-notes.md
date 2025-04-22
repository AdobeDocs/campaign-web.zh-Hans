---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 96%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面的发布采用持续投放模型，该模型支持以可扩展、分阶段的方式进行功能部署。因此，这些发行说明每月更新几次。请定期查看。

[本页](release-notes-24.md)列出了以前版本中的变更和改进。

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
<p>您现在可以在 Adobe Campaign Web 用户界面中创建类型和类型规则。使用类型可以控制和筛选投放的发送并确定其优先顺序。使用类型可以验证投放是否始终包含强制组件（如退订链接或主题行）或过滤规则，以从您的受众中排除群组（如取消订阅者、竞争对手或非忠诚客户）。</p>
<img src="assets/do-not-localize/typology.gif" alt="Adobe Campaign Web 用户界面中类型规则创建的说明">
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
<p>您现在可以在 Campaign Web 用户界面中创建目标映射。目标映射定义了不同的投放渠道（电子邮件、SMS、推送）如何链接到一个架构的数据字段。目标映射功能可以定义目标受众：轮廓、合同受益人、运营商、订阅者、潜在客户等。</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Adobe Campaign Web 用户界面中目标映射创建的说明">
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
<p>现在，您可以通过在列表中选择某个架构的名称来访问该架构的详细信息。现在可以通过架构详细信息中的<b>编辑自定义字段</b>按钮访问自定义字段编辑功能。</p>
<img src="assets/do-not-localize/schemas.gif" alt="Adobe Campaign Web 用户界面中的架构详细信息和自定义字段编辑功能的说明">
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
<img src="assets/do-not-localize/visual-fragment.gif" alt="Adobe Campaign Web 用户界面中视觉片段的创建和使用的说明">
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
<img src="assets/do-not-localize/external-delivery.gif" alt="Adobe Campaign Web 用户界面中的外部投放设置的说明">
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
<p>您现在可以直接通过 Adobe Campaign 网络用户界面创建枚举。枚举是系统建议填充字段的值列表。使用枚举来标准化这些字段的值，辅助数据输入，或在查询中使用。</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Adobe Campaign Web 用户界面中的枚举管理说明">
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
<img src="assets/do-not-localize/options.gif" alt="Adobe Campaign Web 用户界面中自定义选项创建的说明">
<p>有关更多信息，请参阅<a href="../administration/options.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>定义并调用 JavaScript 代码</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Adobe Campaign 网络用户界面中创建 JavaScript 代码。这允许您创建可跨工作流使用的可重用函数，类似于库。</p>
<img src="assets/do-not-localize/javascript.gif" alt="Adobe Campaign Web 用户界面中 JavaScript 代码创建的说明">
<p>有关更多信息，请参阅<a href="../administration/javascript-codes.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用AI助手生成登陆页面</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>AI助手现在可用于登陆页面投放，使您能够生成文本、图像或完整的页面布局。</p>
<img src="assets/do-not-localize/ai-lp.gif" alt="在 Adobe Campaign Web 用户界面中使用 AI 助手生成登陆页面的说明">
<p>有关 AI 助手的更多信息，请参阅<a href="../email/generative-lp.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#25-1-improvements}

* 定制界面中自定义字段的显示：
   * 选择要在界面中显示的其他自定义字段。
   * 设置链接类型自定义字段的显示规则，例如根据另一个字段的输入来限制列表值。
   * 更灵活地排列界面中的字段：字段可以跨越单个列，也可以分组到子部分中，以更好地组织。
   * 将特定字段设置为只读。

* 最近和收藏夹过滤器：将常用属性添加到收藏夹中，以便快速访问。除了收藏夹，查看和使用最近选择的属性。

* 外部帐户：在创建新的外部帐户时，可以选择新的&#x200B;**[!UICONTROL 路由]**&#x200B;类型。它允许您配置一个特定的外部帐户，以用于外部投放。[了解详情](../administration/external-account.md#routing)。