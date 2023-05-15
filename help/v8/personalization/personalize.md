---
title: 在 Campaign 中个性化您的内容
description: 了解如何在 Adobe Campaign Web UI 中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 05d87fc9ff8f5e2038eba4cc9438e058566e04c8
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 95%

---


# 个性化您的内容{#add-personalization}

可以通过以下方式个性化邮件内容：

* 插入动态&#x200B;**个性化字段**

   个性化字段用于邮件的第一级个性化。您可以从个性化编辑器中选择数据库中可用的任何字段。对于投放，您可以选择与收件人、邮件或投放相关的任何字段。可将这些个性化属性插入邮件的主题行或正文中。

   ![](assets/perso-subject-line.png)

   以下语法可在您的内容中插入收件人的城市：&lt;%= recipient.location.city %>。

* 插入预定义的&#x200B;**内容块**

   Campaign 附带了一组个性化块，其中包含可插入投放中的特定渲染。例如，您可以添加徽标、问候邮件或指向邮件的镜像页面的链接。可以从个性化编辑器的专用条目中获得内容块。

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->


内置内容块为：

* **[!UICONTROL 由 Adobe Campaign 启用]**：插入“由 Adobe Campaign 启用”徽标。
* **[!UICONTROL 专有名词的格式化函数]**：生成 **[!UICONTROL toSmartCase]** Javascript 函数，它将每个单词的首字母更改为大写形式。
* **[!UICONTROL 问候]**：插入带收件人全名的问候语，后跟一个逗号。示例：“Hello John Doe,”。
* **[!UICONTROL 插入徽标]**：插入在实例设置中定义的徽标。
* **[!UICONTROL 指向镜像页面的链接]**：插入指向[镜像页面](../content/mirror-page.md)的链接。默认格式为：“如果您无法正确查看此邮件，请单击此处”。
* **[!UICONTROL 镜像页面 URL]**：插入镜像页面 URL，以便投放设计人员能够检查链接。
* **[!UICONTROL 单一模式下的优惠接受 URL]**：插入一个 URL，以便将优惠设置为&#x200B;**[!UICONTROL 已接受]**。（如果启用了交互模块，则此块可用）
* **[!UICONTROL 注册确认]**：插入一个用于确认订阅的链接。
* **[!UICONTROL 注册链接]**：插入订阅链接。在实例设置中定义此链接。默认内容为：“单击此处以注册”。
* **[!UICONTROL 注册链接（带反向链接）]**：插入订阅链接，用于识别访客和投放。在实例设置中定义此链接。
* **[!UICONTROL 注册页面 URL]**：插入订阅 URL
* **[!UICONTROL 内容电子邮件的样式]**&#x200B;和&#x200B;**[!UICONTROL 通知样式]**：生成使用预定义的 HTML 样式设置电子邮件格式的代码。
* **[!UICONTROL 退订链接]**：插入一个链接，用于退订所有投放（列入阻止列表）。默认关联内容为：“您之所以收到这封邮件，是因为您一直与&#x200B;***您的组织名称***&#x200B;或关联公司有联系。要不再接收来自&#x200B;***您的组织名称***&#x200B;的邮件，请单击此处。”

## 个性化电子邮件主题行 {#personalize-subject-line}

要在邮件的&#x200B;**[!UICONTROL 主题行]**&#x200B;字段中添加个性化内容，请执行以下步骤：

1. 单击&#x200B;**[!UICONTROL 主题行]**&#x200B;字段右侧的&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标。

   ![](assets/perso-subject.png){width="600"}

1. 输入主题行内容并选择要添加的个性化属性。

1. 单击 **[!UICONTROL 确认]****验证。 个性化属性将添加到主题行。

## 个性化您的电子邮件内容 {#personalize-emails}

要个性化电子邮件内容，请在电子邮件设计器中打开邮件，然后：

1. 在文本块内单击。
1. 在上下文工具栏中，选择&#x200B;**[!UICONTROL 添加个性化内容]**。

   ![](assets/perso-add-to-content.png)

1. 在个性化编辑器中插入收件人姓名并进行确认。

   ![](assets/perso-add-name.png)

   个性化属性将添加到电子邮件内容。

   您可以模拟内容以检查渲染。[了解详情](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. 要向电子邮件添加内容块，请执行相同的步骤，并从最后一个图标中选择内容块：

   ![](assets/perso-insert-block.png)

1. 插入内容块后，内容块会添加到电子邮件内容中。在投放准备步骤中，内容块会在生成个性化时自动适应收件人用户档案。

   ![](assets/perso-content-block-in-email.png)

## 个性化电子邮件中的链接 {#personalize-links}

要个性化&#x200B;**链接**，请执行以下操作：

1. 选择文本块或图像。
1. 在上下文工具栏中，选择&#x200B;**插入链接**。

   ![](assets/perso-link.png)

1. 输入链接标签并使用&#x200B;**插入链接**&#x200B;按钮来个性化链接。

   ![](assets/perso-link-insert-icon.png)

1. 使用个性化编辑器来定义和个性化链接，并进行确认。

   ![](assets/perso-link-edit.png)


## 个性化您的优惠 {#personalize-offers}

您还可以在将文本类型的内容添加到优惠的表示形式时访问个性化编辑器。在[此章节](../content/offers.md)中了解更多信息。
