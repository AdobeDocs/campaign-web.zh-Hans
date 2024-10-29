---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

## 10月版 {#24-10-release}

**发行日期**：2024年10月29日

从10月版本开始，将提供以下功能和改进。

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
<p>您现在可以直接通过Adobe Campaign Web用户界面设置和管理外部帐户。 利用此新功能，可轻松配置不同类型的外部帐户，例如退回电子邮件(POP3)或执行实例。</p>
<p>有关更多信息，请参阅<a href="../administration/external-account.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>事务性消息传递</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以在Campaign Web用户界面中创建和监控事务型消息。 事务性消息传递是Adobe Campaign中用于处理触发消息的专用模块。 这些消息是响应来自信息系统的事件自动生成的。 此类事件的常见示例包括单击按钮或链接、放弃购买、请求产品可用性警报、创建或修改帐户等。</p>
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

* **工作流活动** — 您现在可以将活动及其所有子节点从过渡移动到工作流中的另一个过渡。 活动的属性窗格中提供了专用的&#x200B;**移动**&#x200B;按钮来执行此操作。 [了解详情](../workflows/orchestrate-activities.md#move)

* **工作流扩充活动**

   * 在&#x200B;**扩充**&#x200B;活动中创建新字段时，您现在可以定义别名和标签。 [了解详情](../workflows/activities/enrichment.md#collection-settings)
   * 您现在可以在&#x200B;**扩充**&#x200B;活动中为每个配置文件添加优惠。 [了解详情](../workflows/activities/enrichment.md##add-offers)

* **值的分布**：当访问个性化字段列表时，您现在可以检查每个字段的值是如何分布的。专用的弹出窗口显示每个值的数字和百分比。[了解详情](../query/build-query.md#distribution-values-query)


## 9 月更新 {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI 助手内容加速器</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>完成消息制作和定制后，可使用Adobe Campaign Web中的AI助理内容加速器将其提升到新的级别。 使用这一功能强大的工具，您可以生成一系列引人入胜的文本、主标题以及在视觉上富有吸引力的图像来优化内容的影响力。</p>
<p>通过<a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">我们的实时功能预览</a>，享受沉浸式的实践体验，让您亲自探索其功能并充分了解其能力</a>。</p>
<p>有关更多信息，请参阅<a href="../email/generative-gs.md">详细文档</a>。</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>发行日期：9 月 12 日</p>
</td>
</tr>
</tbody>
</table>

## 8月版 {#24-8-release}

**发布日期**：2024 年 9 月 3 日

自 8 月版本开始提供以下功能和改进。

* **SMTP 参数** - SMTP 设置现在可在电子邮件传递设置中使用。[了解详情](../advanced-settings/delivery-settings.md#smtp)

* **全局变量** - 您现在可以定义全局变量来定义您的交付的值。[了解详情](../advanced-settings/delivery-settings.md#variables-delivery)

### 有限可用性版本中的新功能 {#acs-24-8}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。
>
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8 ](../rn/acs-migration.md)以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}。

* **直邮的品牌化**：您的技术管理员现在可以定义一个或多个品牌，以便集中管理影响品牌标识的参数。其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您现在可以创建这些品牌并将它们链接到消息或登陆页面。此配置在模板中进行管理。[了解详情](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/branding/branding-assign)

* **带有登陆页面的订阅** - 您现在可以将登陆页面链接到服务，并在用户验证时发送确认消息。[了解详情](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **视觉片段**：您现在可以对视觉内容片段进行存档。[了解详情](../content/create-fragment.md#archive)

* **登陆页面中的验证码**：您现在可以使用 Google reCAPTCHA 机制保护您的登陆页面免受机器人造成的垃圾邮件和滥用的影响。对于您的客户而言，这是非侵入式的，因为它不需要与客户进行任何交互，并且基于与您网站的交互。[了解详情](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
