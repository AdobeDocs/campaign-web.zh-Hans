---
title: 在 Campaign 中个性化您的内容
description: 了解如何在Adobe Campaign Web中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 4%

---

# 个性化您的内容 {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="添加当前日期"
>abstract="此菜单提供与日期格式相关的功能，您可以利用这些功能来个性化您的内容。"

投放内容的Personalization是一项关键功能，它允许您为各个收件人定制消息，从而使通信更具有相关性和吸引力。

在Adobe Campaign中，通过使用[个人资料数据](#data-personalization)（如个人资料的名称、位置或过去的交互）和投放的特定[变量](#variables-personalization)，您可以动态自定义通信中的文本、图像和选件等元素。

交付个性化增强了用户体验并提高了参与率，从而实现了更高的转化率和客户满意度。

## 使用用户档案数据进行个性化 {#data-personalization}

您可以使用表达式编辑器对包含用户档案数据的任何投放进行个性化，该编辑器可在包含&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标的字段中访问，例如主题行、电子邮件链接和文本/按钮内容组件。 [了解如何访问表达式编辑器](gs-personalization.md/#access)。

### Personalization语法 {#syntax}

Personalization标记遵循特定语法： `<%= table.field %>`。 例如，要从收件人表中插入收件人的姓氏，请使用`<%= recipient.lastName %>`语法。

在投放准备过程中，Adobe Campaign会解释这些标记，并将其替换为每个收件人的相应字段值。 您可以通过模拟内容来查看实际替换。

从外部文件上传联系人以进行独立电子邮件投放时，输入文件中的所有字段都可用于个性化。 语法如下： `<%= dataSource.field %>`。

### 添加个性化标记 {#add}

要将个性化标记添加到投放中，请执行以下步骤：

1. 使用&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标打开表达式编辑器，可通过文本类型编辑字段（如主题行或短信正文）访问该图标。 [了解如何访问表达式编辑器](gs-personalization.md/#access)。

   ![显示如何访问个性化对话框的屏幕截图](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. 表达式编辑器将打开。 Adobe Campaign数据库中可用的个性化字段在屏幕左侧被整理到多个菜单中：

   ![显示个性化字段菜单的屏幕截图](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | 菜单 | 说明 |
   |------|-------------|
   | ![订阅者应用程序菜单图标](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | **[!UICONTROL 订阅者应用程序]**&#x200B;菜单列出了与应用程序的订阅者相关的字段，例如使用的终端或操作系统。 *此菜单仅适用于推送通知。* |
   | ![收件人菜单图标](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | **[!UICONTROL 收件人]**&#x200B;菜单列出了在收件人表中定义的字段，如收件人的姓名、年龄或地址。 当从外部文件[&#128279;](../audience/file-audience.md)上载独立电子邮件投放的联系人时，此菜单列出输入文件中所有可用的字段。 |
   | ![消息菜单图标](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | **[!UICONTROL 消息]**&#x200B;菜单列出了与投放日志相关的字段，包括跨所有渠道发送到收件人或设备的所有消息，如与给定收件人的上次事件的日期。 |
   | ![传递菜单图标](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | **[!UICONTROL 投放]**&#x200B;菜单列出了与执行投放所需的参数相关的字段，如投放渠道或标签。 |

   >[!NOTE]
   >
   >默认情况下，每个菜单均列出选定表中的所有字段（收件人、/消息/投放）。 如果要包含链接到选定表的表中的字段，请启用位于列表下方的&#x200B;**[!UICONTROL 显示高级属性]**&#x200B;选项。

1. 要添加个性化字段，请将光标放在内容中所需的位置，然后单击`+`按钮以插入该字段。

1. 内容准备就绪后，保存该内容，并通过模拟内容来测试个性化内容的呈现。 以下示例显示了使用收件人名字的短信消息的个性化设置。

   ![显示带有收件人名字的SMS个性化预览的屏幕截图](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![显示带有收件人名字的SMS个性化预览的屏幕截图](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## 使用变量进行个性化 {#variables-personalization}

您还可以使用变量将投放个性化。 了解有关[将变量添加到投放](../advanced-settings/delivery-settings.md#variables-delivery)的更多信息。

例如，变量`deliveryType`的定义如下所示。

![显示deliveryType变量定义的屏幕截图](assets/variables-deliveryType.png){zoomable="yes"}

此变量通过使用&#x200B;**[!UICONTROL 添加Personalization]**&#x200B;图标和此示例中的表达式`<%= variables.deliveryType %>`在投放内容中使用。

![显示个性化中使用deliveryType变量的屏幕截图](assets/variables-perso.png){zoomable="yes"}

通过&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮检查变量的使用。

![显示使用deliveryType变量模拟内容的屏幕截图](assets/variables-simulate.png){zoomable="yes"}