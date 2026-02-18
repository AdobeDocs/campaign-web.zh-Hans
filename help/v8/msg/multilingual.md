---
audience: end-user
title: 配置多语言投放
description: 了解如何配置多语言投放
exl-id: eea0e997-4da2-4998-b010-234626b21353
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '1514'
ht-degree: 3%

---

# 配置多语言投放 {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="多语言投放"
>abstract="您现在可以在Campaign Web UI中以多种语言发送消息。 对于推送通知，请通过上传CSV文件填充所有语言变体。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="添加语言"
>abstract="在此选项卡中，您将找到要发送的投放所使用的语言列表。您可以通过单击“添加语言”按钮或通过此选项卡复制另一种语言来添加更多语言。"

>[!CONTEXTUALHELP]
>id="acw_multilingual_file_upload"
>title="导入语言变体"
>abstract="使用此对话框可通过导入CSV文件来添加语言变体。 该文件会自动填充所选语言的所有可用字段。 在确认之前，您可以拖放文件或从计算机中选择文件。"

在Campaign Web UI中，您可以将投放设置为多语言，这允许您根据用户档案的首选语言发送消息。 未定义首选项时，将以默认语言发送消息。

在多语言投放中，语言管理基于变体。 每个变体表示一种语言。 在创建投放期间，您可以添加多种语言变体以匹配消息中所需的语言数量。 您还可以在添加这些变体后随时更改默认语言。

目前，多语言功能可用于电子邮件、推送通知、事务性消息和短信。

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

1. 从&#x200B;**添加语言**&#x200B;下拉列表中，选择要添加的语言，然后确认。 对于推送通知，您也可以[上传CSV文件](#csv-upload)以同时导入所有语言变体。

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

## 从CSV导入语言变体（推送通知） {#csv-upload}

对于推送通知，您可以通过上传包含多语言内容的CSV文件来快速填充所有语言变体。 此功能允许您离线准备内容并批量导入内容，从而简化多语言营销活动的创建。

* **效率**：在单个操作中添加多种语言及其内容
* **一致性**：确保所有语言变体之间消息传递一致
* **Collaboration**：使内容团队能够在熟悉的电子表格工具中准备翻译
* **批量管理**：轻松管理和更新大量语言变体

### 先决条件 {#csv-best-practices}

请遵循以下最佳实践以确保成功CSV导入：

* **使用确切的列结构**：CSV文件中必须包含所有14列，即使将一些列留空也是如此。 缺少列将导致导入失败。 您可以使用不同的顺序，但必须存在所有列。
* **与列名完全匹配**：列名区分大小写。 使用`title`而不是`Title`，`badge`不是`Bbadge`，`locale`不是`Locale`。
* **使用小写区域设置代码**：将区域设置代码格式设置为`en_us`、`fr_fr`、`de_de`（带下划线的小写），而不是`en_US`或`en-us`。
* **填写必需的列**： `locale`和`language`列必须包含每行的值。 空值将导致导入失败。
* **保持区域设置唯一**：每个区域设置代码在CSV文件中只能出现一次。 重复的区域设置将被拒绝。
* **另存为UTF-8**：始终使用UTF-8编码保存CSV文件以正确支持国际字符。
* **引号包含逗号的内容**：如果您的标题或邮件正文包含逗号，请将整个字段用双引号括起来： `"Hello, welcome!"`。
* **正确使用数值**：对于标志列(isContentAvailable、isMutableContent、silentPush)，使用`1`表示true，`0`表示false，或保留空白表示默认值。
* **验证JSON格式**：如果使用customFields列，请确保您的JSON格式正确： `{"key":"value"}`包含正确的引号和括号。
* **首先使用最少的数据进行测试**：首先使用简单的2-3语言CSV验证您的格式，然后再创建大型文件。

