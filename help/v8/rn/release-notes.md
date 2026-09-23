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
source-git-commit: 73553f19c6e88256f0e9f38479bdfc292a3221f8
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。 我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

## 2026年9月版 {#26-9-release}

_2026年9月22日_

### 新增功能 {#26-9-features}

<table>
<thead>
<tr>
<th><strong>LINE 渠道</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign现在支持<strong>LINE</strong>渠道，这是一个常用的即时消息应用程序。 使用文本、图像或视频内容，在独立投放或工作流中，以及其他渠道旁创建和发送LINE消息。 <a href="../line/get-started-line.md">了解更多信息</a></p>
</td>
</tr>
</tbody>
</table>

### 改进 {#26-9-improvements}

* **侧面导航访问**：管理员现在可以在侧面导航中隐藏特定的菜单项。 [了解更多](../administration/schemas-browse-access.md#screen-def)
* **其他审批类型**：除了内容和目标审批之外，您现在还可以要求对Campaign投放进行预算和投放开始审批。 [了解更多](../campaigns/campaign-approvals.md#configure-approvals)
* **基于访客的短信定位**：访客目标映射现在可用于短信投放。 [了解更多](../sms/create-sms.md)
* **工作流取消按钮**：新的&#x200B;**取消**&#x200B;按钮允许您还原工作流中未保存的更改。 [了解更多](../workflows/orchestrate-activities.md#save-cancel)
* **带多个值的重复数据删除**： **Follow值列表**&#x200B;选项现在支持多个属性。 [了解更多](../workflows/activities/deduplication.md#deduplication-configuration)
* **移动设备目标映射**：您现在可以为移动设备应用程序目标创建目标映射。 [了解更多](../administration/target-mappings.md#create-mapping)
* **外部数据库扩充**：您现在可以在&#x200B;**扩充**&#x200B;或&#x200B;**生成受众**&#x200B;活动中扩充外部数据库中的数据。 [了解更多](../workflows/activities/enrichment.md#external-data)
* **文件受众协调**：现在，您可以配置在从文件定位受众时是否将收件人导入数据库。 [了解更多](../audience/file-audience.md#upload)
* **集合上的直接联接**：直接从集合中选择属性时，现在可以选择如何构建条件：使用推荐的默认选项、聚合函数或高级直接联接。 [了解更多](../query/build-query.md#links)

