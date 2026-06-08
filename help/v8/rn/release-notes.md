---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 777611699d3d4189cdd7d0d7ded66a9b08cf26cd
workflow-type: ht
source-wordcount: 610
ht-degree: 100%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。 我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

## 2026 年 4 月版本 {#26-4-release}

_2026 年 4 月 29 日_

### 改进 {#26-4-improvement}

**扩充数据**&#x200B;部分现已在&#x200B;**构建受众**&#x200B;工作流活动（查询类型）中提供。您可以直接在 Campaign Web 用户界面中查看、添加、编辑和移除&#x200B;**附加数据**。与&#x200B;**扩充**&#x200B;活动一样，您可以添加单个扩充属性、收藏集链接和表达式。

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

* 新增了&#x200B;**开始**工作流活动，以提高与客户端控制台的兼容性。此活动为可选活动，不会默认添加到新工作流中。不过，系统会自动将其添加到现有工作流中。
  [了解详情](../workflows/activities/about-activities.md#flow-control)
* 投放&#x200B;**计划**&#x200B;设置中的时区选择字段已移动至&#x200B;**联系日期**&#x200B;字段下方。 [了解详情](../msg/create-deliveries.md#gs-schedule)