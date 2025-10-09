---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 71%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 页面中列出了以前版本中的变更和改进。

## 2025年10月更新 {#25-9-updates}

_2025年10月9日_

<table>
<thead>
<tr>
<th><strong>事务性消息传递、推送通知和短信(LA)的多语言功能</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在Adobe Campaign Web用户界面中以不同语言发送多条事务型消息、推送通知和短信消息。 多语言投放功能允许您选择投放的默认语言以及可以发送投放的不同语言。您也可以使用所选的语言预览这些投放。</p>
<p>注意：此功能仅适用于一组组织（限量发布），并将在未来版本中全局推出。</p>
<p>有关更多信息，请参阅<a href="../msg/multilingual.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>事务性消息中的用户档案扩充(LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>此功能允许您通过将Adobe Campaign数据库字段链接到消息内容来个性化事务型消息。 您可以选择目标映射、扩充列和协调键值，以确保准确、实时的个性化，同时保持性能阈值。</p>
<p>注意：此功能仅适用于一组组织（限量发布），并将在未来版本中全局推出。 此功能当前仅适用于电子邮件。</p>
<p>有关更多信息，请参阅<a href="../transactional-messaging/profile-enrichment.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


## 2025 年 9 月版 {#25-9-release}

_2025 年 9 月 23 日_

以下功能自 9 月版本起提供。

<table>
<thead>
<tr>
<th><strong>用于 API 投放的自定义渠道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接从 Adobe Campaign Web UI 基于自定义 API 渠道来编排和执行投放。这些投放既可以独立执行，也可以作为工作流的一部分。自定义 API 渠道的配置需在控制台中完成。</p>
<p>有关更多信息，请参阅<a href="../call-center/gs-custom-channel.md">详细文档</a>。</p>
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
<p>作为 Campaign 管理员，您现在可以从 Campaign Web 用户界面建立与外部系统的新连接。您还可以查看、更新和管理现有的外部帐户。</p>
<p>有关更多信息，请参阅<a href="../administration/create-external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>电子邮件内容锁定</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign 现在支持在电子邮件模板中锁定内容，您可以选择锁定整个模板，或仅锁定特定结构和组件。这可帮助您防止内容被误编辑或误删除，从而更好地掌控模板定制，并提升电子邮件营销活动的效率与可靠性。</p>
<p>有关更多信息，请参阅<a href="../content/content-locking.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### 改进 {#25-9-improvements}

* 在使用电子邮件设计器的条件内容功能设置条件时，新增了一组运算符可供使用。
* 过滤维度现已在&#x200B;**构建受众**&#x200B;工作流活动中可用。要查看或更改，请单击目标维度旁边的图标。[了解详情](../workflows/activities/build-audience.md#build-audience-configuration)。
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

