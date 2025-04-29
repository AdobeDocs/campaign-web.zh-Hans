---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 589d78737a498ffe91cb49a6f689f4104b244d0b
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 34%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

以前版本中可用的更改和改进在[2024](release-notes-24.md)和[2025](release-notes-25.md)中列出。

## 2025年4月版 {#25-4-release}

**发行日期**： 2025年4月29日


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
<p>呼叫中心渠道现在可在Campaign Web用户界面中使用。 此渠道是指用于管理和跟踪通过呼叫中心处理的通信或交互的通信方法，通常是由座席向客户或潜在客户进行的电话呼叫。</p>
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
<p>现在提供了新的规则生成器，帮助您在改进的用户界面中定义复杂的条件。 您可以根据需要从旧规则生成器切换到新规则生成器。</p>
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
<p>作为Campaign管理员，您现在可以从Campaign Web用户界面设置与外部系统的新连接。
您还可以查看、更新和管理现有的外部帐户。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#25-4-improvements}

**常规接口改进**

* 架构属性的字段说明、添加到收藏夹和值分布选项现在在用户界面中更加可见。 有关更多信息，请参阅[详细文档](../get-started/attributes.md)。
* 在界面中，现在会根据Experience League首选项中设置的主要语言显示日期和时间。 这项改进仅适用于多种语言。 要查看支持的语言的完整列表，请参阅[详细文档](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank}。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**电子邮件编辑器**：为了增强Campaign Web UI中的辅助功能，Email Designer中现在提供了两个新字段：它们对应于电子邮件内容`html`元素中的`title`元素和lang属性。 除了电子邮件正文部分中的预编译标头字段外，您还可以定义这些设置。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**架构**

* 您现在可以从Campaign Web用户界面编辑列表的临时架构。 有关更多信息，请参阅[详细文档](../audience/manage-audience.md)。
* 您现在可以在示例屏幕中预览架构的自定义字段。 有关更多信息，请参阅[详细文档](../administration/custom-fields.md#add)。
* 您现在可以使用拖放操作移动列表中的自定义字段。 有关更多信息，请参阅[详细文档](../administration/custom-fields.md#add)。


### 有限可用性版本中的新功能 {#25-4-features-la}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。它们仅限于将&#x200B;**从Adobe Campaign Standard迁移到Adobe Campaign v8**&#x200B;的客户，不能在任何其他环境中部署。 它们需要将Campaign服务器升级到v8.7.4。
>
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8](../rn/acs-migration.md) 以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html)。

* **创建多语言投放** — 您现在可以在Adobe Campaign Web用户界面中以不同语言发送多个电子邮件投放。 利用多语言投放功能，可选择投放的默认语言以及可发送投放的不同语言。 您也可以使用所选的语言预览这些投放。 有关更多信息，请参阅[详细文档](../email/edit-content.md)。

* **多语言的动态报告** — 动态报告现在可用于多语言电子邮件投放。 有关更多信息，请参阅[详细文档](../reporting/global-reports.md)。

* **SMS REST API支持(LA)** — 事务性消息传递REST API现在可用于SMS渠道。 当有效负载中同时存在电子邮件和手机时，您可以使用“widedChannel”字段指定渠道。 如果未提供，则默认使用电子邮件，除非wisdedChannel明确请求短信。 有关更多信息，请参阅[详细文档](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}。

