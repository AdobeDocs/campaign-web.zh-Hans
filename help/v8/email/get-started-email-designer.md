---
audience: end-user
title: 编辑电子邮件内容
description: 了解如何使用 Campaign Web 用户界面中的电子邮件设计器开始构建内容
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: 9ec5483a5253d67110baf6a51b47ebe0c27574d5
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 99%

---

# 电子邮件设计器入门 {#get-started-email-designer}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="新的电子邮件设计器"
>abstract="利用营销活动电子邮件设计器，可通过直观的拖放界面创建令人着迷、个别定制的电子邮件。无论是从头开始、导入现有内容还是利用现有模板，均可设计并细化每封电子邮件的所有内容！"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="请参阅发行说明"

在 Adobe Campaign 中创建电子邮件后，您需要定义其内容。

利用电子邮件设计器，可以通过直观的拖放界面创建迷人的、单独定制的电子邮件。无论您是从头开始，导入现有内容还是利用现有模板，请设计并优化每封电子邮件的所有内容（无论促销还是事务电子邮件均如此）。

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* 使用 [!DNL Campaign] 电子邮件设计功能可轻松生成响应式电子邮件。[了解详情](create-email-content.md)

* 通过根据客户的配置文件属性创建个性化内容来提升客户体验。[了解详情](../personalization/personalize.md)

* 配置条件内容字段以根据收件人的配置文件创建动态个性化内容。[了解详情](../personalization/conditions.md)

## 电子邮件设计最佳实践 {#best-practices}

在发送电子邮件时，请务必考虑到收件人可能会转发它们，而这有时会导致电子邮件的呈现出现问题。当用于转发的电子邮件提供商无法支持所使用的 CSS 类时尤为如此，例如，如果您使用“is-desktop-hidden”CSS 类来隐藏移动设备上的图像。

为了最大限度地减少这些呈现问题，我们建议尽可能使电子邮件设计结构变得简单。尝试使用适用于桌面和移动设备的单一设计，同时避免使用复杂的 CSS 类或其他并非所有电子邮件客户端都完全支持的设计元素。通过遵循这些最佳实践，您可以帮助确保始终如一地正确呈现电子邮件，无论收件人如何查看或转发它们。

## 开始创作内容 {#start-authoring}

从电子邮件投放仪表板中，通过[编辑内容](edit-content.md)屏幕打开电子邮件设计器主页。在该主页中，从以下选项中选择所需的电子邮件设计方式：

* 通过电子邮件设计器界面&#x200B;**从头开始设计电子邮件**。请参阅[此章节](create-email-content.md)以了解如何设计电子邮件内容。

* 直接在电子邮件设计器中&#x200B;**编写或粘贴原始 HTML**。请参阅[此章节](code-content.md)以了解如何编写您自己的内容代码。

* 从文件或 .zip 文件夹中&#x200B;**导入现有 HTML 内容**。请参阅[此章节](existing-content.md)以了解如何导入电子邮件内容。

* 从内置或自定义模板的列表中&#x200B;**选择现有内容**。请参阅此[章节](create-email-templates.md)以了解如何使用电子邮件模板。

  ![](assets/email_designer_create_options.png){zoomable=&quot;yes&quot;}
