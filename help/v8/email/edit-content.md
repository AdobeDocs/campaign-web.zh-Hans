---
audience: end-user
title: 编辑电子邮件内容
description: 了解如何在Campaign Web用户界面中编辑电子邮件内容
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 35%

---

# 配置电子邮件内容 {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="定义电子邮件的内容"
>abstract="通过&#x200B;**编辑内容**&#x200B;屏幕，可定义消息的基本元素（如发件人地址和主题行）、执行其他操作（如添加附件或产品建议）和访问电子邮件 Designer 以美化邮件的外观。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="设置电子邮件属性"
>abstract="通过&#x200B;**基本详细信息**&#x200B;部分，可更新发件人的地址和回复地址以及使用表达式编辑器定义主题行。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="将文件附加到电子邮件"
>abstract="选择要插入邮件的一个或多个文件。为了避免出现性能问题，建议每封电子邮件不要附加多个附件。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="编辑跟踪"
>abstract="默认情况下为投放启用跟踪，这表示将跟踪在邮件内容中包括的所有链接。您可以从此处禁用该选项。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="添加链接和跟踪邮件"

电子邮件&#x200B;**[!UICONTROL 编辑内容]**&#x200B;屏幕允许您：

* 定义消息的基本元素，如发件人地址和主题行
* 执行其他操作，例如添加附件或设置优惠
* 访问[电子邮件Designer](get-started-email-designer.md#start-authoring)以开始生成电子邮件的适当内容
* 向投放添加语言变体。 [了解更多信息](../msg/multilingual.md)

>[!NOTE]
>
>可使用个性化字段填写此屏幕的所有可编辑文本字段。 [了解如何个性化内容](../personalization/personalize.md)

## 配置投放

要配置或编辑电子邮件的内容，请执行以下步骤。

1. 从&#x200B;**[!UICONTROL 电子邮件投放仪表板]**&#x200B;屏幕单击[编辑内容](../email/create-email.md)按钮。

   ![在电子邮件投放仪表板上显示“编辑内容”按钮的屏幕截图。](assets/email-edit-content-button.png){zoomable="yes"}

1. 此时将打开电子邮件内容编辑屏幕。

   ![显示电子邮件内容版本仪表板的屏幕截图。](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >如果配置新电子邮件，则已填充&#x200B;**[!UICONTROL 发件人姓名]**&#x200B;和&#x200B;**[!UICONTROL 发件人电子邮件]**&#x200B;字段。

1. 在电子邮件模板中定义了&#x200B;**[!UICONTROL 发件人姓名]**&#x200B;字段。 如果要对其进行修改，请使用易于收件人识别的名称（如您的品牌名称）来增加投放的打开率。

   >[!NOTE]
   >
   >要进一步改善收件人的体验，您可以添加人员的姓名，例如“Eve from Luma”。

1. **[!UICONTROL 发件人电子邮件]**&#x200B;地址字段也在电子邮件模板中定义。 确保地址域与您委派给Adobe的子域匹配。

   >[!NOTE]
   >
   >您可以更改“@”之前的部分，但不能更改域地址。

1. 展开&#x200B;**[!UICONTROL 回复字段]**&#x200B;部分。 默认情况下，答复使用发件人姓名和地址。 但是，Adobe建议使用现有的真实地址，例如您品牌的客户关怀地址。 在这种情况下，如果收件人发送回复，客户关怀团队将能够处理。

   ![显示电子邮件内容编辑器中“回复字段”部分的屏幕截图。](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. 定义电子邮件&#x200B;**[!UICONTROL 主题行]**。在专用字段中直接键入您的主题，或者打开表达式编辑器以使用各种属性、表达式片段或选件添加[个性化](../personalization/personalize.md)。

1. 如果要将文件附加到电子邮件，请单击&#x200B;**[!UICONTROL 添加附件]**&#x200B;按钮，然后选择一个或多个文件。

   >[!NOTE]
   >
   >为了避免出现性能问题，建议每封电子邮件不要附加多个附件。

   <!--limitation on size + number of files?-->

1. 如果要通过电子邮件发送优惠，请使用&#x200B;**[!UICONTROL 设置优惠]**&#x200B;按钮选择它们。

   然后，您可以使用个性化字段将它们插入到电子邮件中。 [了解如何发送产品建议](../msg/offers.md)

## 编辑电子邮件正文

1. 单击&#x200B;**[!UICONTROL 编辑电子邮件正文]**&#x200B;按钮可使用[电子邮件Designer](get-started-email-designer.md#start-authoring)来构造和设计电子邮件的内容。

   >[!NOTE]
   >
   >您还可以将鼠标悬停在电子邮件预览上并选择&#x200B;**[!UICONTROL 打开电子邮件设计器]**。


   有关如何设计电子邮件内容的其他信息，请参阅以下章节：

   * [从头开始创作电子邮件](create-email-content.md)
   * [设置内容的样式](get-started-email-style.md)

1. 默认情况下，为投放启用跟踪。您可以从&#x200B;**[!UICONTROL 可选功能]**&#x200B;部分中禁用此选项。[了解如何添加链接和管理跟踪](message-tracking.md)

1. 定义电子邮件的内容后，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以在发送内容前检查其显示方式。您还可以验证内容质量，以评估可读性、CTA效果和整体质量。 [了解有关内容质量验证的更多信息](../content/brands-score.md#validate-quality)

1. [了解如何预览和测试电子邮件](../preview-test/preview-test.md)。
