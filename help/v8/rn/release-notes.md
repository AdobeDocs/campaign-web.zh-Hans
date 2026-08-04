---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 29%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。 我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

## 2026年7月版 {#26-7-release}

_2026年7月28日_

### 新增功能 {#26-7-features}

<table>
<thead>
<tr>
<th><strong>产品建议管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以直接从Campaign Web用户界面端到端地管理选件。 配置优惠环境和优惠空间，构建优惠目录和类别，创建具有资格规则和优先级权重的优惠，并批准和部署它们以供在投放中使用。 高级配置在Client Console中仍然可用。</p>
<p>有关更多信息，请参阅<a href="../offers/gs-offer-management.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>品牌配置</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>现在，技术管理员可以直接从Campaign Web用户界面创建和配置品牌，而无需使用客户端控制台。 所有品牌设置（包括标识、子域和协议、电子邮件标头参数以及URL跟踪参数）现在均可在Web UI中使用。</p>
<p>有关更多信息，请参阅<a href="../administration/branding/branding-configure.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>电子邮件Designer中的公共资源</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>将图像添加到电子邮件时，您现在可以选择<strong>公共资源</strong>。 这允许您选择在Adobe Campaign实例上已可用的图像，例如之前在Email Designer中导入的文件或从Client Console上传的公共资源。</p>
<p>有关更多信息，请参阅<a href="../email/content-components.md#image">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>数据加载(RDBMS)工作流活动</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>数据加载(RDBMS)</strong>活动现在可在Campaign Web用户界面中使用。 使用此活动将数据直接从外部关系数据库加载到工作流中。 提取的数据将在整个工作流中可用，可用于目标定位、数据扩充或进一步的数据处理。</p>
<p>有关更多信息，请参阅<a href="../workflows/activities/data-loading-rdbms.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>动态 JavaScript 页面</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>动态 JavaScript 页面 (JSSP) 可用于构建服务器端页面，当通过 URL 访问时生成动态内容，例如自定义 API、导出功能或 Web 应用程序逻辑。 现在，您可以直接从Campaign Web用户界面创建、修改、复制和删除这些页面。</p>
<p>有关更多信息，请参阅<a href="../administration/dynamic-javascript-pages.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-7-improvements}

* 已对&#x200B;**自定义架构配置**&#x200B;进行以下改进：
  * 新的&#x200B;**操作数据**&#x200B;部分允许您限制自定义架构记录上的可用操作，而不管单个文件夹上配置的安全规则如何。 [了解更多](../administration/schemas-action-data.md)
  * **自定义筛选器**&#x200B;已添加到&#x200B;**清单列表配置**&#x200B;部分。 它们允许您选择哪些属性在列表视图的筛选器窗格中显示为快速访问字段。 [了解更多](../administration/schemas-custom-filters.md)

* 已对&#x200B;**工作流**&#x200B;进行以下改进：
  * 现在，删除工作流活动会更加灵活：当活动具有后续活动时，您可以选择删除所有后续活动、仅删除选定活动，或者删除活动，同时将后续活动保留在新分支中。 [了解更多](../workflows/orchestrate-activities.md#delete-activity)
  * 您现在可以断开两个工作流活动之间的过渡，而无需删除其中任一活动。 例如，您可以借此重新组织工作流图，以暂时保留一组要保留的活动，而无需删除和重新创建它们。 [了解更多](../workflows/orchestrate-activities.md#disconnect-transition)
  * 现在，水平滚动条和垂直滚动条会显示在工作流画布周围，您可以通过直接拖动到要查看的区域来导航大型工作流。 [了解更多](../workflows/orchestrate-activities.md)
  * 在保存或启动/重新启动工作流时，如果自您打开工作流后其他用户在Web UI或客户端控制台中修改了该工作流，则现在会显示警告。 您可以选择覆盖其他更改，重新加载工作流以获取最新版本，或者取消。

* **发件人电子邮件地址**：您现在可以使用&#x200B;**NmsDelivery_senderAddressMask**&#x200B;选项，将投放的&#x200B;**From email**&#x200B;字段限制为预定义的地址列表。 [了解更多](../administration/options.md#restrict-sender-address)
* **登录错误消息**&#x200B;已得到改进：当登录尝试失败时，Web UI现在会针对几种情况（例如，当用户未分配安全区域或其IP地址受限制时）显示更具体的错误消息。
