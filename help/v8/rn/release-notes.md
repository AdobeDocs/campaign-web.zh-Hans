---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62294ce1809caee8af770b376aad97bac71c942c
workflow-type: ht
source-wordcount: '688'
ht-degree: 100%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

[2024](release-notes-24.md) 和 [2025](release-notes-25.md) 中列出了以前版本中的变更和改进。

## 7 月 25 日更新 {#25-7-updates}

>[!AVAILABILITY]
>
>要使用这些更新，您的服务器版本需至少升级至 8.8.1。请参阅客户端控制台[发行说明](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans){target="_blank"}。

以下功能此前已在有限可用性阶段发布，现在已面向所有环境全面开放（正式发布）：

* **创建多语言投放** - 您现在可以在 Adobe Campaign Web 用户界面中使用不同语言发送多个电子邮件投放。多语言投放功能允许您选择投放的默认语言以及可以发送投放的不同语言。您还可以使用您选择的语言预览这些投放内容。[了解更多信息](../email/edit-content.md#multilingual-delivery)。

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=zh-Hans){target="_blank"}
-->

* **投放提醒**——投放提醒功能是一个提醒管理系统，利用该系统可让一组用户自动接收包含其投放执行信息的通知。[了解更多信息](../msg/delivery-alerting.md)

* **登陆页面改进** - 以下着陆页面相关的改进功能现已推出：

   * 现在，您可以在配置服务时引用默认订阅/退订登陆页面。在设计电子邮件时，如果您定义了指向该登陆页面的链接，则提交登陆页面表单的用户将会自动订阅或退订此服务。[了解更多信息](../audience/manage-services.md#create-service)
   * 登陆页面配置中的新选项允许匿名访客访问登陆页面。如果取消选择此选项，则只有已识别的用户才能访问和提交表单。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 登陆页面配置中的一个新选项允许在提交登陆页面时存储额外的内部数据。[了解更多信息](../landing-pages/create-lp.md#create-landing-page)
   * 新选项允许将一个登陆页面用于多项服务，从而使其具有动态性。在向电子邮件添加链接时，如果您选择动态登陆页面，则可以选择任何服务。如果您选择与特定服务关联的登陆页面，则会自动使用该服务（您不能选择其他服务）。[了解更多信息](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * 登陆页面现在支持条件内容。[了解更多信息](../landing-pages/lp-content.md)
   * 您可以将着陆页面链接至某项服务，并在用户验证该页面时发送确认消息。[了解详情](../landing-pages/lp-content.md#lp-message)
   * 您可以添加验证码，以防止机器人引发的垃圾信息和滥用行为，从而保护您的着陆页面。对于您的客户而言，这是非侵入式的，因为它不需要与客户进行任何交互，并且基于与您网站的交互。[了解详情](../landing-pages/create-lp.md#captcha)

以下功能此前在有限可用性阶段发布，现在已可&#x200B;**按需**&#x200B;使用：

* **动态报告** - 您现在可以使用动态报告功能，提供完全可自定义且实时更新的报告，以衡量您的营销活动成效。它增加了对轮廓数据的访问，除打开数和点击数等功能性电子邮件营销活动数据外，还支持按轮廓维度（如性别、城市和年龄）进行人口统计分析。动态报告现也适用于多语言电子邮件投放和事务性消息。[了解更多信息](../reporting/dynamic-reporting/get-started-reporting.md)

* **集中式品牌管理** -  您的技术管理员现在可以定义一个或多个品牌，以集中管理影响品牌标识的各项参数。其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您可以创建这些品牌并将它们链接到消息或登陆页面。此配置在模板中进行管理。品牌化选项现在可用于所有渠道，包括短信和直邮。[了解更多信息](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >此功能仅适用于新部署的实施方案。

除上述功能外，本次版本还提供了一组可在客户端控制台中使用的功能：

* [新增 SMS 发送连接器](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=zh-Hans)。
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=zh-Hans)

请参阅客户端控制台[发行说明](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans){target="_blank"}。

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=zh-Hans){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->