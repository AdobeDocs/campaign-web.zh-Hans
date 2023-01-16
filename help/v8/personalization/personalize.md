---
title: 在Campaign中个性化您的内容
description: 了解如何在Adobe Campaign Web UI中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 46d8ac555e554faef91bcc817890466780387d0d
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# 个性化您的内容{#add-personalization}

![](../assets/do-not-localize/badge.png)

您可以通过以下方式个性化消息内容：

* 插入动态 **个性化字段**

   个性化字段用于消息的一级个性化。 您可以从个性化编辑器中选择数据库中可用的任何字段。 对于投放，您可以选择与收件人、消息或投放相关的任何字段。 这些个性化属性可插入到邮件的主题行或正文中。

   ![](assets/perso-subject-line.png)

   以下语法可在内容中插入收件人的城市：&lt;%= recipient.location.city %>。

* 插入预定义 **内容块**

   Campaign附带一组个性化块，其中包含可插入投放的特定渲染。 例如，您可以添加徽标、问候语消息或指向消息镜像页面的链接。 内容块可从个性化编辑器中的专用条目中使用。

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## 个性化电子邮件主题行 {#personalize-subject-line}

在 **[!UICONTROL 主题行]** 字段，请执行以下步骤：

1. 单击 **打开个性化对话框** 图标 **主题行** 字段。
1. 输入主题行内容并选择要添加的个性化属性。
1. 单击 **确认** 验证。 个性化属性会添加到主题行。

![](assets/perso-subject.png)

## 个性化电子邮件内容 {#personalize-emails}

要个性化电子邮件内容，请在电子邮件设计器中打开该消息，然后：

1. 在文本块内单击。
1. 在上下文工具栏中，选择 **添加个性化**.

   ![](assets/perso-add-to-content.png)

1. 在个性化编辑器中插入收件人的名称并进行确认。

   ![](assets/perso-add-name.png)

   个性化属性会添加到电子邮件内容中。

   您可以模拟内容以检查呈现。 [了解详情](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

要向电子邮件添加内容块，请应用相同的步骤，然后从最后一个图标中选择一个内容块：

![](assets/perso-insert-block.png)

插入后，内容块会添加到电子邮件内容中，如下所示。 在投放准备步骤中，当生成个性化时，会自动将其调整为收件人用户档案。

![](assets/perso-content-block-in-email.png)


内置内容块包括：
* **[!UICONTROL 由Adobe Campaign启用]** :插入“Enabled by Adobe Campaign”徽标。
* **[!UICONTROL 专有名词的格式功能]** :生成 **[!UICONTROL toSmartCase]** Javascript函数，该函数将每个单词的第一个字母更改为大写。
* **[!UICONTROL 问候语]** :插入带有收件人姓名的问候语。 示例：“你好，无名氏”。
* **[!UICONTROL 插入徽标]** :插入配置实例时定义的现成徽标。
* **[!UICONTROL 链接到镜像页面]** :插入指向镜像页面的链接：“如果您无法正确查看此消息，请单击此处”。
* **[!UICONTROL 镜像页面URL]** :插入镜像页面URL，使交付设计人员能够检查该链接。
* **[!UICONTROL 统一模式下的优惠接受URL]** :插入一个URL，以便将交互选件设置为 **[!UICONTROL 已接受]**.
* **[!UICONTROL 注册页面URL]** :插入订阅URL。
* **[!UICONTROL 注册链接]** :插入订阅链接。 配置实例时必须定义此链接。 默认内容为：“若要注册，请单击此处。”
* **[!UICONTROL 注册链接（带反向链接）]** :插入订阅链接，以识别访客和投放。 配置实例时已定义链接。
* **[!UICONTROL 注册确认]** :插入用于确认订阅的链接。
* **[!UICONTROL 社交网络共享链接]** :插入使收件人能够共享指向镜像页面内容的链接的按钮。
* **[!UICONTROL 内容电子邮件的样式]** 和 **[!UICONTROL 通知样式]** :生成代码，以使用预定义的HTML样式设置电子邮件的格式。
* **[!UICONTROL 退订链接]** :插入一个链接，以取消所有投放的订阻止列表阅()。 默认关联内容为：“您收到此邮件是因为您与 `<your rganization name>` 或关联。 不再从接收消息 `<your rganization name>` 单击此处。”


## 个性化电子邮件中的链接 {#personalize-links}

个性化 **链接**:

1. 选择文本块或图像。
1. 在上下文工具栏中，选择 **插入链接**.

   ![](assets/perso-link.png)

1. 输入链接标签，然后使用 **插入链接** 按钮以个性化链接。

   ![](assets/perso-link-insert-icon.png)

1. 使用个性化编辑器定义和个性化链接，并进行确认。

   ![](assets/perso-link-edit.png)


## 个性化您的选件 {#personalize-offers}

在将文本类型内容添加到选件的表示时，您还可以访问个性化编辑器。 在 [此部分](../content/offers.md).
