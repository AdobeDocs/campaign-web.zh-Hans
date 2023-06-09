---
title: 动态内容入门
description: 了解如何使用个性化、条件内容和内置内容块使内容成为动态内容。
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: 3dc7f1f6522a7dbd2edadcb0f7b8841e30fd8af0
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 21%

---


# 动态内容入门

为了充分利用每个营销活动，Adobe Campaign为您提供了一种方法，可交付与客户级别对话的自定义动态内容。 根据用户档案数据，使用个性化功能为不同的组和个人创建自定义体验：您可以利用有关消息的数据和信息，根据每个特定收件人调整消息。 这可以是他们的名字、兴趣、居住地、购买的东西等等。

使用 Campaign 创建动态内容并发送个性化消息。可以结合个性化功能来改进您的消息并创建自定义用户体验。

## 如何使您的内容成为动态内容？

您可以通过插入以下内容来动态显示消息内容：

* **个性化字段**：个性化字段用于消息的第一级个性化。 您可以从个性化编辑器中选择数据库中可用的任何字段。对于投放，您可以选择与收件人、邮件或投放相关的任何字段。可将这些个性化属性插入邮件的主题行或正文中。以下语法可在您的内容中插入收件人的城市：&lt;%= recipient.location.city %>。

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **条件内容**：例如，配置条件内容以根据收件人的配置文件添加内容。 满足特定条件时可插入文本块和/或图像。当条件不为true时，您可以定义内容的替代版本。

* **内置内容块**：Campaign提供了一组个性化块，其中包含您可以插入到投放中的特定渲染。 例如，您可以添加徽标、问候语消息或指向电子邮件镜像页面的链接。 内容块可通过个性化编辑器中的专用条目使用。

  ![](assets/perso-content-blocks.png){width="800" align="center"}

## 访问表达式编辑器 {#access}

Adobe Campaign V8 Web提供了一个表达式编辑器，您可以在其中选择、排列、自定义和验证所有数据，从而为您的内容创建自定义体验。 表达式编辑器适用于所有渠道，在每个字段内使用 **[!UICONTROL 打开个性化对话框]** 图标，例如主题行字段，或电子邮件链接和文本/按钮内容组件。

以下是如何根据要使其成为动态的内容访问表达式编辑器的几个示例：

* *从“发件人名称”字段访问表达式编辑器*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *从电子邮件文本组件访问表达式编辑器*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *从电子邮件中的链接访问表达式编辑器*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>除了表达式编辑器之外，在设计电子邮件时，您还可以利用专用的条件内容生成器。 [了解如何在电子邮件中构建条件内容](conditions.md)

## 让我们深入探究

现在，您已了解如何使内容生动活泼，接下来该深入了解这些文档部分以开始使用该功能。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="个性化内容" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>添加个性化内容</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="商机" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>添加条件内容</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="不常见" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>添加内置内容块</strong></a>
</div>
<p></td>
</tr></table>
