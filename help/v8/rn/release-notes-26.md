---
title: Campaign v8 Web 用户界面早期发行说明
description: 2026 Campaign Web 用户界面发布
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: ed3fd4bbe8466c049af13304526daea948ab4706
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 97%

---

# 2026 年发行说明 {#2026-release}

本页列出了 **2026 年版本**&#x200B;的所有变更和改进。 最新发行说明可在[此页面](release-notes.md)查看。

## 2026 年 4 月版本 {#26-4-release}

_2026 年 4 月 29 日_

### 改进 {#26-4-improvement}

**扩充数据**&#x200B;部分现已在&#x200B;**构建受众**&#x200B;工作流活动（查询类型）中提供。 您可以直接在 Campaign Web 用户界面中查看、添加、编辑和移除&#x200B;**附加数据**。 与&#x200B;**扩充**&#x200B;活动一样，您可以添加单个扩充属性、收藏集链接和表达式。

[了解详情](../workflows/activities/build-audience.md)

## 2026 年 3 月版本 {#26-3-release}

2026 年 _3_ 月 24 日_

### 新增功能 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>架构创作（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>“架构创作”功能现已面向所有客户正式发布（GA）。 此功能允许您直接通过 Campaign Web 用户界面创建和管理架构。 您可以创建新表、扩展现有架构以及创建自定义表单。 您可以定义自定义数据结构，以满足您的特定业务需求，而无需访问客户端控制台。</p>
<p>有关更多信息，请参阅<a href="../administration/schemas.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>电子邮件设计器中的主题（LA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>主题通过允许您定义符合品牌指南的可重复使用主题样式，从而提升了电子邮件的编写体验。 现在，您可以在片段中使用主题变量，从而确保所有电子邮件模板的样式保持一致。 该功能通过预定义模块，将标题、描述、图片和链接等内容元素提取出来，同时确保品牌一致性，让您更高效地构建电子邮件。</p>
<p>注释：此功能目前仅面向部分组织开放（限量发布版），将在未来版本中逐步向全球推广。</p>
<p>有关更多信息，请参阅<a href="../email/apply-email-themes.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>自定义 Firefly 模型与第三方图像生成模型的集成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>启用标准和自定义 Firefly 模型以及经过批准的第三方图像模型的无缝集成，从而在生成图像时提供更大的灵活性、控制力以及品牌一致性。</p>
<p>根据您的需求选择合适的模型：</p>
<ul><li> <strong>Adobe 模型</strong>（基于 Firefly Image Model 4），无需额外设置即可即时生成图像</li><li> <strong>合作伙伴模型</strong>（基于 Gemini 2.5 Flash），专为特定功能而设计</li><li><strong>自定义模型</strong>（基于您自有资产训练的特定品牌模型），可生成完全符合您的品牌形象、风格和视觉指南的内容。</li></ul>
<p>有关更多信息，请参阅<a href="../content/generative-models.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>自动投放活动</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>自动投放</strong>工作流活动现已可在工作流调色盘中使用。 您可以用它来创建或执行投放操作（准备、发送验证、准备和启动等） 直接在您的工作流中。 选择在工作流外部创建的现有投放，以便在每次运行时重复使用；或者在每次执行该活动时，根据模板创建新的投放。</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>有关更多信息，请参阅<a href="../workflows/activities/automated-delivery.md">详细文档。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>多个工作流分支和连接活动</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>现在支持<strong>多个分支</strong>。 不使用<strong>分叉</strong>，而是单击工具栏上的<strong>添加分支</strong>。 <strong>AND-join</strong> 活动也已得到改进。 它现在是一个通用的 <strong>Join</strong> 活动，允许您在 AND 和 OR 连接选项之间选择。</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>有关更多信息，请参阅<a href="../workflows/orchestrate-activities.md#toolbar">编排活动</a>和<a href="../workflows/activities/join.md">连接</a>文档页面。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-3-improvements}

