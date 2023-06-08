---
title: 在 Campaign 中个性化您的内容
description: 了解如何在 Adobe Campaign Web UI 中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

---


# 个性化您的内容{#add-personalization}

可以使用表达式编辑器将个性化添加到任何投放中。

个性化标记始终使用以下语法： `<%=table.field%>`例如，要插入存储在收件人表中的收件人名称，个性化标记使用&lt;%= recipient.lastName %>语法。

准备投放后，Adobe Campaign会自动解释这些标记，并将其替换为给定收件人的字段值。 然后，在模拟内容时，可以查看物理替换。

要将个性化标记添加到投放中，请单击可从文本类型编辑字段（如主题行或短信正文）访问的打开个性化对话框图标。

![](assets/perso-access.png)

此时将显示表达式编辑器。 个性化字段被组织为三个菜单，位于屏幕左侧。 通过这些菜单，可以访问Adobe Campaign数据库中可用的所有字段。

| 菜单 | 说明 |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | 此 **[!UICONTROL 收件人]** 菜单列出了收件人表中定义的所有字段，例如收件人的姓名、年龄或地址。 |
| ![](assets/do-not-localize/perso-message-menu.png) | 此 **[!UICONTROL 消息]** 菜单列出与投放日志相关的所有字段，即跨所有渠道发送到收件人或设备的所有消息，如与给定收件人发生的最后一个事件的日期 |
| ![](assets/do-not-localize/perso-delivery-menu.png) | 此 **[!UICONTROL 投放]** 菜单列出与执行投放所需的参数相关的所有字段，例如投放渠道、标签等。 |

>[!NOTE]
>
>默认情况下，该列表显示选定表中的所有字段（收件人、/消息/投放）。 如果要包含链接到选定表的表中的字段，请启用 **[!UICONTROL 显示高级属性]** 选项的位置。

要添加个性化字段，请将光标放在内容中的所需位置，然后单击+按钮以插入该字段。

![](assets/perso-insert-field.png)

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

1. 一旦插入该内容块，即将它添加到电子邮件内容。在投放准备步骤中生成个性化时，将自动使该内容块适应收件人配置文件。

   ![](assets/perso-content-block-in-email.png)


## 个性化您的优惠 {#personalize-offers}

您还可以在将文本类型的内容添加到优惠的表示形式时访问个性化编辑器。在[此章节](../content/offers.md)中了解更多信息。