>[!NOTE]
>
>此[部分](#csv-columns)中详细介绍了列结构。

### 导入CSV文件 {#csv-steps}

要从CSV文件导入语言变体，请执行以下步骤：

1. 在投放内容编辑器中，单击&#x200B;**[!UICONTROL 添加语言]**。

   ![在推送通知内容编辑器中显示“添加语言”按钮的屏幕截图](assets/multilingual-csv.png){zoomable="yes"}

1. 通过将CSV文件拖放到上传区域来选择该文件，或单击以浏览计算机。

   系统会验证您的文件格式和内容。 如果验证失败，错误消息将指示哪些列或数据不正确。 修复了CSV文件中的问题并再次上传。 请参阅此[章节](#csv-troubleshooting)。

   ![屏幕截图显示成功对所有语言导入的CSV验证](assets//multilingual-csv2.png){zoomable="yes"}

1. 在语言变体面板中查看导入的内容以确认所有翻译均已正确加载。

   ![显示导入的多语言内容变体预览的屏幕截图](assets/multilingual-csv3.png){zoomable="yes"}

### 列结构 {#csv-columns}

以下是要使用的正确列结构：

>[!NOTE]
>
>您可以使用不同的顺序，但必须存在所有列。 有关更多最佳实践，请参阅此[部分](#csv-best-practices)。

1. **title**：通知标题（必需）
1. **messageBody**：通知邮件正文（必需）
1. **声音**：声音文件名（例如，`default`，`custom_sound.mp3`） — 留空表示默认值
1. **徽章**：要在应用程序图标上显示的徽章编号(iOS) — 仅使用编号
1. **deeplinkURI**：在点按通知时打开的深层链接URL — 如果未使用，则留空
1. **category**：自定义操作的通知类别标识符(iOS) — 如果未使用，请留空
1. **iosMediaAttachmentURL**：用于iOS通知的媒体附件的URL — 如果未使用，则保留为空
1. **androidMediaAttachmentURL**：用于Android通知的媒体附件的URL — 如果未使用，请留空
1. **isContentAvailable**： Content available标志(iOS) — 将`1`用于true，将`0`用于false，将留空用于默认值(0)
1. **isMutableContent**：可变内容标志(iOS) — 将`1`用于true，将`0`用于false，将留空用于默认值(0)
1. **customFields**： JSON格式的自定义数据（例如，`{"key1":"value1","key2":"value2"}`） — 如果未使用，则留空
1. **区域设置**：语言代码（必需） — 例如`en_us`、`fr_fr`、`de_de` - **必需，每行必须是唯一的**
1. **语言**：语言名称（必需） — 例如，`English-United States`，`French-France` - **必需**
1. **silentPush**：静默推送标志 — 将`1`用于静默推送，`0`用于常规，保留为空则用于默认值(0)

### CSV文件示例 {#csv-examples}

以下是必填字段的基本示例：

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
Welcome!,Thank you for joining us,,,,,,,,,, en_us,English-United States,0
Bienvenue !,Merci de nous avoir rejoint,,,,,,,,,,fr_fr,French-France,0
Willkommen!,Vielen Dank für Ihre Anmeldung,,,,,,,,,, de_de,German-Germany,0
¡Bienvenido!,Gracias por unirte a nosotros,,,,,,,,,, es_es,Spanish-Spain,0
```

以下是可选字段的示例：

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
Welcome!,Thank you for joining us,default,1,,,https://example.com/welcome-en.jpg,https://example.com/welcome-en.jpg,,,, en_us,English-United States,0
Bienvenue !,Merci de nous avoir rejoint,default,1,,,https://example.com/welcome-fr.jpg,https://example.com/welcome-fr.jpg,,,, fr_fr,French-France,0
Willkommen!,Vielen Dank für Ihre Anmeldung,default,1,,,https://example.com/welcome-de.jpg,https://example.com/welcome-de.jpg,,,, de_de,German-Germany,0
¡Bienvenido!,Gracias por unirte a nosotros,default,1,,,https://example.com/welcome-es.jpg,https://example.com/welcome-es.jpg,,,, es_es,Spanish-Spain,0
```

以下是自定义字段的示例

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
New Collection,Discover our latest products,default,1,,,,,,,"{"campaign":"summer2025","segment":"premium"}",en_us,English-United States,0
Nouvelle Collection,Découvrez nos derniers produits,default,1,,,,,,,"{"campaign":"summer2025","segment":"premium"}",fr_fr,French-France,0
```

>[!NOTE]
>
>对于包含轮播或操作按钮的富推送通知，Campaign使用与CSV导入不同的配置方法。 导入基本多语言内容后，直接在投放编辑器中配置富推送内容。

### CSV文件中的Personalization {#csv-personalization}

要在CSV内容中使用个性化字段，您需要使用`<span>`标记：

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
"Hello <span class=""nl-dce-field nl-dce-done"" data-nl-expr=""recipient.firstName"">recipient.firstName</span>","Your order has shipped!",,,,,,,,,,en_us,English-United States,0
"Bonjour <span class=""nl-dce-field nl-dce-done"" data-nl-expr=""recipient.firstName"">recipient.firstName</span>","Votre commande a été expédiée !",,,,,,,,,,fr_fr,French-France,0
```

在投放期间，Campaign会用实际的收件人数据替换这些占位符。

### 故障排除 {#csv-troubleshooting}

| 错误 | 原因 | 解决方案 |
|-------|-------|----------|
| 缺少所需的列 | CSV文件不包含所有14列 | 请确保CSV具有全部14列，且顺序完全符合上图。 对未使用的列使用空值。 |
| 区域设置/语言值无效 | 区域设置或语言列为空 | 区域设置和语言列必须具有每行的值 |
| 复制区域设置 | 同一区域设置代码出现多次 | 每个区域设置值必须是唯一的 — 删除重复行 |
| 文件编码问题 | CSV文件使用不兼容的编码 | 使用UTF-8编码保存CSV文件 |
| 列不匹配 | 行与标题的列数不同 | 确保所有行中的14列与标题完全匹配 |
| 无效的数值 | 徽章、isContentAvailable、isMutableContent或silentPush包含非数字值 | 仅使用数字：标记使用0或1，默认保留为空 |
| JSON格式不正确 | customFields列包含无效的JSON | 确保JSON语法正确： `{"key":"value"}`或留空 |
| 列名大小写不匹配 | 列名称不完全匹配 | 列名称区分大小写 — 使用上面显示的确切名称（例如，`badge`，而不是`Badge`或`BADGE`） |

>此[部分](#csv-best-practices)列出了最佳实践。 此[部分](#csv-columns)中详细介绍了列结构。
