---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 100%
---
# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。 我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

## 2026 年 8 月版本 {#26-8-release}

_2026 年 8 月 18 日_

### 新增功能 {#26-8-features}

<table>
<thead>
<tr>
<th><strong>审批工作流活动</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>审批</strong>工作流活动（此前仅在客户端控制台中提供）现已在 Campaign Web 用户界面中提供。 将任务分配给组或单个操作员，自定义通知标题和消息，并将可能的答案（例如“是/否”）定义为输出分支。</p>
<p>有关更多信息，请参阅<a href="../workflows/activities/approval.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-8-improvements}

* **打开跟踪**：您现在可以直接从 Campaign Web 用户界面启用或禁用打开跟踪。 这有助于您遵守数据保护法规。 [了解更多](../advanced-settings/delivery-settings.md#tracking-tab)
* **项目列表视图**：现在，项目会在专用视图中列出，与营销活动、投放和工作流的展示方式类似。 您可以浏览现有项目并直接从此视图创建新项目。 [了解更多](../administration/plans-programs.md#create-program)
* **自定义架构配置**：在&#x200B;**操作数据**&#x200B;部分中，您现在可以禁止对自定义架构的记录执行&#x200B;**复制**&#x200B;操作。 [了解更多](../administration/schemas-action-data.md#action-data)
* **自定义过滤器**：在架构编辑器中，您现在可以使用新的&#x200B;**链接设置**&#x200B;对话框限制链接类型自定义过滤器的选取器中可用的值。 [了解更多](../administration/schemas-custom-filters.md#settings)
* **架构验证**：您现在可以使用新的&#x200B;**检查**&#x200B;按钮，直接从架构编辑器验证架构的结构。 [了解更多](../administration/schemas-create-publish.md#create-new)
* **文件夹安全性**：现在，文件夹上可执行的操作统一受操作员的权限管控，与客户端控制台的行为保持一致。 [了解详情](../get-started/work-with-folders.md#about-folders)。
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->

