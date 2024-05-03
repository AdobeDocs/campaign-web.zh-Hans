---
title: 最新发行说明
description: 发现 Campaign Web 用户界面附带的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f6a1ebcb5a77798f738e2a4ac0b45454d941d7c7
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 25%

---

# 发行说明 {#latest-release}

<!--Last update: **March 19, 2024**-->

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

## 4月发行说明 {#april-24-4-release}

**发行日期**：2024年5月2日

### 新增功能 {#new-24-4}

从4月版开始，所有用户都可以使用以下功能。

**新的工作流活动**

* **更新数据**  — 使用此活动对数据库中的字段执行批量更新。 您可以通过多个选项将数据更新个性化。 [了解更多信息](../workflows/activities/update-data.md)
* **订阅服务**  — 使用此活动可在单次操作中订阅或退订多个用户档案加入/退出服务。 [了解更多信息](../workflows/activities/subscription-services.md)
* **提取文件**  — 使用此活动将数据从Adobe Campaign作为外部文件导出到其他系统。 [了解更多信息](../workflows/activities/extract-file.md)
* **传输文件**  — 使用此活动接收或发送文件、测试文件是否存在或列出服务器上的文件。 使用的协议可以是服务器到服务器协议或HTTP协议。 [了解更多信息](../workflows/activities/transfer-file.md)
* **测试**  — 使用此活动可根据指定的条件启用过渡。 [了解更多信息](../workflows/activities/test.md)
* **JavaScript代码**  — 使用此活动可在工作流上下文中执行JavaScript代码片段。 [了解更多信息](../workflows/activities/javascript-code.md)
* **外部信号**  — 使用此活动触发从另一个工作流执行的工作流或API调用。 [了解更多信息](../workflows/activities/external-signal.md)
* **增量查询**  — 使用此活动按计划查询数据库。 每次执行此活动时，都会排除先前执行得出的结果。这样可让您仅定向新元素。 [了解更多信息](../workflows/activities/incremental-query.md)

**富推送通知模板**

您现在可以通过Android发送富推送通知。 富推送通知是移动通知的一种增强形式，它通过合并多媒体元素（如图像、交互式按钮或其他富媒体内容）而超出简单的文本消息。 [了解更多信息](../push/rich-push.md)

请注意，此功能位于 **有限可用性** （洛杉矶）。

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### 限量发布中的新增功能 {#acs-24-4}

>[!AVAILABILITY]
>
>以下功能在有限可用性(LA)中提供。 它们仅限于迁移的客户 **从Adobe Campaign Standard到Adobe Campaign v8**&#x200B;和无法部署在任何其他环境中。
>
>请参阅以下文档页面： [Campaign Standard过渡到Campaign v8](../rn/acs-migration.md) 和 [面向Campaign Standard用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **品牌化**  — 作为Campaign Standard迁移的用户，您的技术管理员现在可以定义一个或多个品牌，以集中处理影响品牌识别的参数。 其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您可以创建这些品牌并将它们链接到消息或登陆页面。 此配置在模板中进行管理。 [了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest API**  — 作为Campaign Standard迁移用户，您可以使用Rest API为Adobe Campaign创建集成，并通过将Adobe Campaign与您使用的技术面板连接来构建您自己的生态系统。 [了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **动态报告**  — 作为Campaign Standard迁移的用户，您可以访问动态报表，其中提供完全可自定义的实时报表以衡量营销活动的影响。 它增加了对用户档案数据的访问权限，从而除了功能电子邮件促销活动数据（如打开数和点击数）之外，还可按用户档案维度（如性别、城市和年龄）进行人口统计分析。 [了解更多信息](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **登陆页面**  — 以下对登陆页面的改进仅适用于从Campaign Standard过渡的用户：

   * 现在，在配置服务时，您可以引用默认订阅/退订登陆页面。 设计电子邮件时，如果您定义指向该登陆页面的链接，则提交登陆页面表单的用户将自动订阅或取消订阅此服务。 [了解更多信息](../audience/manage-services.md#create-service)
   * 登陆页面配置中的新选项允许匿名访客访问登陆页面。 如果取消选择此选项，则只有已识别的用户才能访问和提交表单。 [了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 登陆页面配置中的新选项允许在提交登陆页面时存储其他内部数据。 [了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 通过新选项，可以将登陆页面用于多项服务，使其成为动态页面。 将链接添加到电子邮件时，如果您选择了动态登陆页面，则可以选择任何服务。 如果选择关联了特定服务的登陆页面，则将自动使用此服务（您无法选择其他服务）。 [了解更多信息](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 现在，登陆页面支持条件内容。 [了解更多信息](../landing-pages/lp-content.md)

### 一般改进 {#improvements-24-4}

从4月版开始，所有客户都可以获得以下改进。
<!--**Workflow - Copy/Paste into another tab**: -->

* 此 **加载文件** 增强了活动，提供了多个部分来上传样例文件、管理错误和拒绝以及在执行活动后删除上传的文件。 [了解更多信息](../workflows/activities/load-file.md)


* 您现在可以 **复制/粘贴活动** 从不同的浏览器选项卡将访客从某个工作流转到另一个工作流。 [了解更多信息](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* 现在，所有工作流活动都允许您管理其 **执行选项**. 这让您能够定义活动的执行模式和出现错误时的行为。 [了解更多信息](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* 中的“如果群体为空，则不激活过渡”选项 **拆分活动** 允许您选择当区段结果为空时，工作流是否应过渡到下一个活动。 [了解更多信息](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **自定义字段** 是通过Adobe Campaign控制台添加到现成模式的其他属性。 在Campaign Web用户界面中，这些自定义字段现在可在各种屏幕中看到，例如用户档案或测试用户档案的详细信息。 在Web用户界面中，无法创建自定义字段，但现在可以修改其显示方式。 [了解更多信息](../administration/custom-fields.md)


## 3 月发行说明 {#24-3-release}

>[!AVAILABILITY]
>
>此版本适用于所有 [Campaign（控制台）v8.6 及更高版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans)的用户。请参阅 [Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hans){target="_blank"}，了解有关 Adobe Campaign 客户端控制台版本和升级的更多信息。

**发布日期**：2024 年 3 月 19–20 日

### 直邮渠道 {#24-3-dm}

**直邮**&#x200B;渠道现在既可在工作流中使用，也可独立投放。直邮是一种离线渠道，允许您创建和生成提取文件、进行个性化设置，并与直邮提供商共享，向客户发送邮件。

### 新的更改数据源工作流活动 {#24-3-change-data-source}

**更改数据源**&#x200B;定位活动允许您更改工作流工作表使用的数据源。这项活动提供了更大的灵活性，使您可以跨不同的数据库管理数据并提高性能。

### 拆分工作流活动改进 {#24-3-split}

您现在可以使用 **在同一张表中生成所有子集** 中的选项 **Split** 工作流活动，用于将所有子集分组到单个输出转换中。

### 查询建模器 {#24-3-query-modeler}

* 查询建模器现在可在电子邮件设计器中使用。它允许您在创建条件内容时构建条件。
* 现在，创建自定义条件时，预定义值可用于日期类型属性。
* 无法再在图中的新过渡上添加运算符。它们只能在筛选组件以将它们分组到一起之前添加到现有过渡上。
