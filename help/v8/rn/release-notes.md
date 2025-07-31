---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 58%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

以前版本中可用的更改和改进列在[2024](release-notes-24.md)和[2025](release-notes-25.md)页中。

## 2025年7月版 {#25-7-release}

### 新增功能 {#25-7-features}

以下功能从7月版本开始可用。

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>电子邮件Designer支持自定义CSS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>设计电子邮件时，您现在可以直接在Email Designer中添加自己的自定义CSS。 此功能使您能够应用高级和特定的样式，从而更加灵活地控制内容的外观。</p>
<p>有关更多信息，请参阅<a href="../email/custom-css.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>品牌</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以创建和自定义自己的品牌，以清楚地定义您在通信中的视觉和口头身份。 借助品牌一致性分数，您可以实时收到关于内容如何反映品牌基调、风格和准则的反馈，从而帮助您在发送每条消息时始终与品牌保持一致。
</p>
<p>有关更多信息，请参阅<a href="../content/brands.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>投放警报</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>投放警报功能是一个警报管理系统，利用该系统可让一组用户自动接收包含其投放执行信息的通知。</p>
<p>有关更多信息，请参阅<a href="../msg/delivery-alerting.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>动态报告</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您现在可以访问动态报告，其中提供完全可自定义的实时报告以衡量营销活动的影响。 它增加了对轮廓数据的访问，除打开数和点击数等功能性电子邮件营销活动数据外，还支持按轮廓维度（如性别、城市和年龄）进行人口统计分析。动态报告也可用于多语言电子邮件投放和事务型消息。</p>
<p>此功能仅在需要时可用。 要获取访问权限，请联系您的Adobe代表。 您的服务器必须升级到8.8.1的最低版本。 请参阅客户端控制台<a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans" target="_blank">发行说明</a>。
<p>有关更多信息，请参阅<a href="../reporting/dynamic-reporting/get-started-reporting.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>集中化品牌化</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>您的技术管理员现在可以定义一个或多个品牌，以集中处理影响品牌识别的参数。 其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您可以创建这些品牌并将它们链接到消息或登陆页面。此配置在模板中进行管理。品牌推广选项适用于所有渠道，包括短信和直邮。</p>
<p>此功能仅在新的实施中按需提供。 要获取访问权限，请联系您的Adobe代表。 您的服务器必须升级到8.8.1的最低版本。 请参阅客户端控制台<a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans" target="_blank">发行说明</a>。
<p>有关更多信息，请参阅<a href="../administration/branding/branding-gs.md">详细文档</a>。</p>
</td>
</tr>
</tbody>
</table>

除上述功能外，本次版本还提供了一组可在客户端控制台中使用的功能：

* [新SMS发送连接器](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=zh-Hans) （FDA环境）
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=zh-Hans)（按需，FDA环境）

请参阅客户端控制台[发行说明](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans){target="_blank"}。

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=zh-Hans){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=zh-Hans) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=zh-Hans) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans){target="_blank"}.

-->

### 改进 {#25-7-improvements}

* 现在，您可以在规则生成器中直接计算每个条件和组的目标群体。 单击结果编号可查看记录的详细列表。 [了解详情](../query/build-query.md#validate-query)

* 您现在可以直接从规则生成器中编辑或删除预定义过滤器。 [了解详情](../get-started/predefined-filters.md#manage-predefined-filter)

* 配置短信投放时，在&#x200B;**短信**&#x200B;部分中，您现在可以访问&#x200B;**可选SMPP参数(TLV)**。 此参数与客户端控制台中的参数相同。 [了解详情](../advanced-settings/delivery-settings.md#sms-tab)

* 您现在可以使用iOS内容版屏幕的&#x200B;**高级设置**&#x200B;部分中提供的新&#x200B;**可用内容**&#x200B;选项在iOS上启用后台通知。 这会在`content-available:1`有效负载中添加`aps`标志。 在此页面[上了解更多](../push/content-push.md)。 另请参阅[此页面](../push/rich-push-ios.md)

* 现已提供以下登陆页面改进功能：

   * 现在，您可以在配置服务时引用默认订阅/退订登陆页面。在设计电子邮件时，如果您定义了指向该登陆页面的链接，则提交登陆页面表单的用户将会自动订阅或退订此服务。[了解更多信息](../audience/manage-services.md#create-service)
   * 登陆页面配置中的新选项允许匿名访客访问登陆页面。如果取消选择此选项，则只有已识别的用户才能访问和提交表单。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 登陆页面配置中的一个新选项允许在提交登陆页面时存储额外的内部数据。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 新选项允许将一个登陆页面用于多项服务，从而使其具有动态性。在向电子邮件添加链接时，如果您选择动态登陆页面，则可以选择任何服务。如果您选择与特定服务关联的登陆页面，则会自动使用该服务（您不能选择其他服务）。[了解更多信息](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陆页面现在支持条件内容。[了解更多信息](../landing-pages/lp-content.md)
   * 您可以将着陆页面链接至某项服务，并在用户验证该页面时发送确认消息。[了解详情](../landing-pages/lp-content.md#lp-message)
   * 您可以添加验证码，以防止机器人引发的垃圾信息和滥用行为，从而保护您的着陆页面。对于您的客户而言，这是非侵入式的，因为它不需要与客户进行任何交互，并且基于与您网站的交互。[了解详情](../landing-pages/create-lp.md#captcha)
