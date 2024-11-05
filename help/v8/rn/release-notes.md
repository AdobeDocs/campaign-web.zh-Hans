---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

[本页](release-notes-24.md)列出了以前版本中的变更和改进。

## 2024 年 10 月版本 {#24-10-release}

**发行日期**：2024 年 10 月 29 日

自 10 月版本开始提供以下功能和改进。

### 功能

<table>
<thead>
<tr>
<th><strong>外部帐户</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接通过 Adobe Campaign Web 用户界面设置和管理外部帐户。此新功能可以轻松配置不同类型的外部帐户，例如退回电子邮件（POP3）或执行实例。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>交易型消息传递</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>交易消息传递（消息中心）现已在 Campaign 网络用户界面中提供。此附加组件用于触发由信息系统触发的事件生成的消息，可以是：发票、订单确认、发货确认、密码更改、产品不可用通知、帐户报表、网站帐户创建等等。</p>
<p>有关更多信息，请参阅<a href="../transactional-messaging/transactional.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### 改进

* **工作流活动** - 您现在可以将活动及其所有子节点从工作流中的一个过渡移动到另一个过渡。活动的属性窗格中有一个专用的 **移动** 按钮可以执行此操作。[了解详情](../workflows/orchestrate-activities.md#move)

* **工作流扩充活动**

   * 现在，您可以在 **扩充** 活动中创建新字段时定义别名和标签。[了解详情](../workflows/activities/enrichment.md#collection-settings)
   * 您现在可以在 **扩充** 活动中为每个轮廓添加产品建议。[了解详情](../workflows/activities/enrichment.md##add-offers)

* **值的分布**：当访问个性化字段列表时，您现在可以检查每个字段的值是如何分布的。专用的弹出窗口显示每个值的数字和百分比。[了解详情](../query/build-query.md#distribution-values-query)

* **版本和系统信息** - 您现在可以访问有关实例版本的详细信息，包括客户端控制台和 Web 用户界面。此新部分还列出了您的环境中安装的所有内置包。[了解详情](../get-started/user-interface.md#user-interface-about)

* **列表** - 您现在可以轻松地重新排序列表的值。[了解详情](../get-started/work-with-folders.md)

* **交付** - 现在可以从个性化字段访问交付变量。[了解详情](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)