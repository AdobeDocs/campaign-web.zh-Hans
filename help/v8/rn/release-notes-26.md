---
title: Campaign v8 Web 用户界面早期发行说明
description: 2026 Campaign Web 用户界面发布
source-git-commit: abec861b2c542644b90d3385fb5cf1d785ae7b70
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 20%

---

# 2026 年发行说明 {#2026-release}

本页列出了 **2026 年版本**&#x200B;的所有变更和改进。在[此页面](release-notes.md)中提供了最新发行说明。

## 2026年1月版 {#26-1-release}

_2026 年 1 月 27 日_

### 新增功能 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>多语言交付功能(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>多语言交付功能现在向所有客户提供(GA)。 利用此功能，可在Adobe Campaign Web用户界面中以不同语言发送多条消息。 您可以选择投放的默认语言以及可发送投放的不同语言。 您还可以使用您选择的语言预览这些投放内容。 
<p>有关更多信息，请参阅<a href="../msg/multilingual.md">详细文档</a>。</p>
<p>对多语言推送通知进行了以下改进：</p>
<ul>
<li>您现在可以通过上传包含多语言内容的CSV文件来快速填充所有语言变体。 <a href="../msg/multilingual.md#csv-upload">了解更多信息</a>
</li>
<li>现在支持富推送通知。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>事务性消息中的用户档案扩充(GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>现在，所有客户都可以使用“事务性消息中的用户档案扩充”功能(GA)。 除了电子邮件之外，现在还支持短信和推送通知。 此功能允许您通过将Adobe Campaign数据库字段链接到消息内容来个性化事务型消息。 您可以选择目标映射、扩充列和协调键，以确保准确、实时的个性化，同时保持性能阈值。</p>
<p>有关更多信息，请参阅<a href="../transactional-messaging/profile-enrichment.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager实时和语言副本</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Manager内容集成允许您在构建投放时直接在Campaign中访问在Adobe Experience Manager中创建的所有语言和活动副本。 您可以实时刷新内容以获取最新的Adobe Experience Manager版本。 此集成消除了Adobe Experience Manager和Campaign之间的手动内容同步，简化了多语言活动工作流。</p>
<p>有关更多信息，请参阅<a href="../integrations/aem-multilingual.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>内容实验 — A/B测试</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign Web中的内容实验允许您定义多个A/B测试投放变体，以衡量哪些变体最符合您的目标受众。 您可以更改投放内容、主题或发件人，以测试不同的版本并确定哪个变体产生最佳结果。 您可以对不同的电子邮件元素（如主题行、发件人姓名和电子邮件正文内容）执行A/B测试。</p>
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
<p>利用连续投放活动，可将新收件人添加到现有投放。 此投放类型可避免每次都创建新投放，从而更有效地根据需要发送低流量警报或通知。 连续投放会创建单个投放实例。 所有投放日志(broadLog)和跟踪日志都引用此一次投放，从而简化了监控和报告。</p>
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
<p>批准流程有助于协调多个利益相关者，并确保在发送投放之前进行质量控制。 当您的组织需要经过不同团队的验证时，例如营销经理审查内容或数据分析师验证目标受众，请使用批准。</p>
<p>有关更多信息，请参阅<a href="../campaigns/campaign-approvals.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-1-improvements}

* 动态报告现在支持推送通知和短信。 [了解详情](../reporting/dynamic-reporting/get-started-reporting.md)
* 预定义过滤器 — 通过新的“共享过滤器”选项，您可以使预定义过滤器可供组织中的其他用户使用。 [了解详情](../get-started/predefined-filters.md#share-filter)
* 现在包括在Adobe Experience Manager中创建的个性化字段，例如名称、电子邮件、日期和地址，这些字段在使用内容模板时可用。
* 内容质量评估现在检查可读性、一致性和有效性问题，而不依赖于品牌准则，识别不明确的消息、不一致的语调或结构性缺口。 [了解详情](../content/brands-score.md)
