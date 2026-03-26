---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

## 2026年3月版 {#26-3-release}

### 新增功能 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>架构创作(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>架构创作功能现在可供所有客户使用(GA)。 此功能允许您直接从Campaign Web用户界面创建和管理架构。 您可以创建新表、扩展现有模式以及创建自定义表单。 您可以定义自定义数据结构来支持您的特定业务需求，而无需访问客户端控制台。</p>
<p>有关更多信息，请参阅<a href="../administration/schemas.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Email Designer (LA)中的主题</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>主题通过允许您定义符合品牌准则的可重用主题样式，提供了改进的电子邮件创作体验。 您现在可以在片段中使用主题变量，确保电子邮件模板中的样式一致。 此功能允许您使用预定义模块更快地构建电子邮件，这些模块抽象了标题、描述、图像和链接等内容元素，同时维护品牌一致性。</p>
<p>注释：此功能目前仅面向部分组织开放（限量发布版），将在未来版本中逐步向全球推广。</p>
<p>有关更多信息，请参阅<a href="../email/apply-email-themes.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>自定义Firefly模型与第三方图像生成模型的集成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>实现标准和自定义Firefly模型与经批准的第三方图像模型的无缝集成，以在生成图像时提供更大的灵活性、控制力以及品牌一致性。</p>
<p>根据您的需求选择合适的模型：</p>
<ul><li> <strong>Adobe模型</strong>（由Firefly Image Model 4提供支持），无需其他设置即可立即生成图像</li><li> <strong>合作伙伴型号</strong> （由Gemini 2.5 Flash提供支持）提供专业功能</li><li><strong>自定义模型</strong>（基于您自己的资产进行培训的品牌特定模型），用于生成与您的品牌标识、风格和视觉准则完全一致的品牌。</li></ul>
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
<p><strong>自动投放</strong>工作流活动现在在工作流面板中可用。 您可以用它直接在工作流中创建或执行投放操作（准备、发送验证、准备和启动等）。 选择在工作流之外创建的现有投放以在每次运行时重用它，或在每次活动执行时从模板创建新投放。</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>有关详细信息，请参阅<a href="../workflows/activities/automated-delivery.md">详细文档。</p>
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

<p>现在支持<strong>多个分支</strong>。 您可以单击工具栏上的“添加分支”<strong></strong>，而不是使用<strong>分支</strong>。 <strong>AND-join</strong>活动也已得到改进。 它现在是一个通用的<strong>连接</strong>活动，允许您在AND和OR连接选项之间进行选择。</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>有关详细信息，请参阅<a href="../workflows/orchestrate-activities.md#toolbar">编排活动</a>和<a href="../workflows/activities/join.md">加入</a>文档页面。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-3-improvements}

* 已添加&#x200B;**Start**工作流活动，以改善与客户端控制台的兼容性。 此活动是可选的，默认情况下不会插入新的工作流中。 但是，它会自动添加到现有工作流中。
  [了解详情](../workflows/activities/about-activities.md#flow-control)
* 投放的&#x200B;**计划**&#x200B;设置中的时区选择字段已移动到&#x200B;**联系日期**&#x200B;字段下方。 [了解详情](../msg/create-deliveries.md#gs-schedule)