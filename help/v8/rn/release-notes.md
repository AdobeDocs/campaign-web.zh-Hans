---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ca1a437f8a8a25c0a15b9148e9c73271795f16c7
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 100%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 页面中列出了以前版本中的变更和改进。

## 2025 年 10 月版本 {#25-10-updates}

_2025 年 11 月 3 日_

<table>
<thead>
<tr>
<th><strong>事务性消息、推送通知和短信（LA）的多语言功能</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在 Adobe Campaign Web 用户界面中以不同语言发送多条事务性消息、推送通知和短信消息。多语言投放功能允许您选择投放的默认语言以及可以发送投放的不同语言。您还可以使用您选择的语言预览这些投放内容。</p>
<p>注释：此功能目前仅面向部分组织开放（限量发布版），将在未来版本中逐步向全球推广。</p>
<p>有关更多信息，请参阅<a href="../msg/multilingual.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>事务性消息中的轮廓扩充（LA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>此功能允许您通过将 Adobe Campaign 数据库字段链接到消息内容来个性化事务性消息。您可以选择目标映射、扩充列和协调键，以确保准确、实时的个性化，同时保持性能阈值。</p>
<p>注释：此功能目前仅面向部分组织开放（限量发布版），将在未来版本中逐步向全球推广。此功能目前仅适用于电子邮件。</p>
<p>有关更多信息，请参阅<a href="../transactional-messaging/profile-enrichment.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>与 Adobe GenStudio 集成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>为提升营销效率并保持品牌一致性，您现在可以将 GenStudio for Performance Marketing 体验与 Campaign 无缝集成。这使您能够结合使用 GenStudio 的 AI 驱动内容创作功能与 Campaign 的高级编排能力。<p>
<p>有关更多信息，请参阅<a href="../integrations/genstudio.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>电子邮件设计器中的深色模式支持</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>电子邮件设计器现已支持切换至深色模式视图，您还可以在该模式下定义特定的自定义设置。请注意，电子邮件的最终呈现效果取决于收件人的电子邮件客户端，并非所有电子邮件客户端都支持深色模式。</p>
<p>有关更多信息，请参阅<a href="../email/dark-mode.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### 改进 {#25-10-improvements}

* 在客户端控制台中创建的投放中，**受众**&#x200B;部分现在会显示是否已为校样目标定义动态条件。<!-- [Learn more](../msg/gs-deliveries.md#access)-->

* 使用电子邮件设计器的条件内容功能设置条件时，您现在可以在新版规则生成器与旧版规则生成器之间切换。<!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* 您现在可以在收件人架构的屏幕定义中选择收藏集链接，例如购买记录。这样可通过专用选项卡在轮廓界面中显示相关数据。<!-- [Learn more](../administration/schemas.md#collection-lists)-->

* 作为 Campaign 管理员，您现在可以设置与 Salesforce CRM 和 Microsoft Dynamics 的连接。
  [了解详情](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

