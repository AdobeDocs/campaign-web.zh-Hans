---
title: 创建条件内容
description: 了解如何在 Adobe Campaign Web UI 中定义条件以使内容个性化
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta 版"
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 14%

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

<!--In addition to the expression editor, you can leverage a dedicated **conditional content builder** when designing an email that allows you to build conditions using profile attributes only. [Learn how to create conditional content in emails](#condition-condition-builder)-->

## 在表达式编辑器中创建条件 {#condition-perso-editor}

要使用表达式编辑器为投放定义条件内容，请执行以下步骤。 在本例中，我们要根据收件人的语言（法语或英语）创建条件内容。

1. 打开投放并导航到内容编辑部分。

1. 找到要添加条件内容的字段。 例如，可以向短信消息添加条件内容。

1. 单击 **[!UICONTROL 打开个性化对话框]** 图标来打开表达式编辑器。

   ![](assets/open-perso-editor-sms.png)

1. 在个性化编辑器中，浏览到 **[!UICONTROL 辅助函数]** 菜单的位置。

1. 要开始构建条件，请单击 **如果** 函数。 以下行将添加到中央屏幕中：`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * 替换 `<FIELD>` 替换为个性化字段，例如收件人的语言： `recipient.language`.
   * 替换 `<VALUE>` 包含要满足的值。 例如， `'French'`.
   * 替换 `Ìnsert content here` ，其中包含您要向符合指定条件的配置文件显示的内容。

     ![](assets/condition-sample1.png){width="800" align="center"}

1. 指定收件人不符合条件时应显示的内容。 为此，请使用 **否则** 辅助函数：

   1. 将光标放在表达式结束标记之前 `%>` 然后单击 `+` 旁边的 **否则** 函数。

   1. 替换 `Ìnsert content here` ，其中包含您要显示给不符合if函数条件的用户档案的内容。

   ![](assets/condition-sample2.png){width="800" align="center"}

   您也可以使用 **否则，如果** 用于使用多个内容变量构建条件的辅助函数。 例如，下面的表达式根据收件人的语言显示消息的三种变体：

   ![](assets/condition-sample3.png){width="800" align="center"}

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

<!--SECTION REMOVED FOR LA > CONDITIONAL CONTENT NOT AVAILABLE ANYMORE FROM THE DEDICATED MENU IN THE EMAIL DESIGNER. ONLY THE EXPRESSION EDITOR IS AVAILABLE FOR NOW

## Create conditional content in emails {#condition-condition-builder}

Conditional content in emails can be created in two ways:
* In the expression editor by building a condition with helper functions,
* In a dedicated conditional content builder that is accessible when designing an email.

Detailed information on how to create conditions using the expression editor is available [here](#condition-perso-editor). The following section provides step-by-step instructions on how to create conditions using the email designer's conditional content capability. In this example, we want to create an email message with multiple variants based on the recipients' language. Follow these steps:

1. Create or open an email delivery, edit its content, and click the **[!UICONTROL Edit email body]** button to open the email designing workspace.

1. Select a content component and click the **[!UICONTROL Enable conditional content]** icon.

    ![](assets/condition-email-enable.png){width="800" align="center"}

1. The **[!UICONTROL Conditional Content]** pane opens on the left-hand side of the screen. In this pane, you can create multiple variants of the selected content component using conditions.

1. Configure your first variant. Hover over **[!UICONTROL Variant - 1]** in the **[!UICONTROL Conditional Content]** pane and click the **[!UICONTROL Add condition]** icon.

1. A query modeler appears. Use profile attributes to create the condition for the first variant of the message and click **[!UICONTROL Confirm]**. In this example, we are creating a rule targeting recipients whose language is 'French'.

    ![](assets/condition-email-rule.png){width="800" align="center"}

1. The rule is now associated to the variant. For better readability, we recommend renaming the variant by clicking the ellipsis menu.

1. Configure how the component should display if the rule is met when sending the message. In this example, we want to display the text in French if it is the recipient's preferred language.

    ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Add as many variants as needed for the content component. You can switch between the variants at any time to check how the content component will display based on their conditional rules.

    >[!NOTE]
    >If none of the rules defined in the variants are met when sending the message, the content component will display the content defined in the **[!UICONTROL Default variant]** from the **[!UICONTROL Conditional Content]** pane.
-->