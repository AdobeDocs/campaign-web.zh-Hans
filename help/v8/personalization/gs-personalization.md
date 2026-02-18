---
title: 如何将内容设置为动态内容？
description: 了解如何使用个性化、条件内容将内容设置为动态内容。
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
old-role: Data Architect
role: Developer
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 100%

---

# 如何将内容设置为动态内容？ {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="个性化"
>abstract="个性化编辑器允许您选择、整理、定制和验证所有数据，为您的内容打造个性化体验。您可以利用轮廓数据为每位收件人定制个性化信息，并创建条件性内容，使信息适应每位收件人，并只展示相关内容。"

作为一名营销人员，锁定那些真正对您的产品感兴趣的客户，并提供有效的相关内容来吸引他们是至关重要的。鉴于您会遇到各种不同的收件人，创建多种营销内容来吸引不同的受众可能会既耗时又浪费。这就是动态内容变得至关重要的地方。

Adobe Campaign Web 动态内容功能可让您根据收集到的收件人的相关信息来定制内容。通过使用动态内容，您可以确保营销工作更具相关性，避免推广不需要或不必要的产品或服务。这种方法可使您的内容更具吸引力，并使受众更愿意去阅读内容。此外，它使您能够个性化您的内容，让收件人觉得他们收到的信息是由人而不是机器发送的。

## 如何将内容设置为动态内容？ {#make-content-dyn}

您可以通过在 Campaign Web 表达式编辑器中插入 JavaScript 结构来将消息内容设为动态内容。在发送消息时，Adobe Campaign 会解读这些表达式，以便向每位收件人发送正确的内容：

* 通过利用轮廓数据（例如，收件人的名字、兴趣、居住地、购买的产品等），针对每个特定的收件人&#x200B;**个性化您的消息**。您可以从与收件人、消息或投放相关的个性化编辑器中选择数据库中的任何可用字段。可将这些个性化属性插入邮件的主题行或正文中。以下语法可在您的内容中插入收件人的城市：`<%= recipient.location.city %>`。

  [描述：使用个性化属性将收件人的城市插入主题行的示例。](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **创建条件内容**，使您的投放适合每个收件人，并根据您获得的给定客户的相关信息，仅向其显示相关内容。这允许您根据条件显示特定的文本块和/或图像。例如，根据收件人的特定服务订阅来调整电子邮件横幅。

  [描述：基于收件人订阅情况的电子邮件横幅中的条件内容示例。](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [通过观看视频了解此功能](#video)

## 访问表达式编辑器 {#access}

Adobe Campaign Web 提供了一个表达式编辑器，可让您选择、排列、自定义和验证所有数据，为自己的内容创建定制体验。在每个带有&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标的字段（例如主题行字段）或电子邮件链接和文本/按钮内容组件中，表达式编辑器可用于所有渠道。

以下是有关如何根据要设为动态内容的内容来访问表达式编辑器的一些示例：

* *从发件人名称字段访问表达式编辑器*

  [描述：从发件人名称字段访问表达式编辑器的示例。](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *从电子邮件文本组件访问表达式编辑器*

  [描述：从电子邮件文本组件访问表达式编辑器的示例。](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *从电子邮件中的链接访问表达式编辑器*

  [描述：从电子邮件中的链接访问表达式编辑器的示例。](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>除了表达式编辑器之外，您还可以在设计电子邮件时利用专用的条件内容生成器。[了解如何在电子邮件中生成条件内容](conditions.md)

## 操作说明视频 {#video}

了解如何通过使用表达式编辑器来个性化您的消息或添加条件内容，从而使消息内容动态化。

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)