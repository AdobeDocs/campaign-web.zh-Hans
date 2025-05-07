---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: ht
source-wordcount: '689'
ht-degree: 100%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 中列出了以前版本中的变更和改进。

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

* **SMS REST API 支持 (LA)** - 事务性消息传递 REST API 现可用于 SMS 渠道。当负载中同时存在电子邮件和移动电话时，您可以使用“wishedChannel”字段来指定渠道。如果未提供，则默认使用电子邮件，除非 wishedChannel 明确请求 SMS。有关更多信息，请参阅[详细文档](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}。

