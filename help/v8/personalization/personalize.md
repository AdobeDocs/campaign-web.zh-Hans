---
title: 在 Campaign 中个性化您的内容
description: 了解如何在Adobe Campaign Web中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 2%

---


# 个性化您的内容 {#add-personalization}

您可以使用表达式编辑器对任何投放进行个性化设置，该编辑器可在带有&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标的字段中访问，例如主题行、电子邮件链接和文本/按钮内容组件。 [了解如何访问表达式编辑器](gs-personalization.md/#access)

## Personalization语法 {#syntax}

Personalization标记遵循特定语法： `<%= table.field %>`。 例如，要从收件人表中插入收件人的姓氏，请使用`<%= recipient.lastName %>`语法。

在投放准备过程中，Adobe Campaign会自动解释这些标记，并将其替换为每个收件人的相应字段值。 您可以通过模拟内容来查看实际替换。

从外部文件上传联系人以进行独立电子邮件投放时，输入文件中的所有字段都可用于个性化。 语法如下： `<%= dataSource.field %>`。

## 添加个性化标记 {#add}

要将个性化标记添加到投放中，请执行以下步骤：

1. 使用可从文本类型编辑字段（如主题行或短信正文）访问的&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标打开表达式编辑器。 [了解如何访问表达式编辑器](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. 表达式编辑器将打开。 Adobe Campaign数据库中可用的个性化字段在屏幕左侧被整理到多个菜单中：

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | 菜单 | 说明 |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | **[!UICONTROL 订阅者应用程序]**&#x200B;菜单列出了与应用程序的订阅者相关的字段，例如使用的终端或操作系统。 *此菜单仅适用于推送通知* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | **[!UICONTROL 收件人]**&#x200B;菜单列出了在收件人表中定义的字段，如收件人的姓名、年龄或地址。 当从外部文件](../audience/file-audience.md)上载独立电子邮件投放的联系人时[，此菜单列出输入文件中所有可用的字段。 |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | **[!UICONTROL 消息]**&#x200B;菜单列出了与投放日志相关的字段，包括跨所有渠道发送到收件人或设备的所有消息，如与给定收件人的最后事件的日期 |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | **[!UICONTROL 投放]**&#x200B;菜单列出了与执行投放所需的参数（如投放渠道或标签）相关的字段。 |

   >[!NOTE]
   >
   >默认情况下，每个菜单均列出选定表中的所有字段（收件人、/消息/投放）。 如果要包含链接到选定表的表中的字段，请启用位于列表下方的&#x200B;**[!UICONTROL 显示高级属性]**&#x200B;选项。

1. 要添加个性化字段，请将光标放在内容中所需的位置，然后单击`+`按钮以插入该字段。

1. 内容准备就绪后，您可以保存它并通过模拟内容来测试个性化呈现。 以下示例显示了使用收件人名字的短信消息的个性化设置。

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}