* 新增了&#x200B;**开始**&#x200B;工作流活动，以提高与客户端控制台的兼容性。此活动为可选活动，不会默认添加到新工作流中。不过，系统会自动将其添加到现有工作流中。
  [了解详情](../workflows/activities/about-activities.md#flow-control)
* 投放&#x200B;**计划**&#x200B;设置中的时区选择字段已移动至&#x200B;**联系日期**&#x200B;字段下方。 [了解详情](../msg/create-deliveries.md#gs-schedule)

## 2026 年 2 月版本 {#26-2-release}

_2026 年 2 月 17 日_

### 新增功能 {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>营销活动库存的时间线视图</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>营销活动库存现新增了“时间线”视图，可让您直观地查看并管理营销活动随时间的变化：在列表视图和时间线视图之间切换，按周、月或天浏览，点击“今天”按钮跳转至当前日期，并在右侧面板中查看营销活动详细信息（状态、工作流、投放）。该视图支持与列表视图相同的过滤器和搜索功能。</p>
<p>有关更多信息，请参阅<a href="../campaigns/manage-campaigns.md#timeline">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>架构创作（LA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接从 Campaign Web 用户界面创建和管理架构。 此功能允许您创建新表、扩展现有架构以及创建自定义表单。 您可以定义自定义数据结构，以满足您的特定业务需求，而无需访问客户端控制台。</p>
<p>注释：此功能目前仅面向部分组织开放（限量发布版），将在未来版本中逐步向全球推广。</p>
<p>有关更多信息，请参阅<a href="../administration/schemas.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## 2026 年 1 月版本 {#26-1-release}

_2026 年 1 月 27 日_

### 新增功能 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>多语言投放功能（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>多语言交付功能现在向所有客户提供(GA)。利用此功能，可在Adobe Campaign Web用户界面中以不同语言发送多条消息。您可以选择投放的默认语言以及可发送投放的不同语言。您也可以使用所选的语言预览这些投放。 
<p>有关更多信息，请参阅<a href="../msg/multilingual.md">详细文档</a>。</p>
<p>多语言推送已进行以下改进：</p>
<ul>
<li>您现在可以通过上传包含多语言内容的CSV文件来快速填充所有语言变体。<a href="../msg/multilingual.md#csv-upload">阅读更多</a>
</li>
<li>现已支持富媒体推送。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>事务性消息中的轮廓扩充（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>事务性消息中的轮廓扩充功能现已向所有客户开放（GA）。 除电子邮件外，现在还支持短信和推送。 此功能允许您通过将 Adobe Campaign 数据库字段与消息内容关联，来个性化事务性消息。 您可以选择目标映射、扩充列和协调键，以确保准确、实时的个性化，同时保持性能阈值。</p>
<p>有关更多信息，请参阅<a href="../transactional-messaging/profile-enrichment.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager 实时副本和语言副本</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>借助 Adobe Experience Manager 内容集成，您在 Campaign 中构建投放时，可直接访问在 Adobe Experience Manager 中创建的所有语言副本和实时副本。 您可以实时刷新内容，以获取最新的 Adobe Experience Manager 版本。 此集成消除了 Adobe Experience Manager 与 Campaign 之间的手动内容同步，从而简化了您的多语言营销活动工作流。</p>
<p>有关更多信息，请参阅<a href="../integrations/aem-multilingual.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>内容试验 - A/B 测试</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>在 Adobe Campaign Web 中进行内容试验，您可以定义多个 A/B 测试投放变体，从而衡量哪一种对目标受众的效果最佳。 您可以变化投放内容、主题或发件人，以测试不同的版本，确定哪个变体能产生最佳结果。 您可以对电子邮件的各种元素（如主题行、发件人姓名和电子邮件正文内容）进行 A/B 测试。</p>
<p>有关更多信息，请参阅<a href="../email/ab-testing.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>连续投放活动</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>持续投放允许您向现有投放添加新的收件人。 此类投放无需每次都创建新投放，更适用于按需发送的小规模提醒或通知，可提升效率。 一次持续投放会创建一个投放实例。 所有投放日志（broadLog）和跟踪日志均指向此次投放，从而简化了监控和报告。</p>
<p>有关更多信息，请参阅<a href="../workflows/activities/continuous-delivery.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>活动审批管理</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>审批流程有助于协调各方利益相关者，并在投放前确保质量控制。 当您的组织需要不同团队进行验证时，请使用审批功能，例如市场经理审阅内容，或数据分析师验证目标受众。</p>
<p>有关更多信息，请参阅<a href="../campaigns/campaign-approvals.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-1-improvements}

* 动态报告现已支持推送和短信。 [了解详情](../reporting/dynamic-reporting/get-started-reporting.md)
* 预定义过滤器：新增的“共享过滤器”选项可让您将预定义过滤器提供给组织中的其他用户。 [了解详情](../get-started/predefined-filters.md#share-filter)
* 在 Adobe Experience Manager 中创建的个性化字段（例如姓名、电子邮件、日期和地址）现已包含在内容模板中，并可供使用。
* 内容质量评估现可独立于品牌指南，对可读性、连贯性和有效性问题进行检查，从而识别出表述不清、语气不一致或结构缺失等问题。 [了解详情](../content/brands-score.md)
