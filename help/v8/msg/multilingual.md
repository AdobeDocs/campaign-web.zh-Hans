---
audience: end-user
title: 配置多语言投放
description: 了解如何配置多语言投放
source-git-commit: e005c409a61748d99b70b2a99f4f4f89d4d6229e
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 7%

---

# 配置多语言投放 {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="添加语言"
>abstract="在此选项卡中，您将找到要发送的投放所使用的语言列表。您可以通过单击“添加语言”按钮或通过此选项卡复制另一种语言来添加更多语言。"

[!CONTEXTUALHELP]
>id=&quot;acw_multilingual_file_upload&quot;
>title=&quot;导入语言变体&quot;
>abstract=&quot;使用此对话框可通过导入CSV文件来添加语言变体。 该文件会自动填充所选语言的所有可用字段。 您可以在确认之前拖放文件或从计算机中选择文件。”

在Campaign Web UI中，您可以将投放设置为多语言，这允许您根据用户档案的首选语言发送消息。 未定义首选项时，将以默认语言发送消息。

在多语言投放中，语言管理基于变体。 每个变体表示一种语言。 在创建投放期间，您可以添加多种语言变体以匹配消息中所需的语言数量。 您还可以在添加这些变体后随时更改默认语言。

目前，多语言功能可用于电子邮件、推送通知、事务性消息和短信。

>[!AVAILABILITY]
>
>多语言推送通知、事务性消息和短信仅适用于一组组织（限量发布），并将在未来版本中全局推出。 您的服务器必须升级到8.8.2或更高版本。

要设置多语言投放，请执行以下步骤：

1. 添加语言变体，[阅读更多](#add-variant)
1. 定义每个变体的内容，[了解更多](#define-content)
1. 管理语言变体，[阅读更多](#manage-variant)

## 添加语言变体{#add-variant}

要创建语言变体，请执行以下步骤：

1. 在投放仪表板中，单击铅笔图标以访问投放内容版本屏幕，然后单击&#x200B;**[!UICONTROL 添加语言]**。

   >[!IMPORTANT]
   >
   >仅当目标维度包含&#x200B;**[!UICONTROL 语言]**&#x200B;架构时，**添加语言**&#x200B;按钮才可用。 要了解有关架构和目标维度的更多信息，请参阅[详细文档](../audience/targeting-dimensions.md)。

   ![](assets/edit-content_2.png){zoomable="yes"}

1. 从&#x200B;**添加语言**&#x200B;下拉列表中，选择要添加的语言，然后确认。

   您添加的第一种语言会自动设置为默认语言，而现有内容会成为默认版本。 添加其他语言时，最初会从默认语言复制其内容。

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >通过此列表可用的语言取决于&#x200B;**语言**&#x200B;属性定义的值（如system、user、dbenum等值）。 在此[部分](../administration/enumerations.md)中了解有关枚举管理的更多信息。

1. 重复此操作以添加其他语言。 左侧的&#x200B;**[!UICONTROL 语言]**&#x200B;面板显示您已选择的语言列表、语言数和默认语言。

   例如，如果您选择了英语、法语和瑞典语，则可以看到如下所示的这3种语言：

   ![](assets/edit-content_9.png){zoomable="yes"}

   要了解如何管理语言变体，请参阅此[部分](#manage-variant)。

## 定义每个变体的内容{#define-content}

设置语言后，为每个语言定义投放内容。

1. 从投放内容版本屏幕的左侧&#x200B;**[!UICONTROL 语言]**&#x200B;面板中选择一种语言。

   ![](assets/edit-content_11.png){zoomable="yes"}

1. 为此语言定义消息的内容。 在此[部分](../msg/create-deliveries.md)中了解详情。

1. 对每种语言重复此操作。

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

要预览投放，请单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮，然后选择用户档案。 确保为每个配置文件显示正确的内容。

![](assets/edit-content_5.png){zoomable="yes"}

## 管理语言变体{#manage-variant}

在左侧面板中，将显示所有语言变体信息。 若要删除所有语言，请单击“展开”按钮，然后单击“删除所有变体”****。

![](assets/edit-content_13.png){zoomable="yes"}

在语言变体列表中，您可以执行以下操作：

* **编辑**：在保留关联内容的同时更改语言。
* **设置为默认语言**：将语言设置为默认语言。 当个人资料未定义语言时，消息将以默认语言发送。
* **复制**：复制为此语言定义的内容并选择其他变体。
* **删除**：删除变体及其关联内容。

![](assets/edit-content_13-sms.png){zoomable="yes"}

