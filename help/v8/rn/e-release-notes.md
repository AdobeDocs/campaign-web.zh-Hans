---
title: Campaign v8 Web 用户界面早期发行说明
description: 了解下一版 Campaign Web 用户界面的新功能
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 126ebed5066bbc8c20d58d24e237b13f096b9d02
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 32%

---

# 早期发行说明 {#e-release}

Adobe Campaign Web 用户界面不断地提供新功能、对现有功能进行增强和修复错误。所有更改会在每月的最后整合到[发行说明](release-notes.md)中。

**以下早期发行说明在发行可用日期之前如有更改，恕不另行通知**。链接、屏幕和更新的文档会于发布日期在[发行说明](release-notes.md)中发布。

## 2025年1月版 {#25-1-release}

**发行日期**：2025年2月5日

从1月版本开始，将提供以下功能和改进。

### 功能 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>创建和使用可视化片段</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>可视化片段是预定义的可视化块，您可以在多个电子邮件投放中或在内容模板中重复使用。 此功能现在适用于在服务器版本8.6.4及更高版本上运行的所有客户。</p>
<p>有关更多信息，请参阅<a href="../content/use-visual-fragments.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>使用第三方系统发送投放</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在Campaign Web用户界面中定义外部投放和外部投放模板。 在这种模式下，输入文件中会生成消息，并可以与外部提供商共享。外部投放模式是直邮渠道的默认模式。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>控制和过滤带有类型的投放发送</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>现在，您可以在Adobe Campaign Web用户界面中创建分类和分类规则。 类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。分类验证投放始终包含所需的元素（如退订链接或主题行），或者用于从预期目标中排除分组（如取消订阅者、竞争对手或不忠诚客户）的筛选规则。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>管理您的明细列表</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>现在，您可以直接通过Adobe Campaign Web用户界面创建明细列表。 枚举是系统建议用于填充字段的值列表。 使用枚举来标准化这些字段的值，帮助在查询中输入或使用数据。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
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
<p>您现在可以访问Adobe Campaign Web用户界面中的技术选项，并根据自己的需求创建自定义选项。 在使用JavaScript代码工作流活动存储中间数据时，这尤其有用。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>定义和调用Javascript代码</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在Adobe Campaign Web用户界面中创建JavaScript代码。 这允许您创建可重复使用的功能，这些功能可在多个工作流中使用，类似于库。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#25-1-improvements}

* 自定义界面中自定义字段的显示：

   * 您现在可以选择要在界面中显示的其他自定义字段
   * 您现在可以设置用于显示链接类型自定义字段的规则，例如基于其他字段的输入来限制列表值
   * 您现在可以更灵活地排列界面中的字段：字段可以跨越一列，或者分组到子部分中以更好地组织
   * 您现在可以将特定字段设置为只读。

* 最近和收藏夹过滤器：要快速重用经常使用的属性，您现在可以将它们添加到收藏夹。 这可以确保将来任务可以随时访问它们。 除了收藏夹之外，您还可以查看和使用最近选定的属性。


