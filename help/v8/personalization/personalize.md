---
title: 在Campaign中个性化您的内容
description: 了解如何在Adobe Campaign Web UI中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 2d23b04b81ab625de0936fdf058f6ac8bd1017c3
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# 个性化您的内容{#add-personalization}

![](../assets/do-not-localize/badge.png)

您可以通过以下方式个性化消息内容：

* 插入动态 **个性化字段**

   个性化字段用于消息的一级个性化。 您可以从个性化编辑器中选择数据库中可用的任何字段。 对于投放，您可以选择与收件人、消息或投放相关的任何字段。 这些个性化属性可插入到消息的主题行或正文中。

   ![](assets/perso-subject-line.png)

   上述语法可在内容中插入收件人的城市：&lt;%= recipient.location.city %>。

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
1. 单击确认以验证。 个性化属性会添加到主题行。

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


## 个性化电子邮件中的链接 {#personalize-links}

个性化 **链接**:

1. 选择文本块或图像。
1. 在上下文工具栏中，选择 **添加个性化**.

   ![](assets/perso-link.png)

1. 使用个性化编辑器定义和个性化链接。

## 个性化您的选件 {#personalize-offers}

在将文本类型内容添加到选件的表示时，您还可以访问个性化编辑器。
