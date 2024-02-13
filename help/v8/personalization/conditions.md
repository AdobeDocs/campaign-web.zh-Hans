---
title: 创建条件内容
description: 了解如何定义条件以在Adobe Campaign Web中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 6%

---

# 构建条件内容{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="添加条件内容"
>abstract="配置条件内容字段以根据收件人的配置文件数据创建高级动态个性化内容。当满足特定条件时，将替换消息内容中的文本块、链接、主题行和/或图像。"

## 条件内容入门 {#gs}

条件内容是一项强大的功能，允许您根据收件人的配置文件创建动态个性化，在满足某些条件时自动替换文本块和图像。 此功能可进一步提升您的营销活动，并为您的受众提供具有高度针对性的个性化体验。

通过配置条件内容字段，您可以根据收件人的用户档案创建高级动态个性化。 当满足特定条件时，在消息内容中替换文本块、链接、主题行和/或图像。 例如，您可以根据Adobe Campaign数据库中“性别”字段的值显示“先生”或“夫人”，或根据收件人的首选语言包含其他链接。

要创建条件内容，您需要在 **表达式编辑器** 使用特定的辅助函数。 此方法适用于所有投放渠道，以及可访问表达式编辑器的任何字段，例如主题行或电子邮件链接和文本/按钮内容组件。 [了解如何访问表达式编辑器](gs-personalization.md/#access)

除了表达式编辑器之外，您还可以利用专用的 **条件内容生成器** 在设计允许您为电子邮件正文的某个元素创建多个变体的电子邮件时。 [了解如何在电子邮件中创建条件内容](#condition-condition-builder)

## 在表达式编辑器中创建条件 {#condition-perso-editor}

要使用表达式编辑器为投放定义条件内容，请执行以下步骤。 在本例中，我们要根据收件人的语言（法语或英语）创建条件内容。

1. 打开投放并导航到内容编辑部分。

1. 找到要添加条件内容的字段。 例如，可以向短信消息添加条件内容。

1. 单击 **[!UICONTROL 打开个性化对话框]** 图标来打开表达式编辑器。

   ![](assets/open-perso-editor-sms.png){zoomable=&quot;yes&quot;}

1. 在个性化编辑器中，浏览到 **[!UICONTROL 辅助函数]** 菜单的位置。

1. 要开始构建条件，请单击 **如果** 函数。 以下行将添加到中央屏幕中：`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * 替换 `<FIELD>` 替换为个性化字段，例如收件人的语言： `recipient.language`.
   * 替换 `<VALUE>` 包含要满足的值。 例如， `'French'`.
   * 替换 `Ìnsert content here` ，其中包含您要向符合指定条件的配置文件显示的内容。

     ![](assets/condition-sample1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 指定收件人不符合条件时应显示的内容。 为此，请使用 **否则** 辅助函数：

   1. 将光标放在表达式结束标记之前 `%>` 然后单击 `+` 旁边的 **否则** 函数。

   1. 替换 `Ìnsert content here` ，其中包含您要显示给不符合if函数条件的用户档案的内容。

   ![](assets/condition-sample2.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   您也可以使用 **否则，如果** 用于使用多个内容变量构建条件的辅助函数。 例如，下面的表达式根据收件人的语言显示消息的三种变体：

   ![](assets/condition-sample3.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   >[!NOTE]
   >
   >每次添加辅助函数时，打开(`<%`)和结束(`%>`)标记会在函数之前和之后自动添加。
   >
   >在表达式中添加“Else”辅助函数后的示例：>
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >确保删除这些标记以避免任何语法错误。 在本例中，删除 **否则** 函数标签为：
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. 条件就绪后，您可以保存内容并通过模拟内容来检查其渲染情况。

## 在电子邮件中创建条件内容 {#condition-condition-builder}

可通过两种方式创建电子邮件中的条件内容：
* 在表达式编辑器中，通过构建包含辅助函数的条件，
* 在设计电子邮件时可访问的专用条件内容生成器中。

以下部分提供了有关如何使用Email Designer的条件内容功能创建条件的分步说明。 提供了有关如何使用表达式编辑器创建条件的详细信息 [此处](#condition-perso-editor).

在本例中，我们希望根据收件人的语言创建包含多个变体的电子邮件。 执行以下步骤：

1. 创建或打开电子邮件投放，编辑其内容，然后单击 **[!UICONTROL 编辑电子邮件正文]** 按钮以打开电子邮件设计工作区。

1. 选择内容组件并单击 **[!UICONTROL 启用条件内容]** 图标。

   ![](assets/condition-email-enable.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 此 **[!UICONTROL 条件内容]** 窗格在屏幕左侧打开。 在此窗格中，您可以使用条件创建所选内容组件的多个变体。

1. 配置您的第一个变体。 将鼠标悬停在 **[!UICONTROL 变体 — 1]** 在 **[!UICONTROL 条件内容]** 窗格并单击 **[!UICONTROL 添加条件]** 按钮。

   ![](assets/condition-add-condition.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 此时会显示规则生成器。 它提供 **个人资料**， **消息**、和 **投放** 可用于创建条件的属性。

   此外， **条件** 菜单提供了预建条件，您可以将这些条件添加到画布以轻松构建变体。 要使用它们，请单击 **添加** 按钮替换以下元素之间的元素 `<` 和 `>`符号。 确保您为 `<value>` 对象在引号中。

   ![](assets/condition-syntax.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 消息第一个变体的条件就绪后，单击 **[!UICONTROL 确认]**. 在本例中，我们将创建一项规则，以语言为“法语”的收件人为目标。

   ![](assets/condition-example.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 该规则现在已关联到变体。 为了提高可读性，我们建议通过单击省略号菜单来重命名变体。

1. 配置在发送消息时如果满足规则应如何显示组件。 在本例中，我们希望以法文显示文本（如果它是收件人的首选语言）。

   ![](assets/condition-email-variant1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 根据内容组件的需要，添加任意数量的变体。 您可以随时在变体之间切换，以检查内容组件将如何根据其条件规则显示。

   >[!NOTE]
   >如果在发送消息时未满足变体定义的所有规则，则内容组件将显示中定义的内容。 **[!UICONTROL 默认变量]** 从 **[!UICONTROL 条件内容]** 窗格。
