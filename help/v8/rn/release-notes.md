---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

## 8月发行说明 {#24-8-release}

**发行日期**： 2024年9月3日

从8月版本开始，将提供以下功能和改进。

* **值分布** — 访问个性化字段列表时，现在可以检查每个字段值的分布方式。 专用弹出窗口显示每个值的数量和百分比。 [了解详情](../query/build-query.md#distribution-values-query)

* **SMTP参数** - SMTP设置现在可在电子邮件投放设置中使用。 [了解详情](../advanced-settings/delivery-settings.md#smtp)

* **全局变量** — 您现在可以定义全局变量来定义投放的值。 [了解详情](../advanced-settings/delivery-settings.md#variables-delivery)

### 有限可用性版本中的新功能 {#acs-24-8}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。
>
>请参阅以下文档页面：[Campaign Standard过渡到Campaign v8](../rn/acs-migration.md)以及Campaign Standard用户的[功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-hans){target="_blank"}。

* **直邮品牌** — 技术管理员现在可以定义一个或多个品牌以集中影响品牌识别的参数。 其中包括品牌徽标、登陆页面访问 URL 的域名或消息跟踪设置。您现在可以创建这些品牌，并将它们链接到消息或登陆页面。 此配置在模板中进行管理。[了解详情](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **具有登陆页面的订阅** — 您现在可以将登陆页面链接到服务，并在用户验证服务时发送确认消息。 [了解详情](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **可视片段** — 您现在可以将可视内容片段存档。 [了解详情](../content/create-fragment.md#archive)

* **登陆页面中的验证码** — 您现在可以添加验证码以保护登陆页面免受机器人程序造成的垃圾邮件和滥用。 对于您的客户而言，这是非侵入式的，因为它不需要与客户进行任何交互，并且基于与您网站的交互。[了解详情](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
