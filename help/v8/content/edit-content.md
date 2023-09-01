---
audience: end-user
title: 编辑电子邮件内容
description: 了解如何在 Campaign Web UI 中编辑电子邮件内容
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 50%

---

# 配置电子邮件内容 {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="创建电子邮件内容"
>abstract="通过此部分，您可以为电子邮件创建内容，并使用电子邮件设计器为其赋予精美外观。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="电子邮件参数"
>abstract="在电子邮件模板中定义“发件人姓名”和“发件人电子邮件”值。可以使用表达式编辑器对主题行进行个性化设置。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="电子邮件附件"
>abstract="选择要在邮件中插入的一个或多个文件。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="跟踪选项"
>abstract="默认情况下，为投放启用跟踪。您可以从此处禁用该选项。"

电子邮件 **[!UICONTROL 编辑内容]** 屏幕允许您：
* 定义消息的基本元素，如发件人地址和主题行
* 执行其他操作，例如添加附件或设置优惠
* 访问 [电子邮件设计工具](get-started-email-designer.md#start-authoring) 以开始构建电子邮件的适当内容

要配置或编辑电子邮件的内容，请执行以下步骤。

1. 单击 **[!UICONTROL 编辑内容]** 按钮来自 [电子邮件投放仪表板](../email/create-email.md) 屏幕。

   ![](assets/email-edit-content-button.png)

1. 此时将打开电子邮件内容编辑屏幕。

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >如果您正在配置新电子邮件，则 **[!UICONTROL 发件人姓名]** 和 **[!UICONTROL 发件人电子邮件]** 已填充字段。

1. 此 **[!UICONTROL 发件人姓名]** 字段在电子邮件模板中定义。 如果要对其进行修改，请使用易于收件人识别的名称（如您的品牌名称）来增加投放的打开率。

   >[!NOTE]
   >
   >要进一步改善收件人的体验，您可以添加人员的姓名，例如“Eve from Luma”。

1. 此 **[!UICONTROL 发件人电子邮件]** 地址字段也在电子邮件模板中定义。 确保地址域与您委派给Adobe的子域相同。

   >[!NOTE]
   >
   >您可以更改“@”之前的部分，但不能更改域地址。

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. 定义电子邮件&#x200B;**[!UICONTROL 主题行]**。在专用字段中直接键入主题，或打开表达式编辑器以使用各种属性和内容块或选件添加个性化。 [了解如何个性化内容](../personalization/personalize.md)

1. 如果要将文件附加到电子邮件，请单击&#x200B;**[!UICONTROL 添加附件]**&#x200B;按钮，然后选择一个或多个文件。

   >[!NOTE]
   >
   >    为了避免出现性能问题，建议每封电子邮件不要附加多个附件。

   <!--limitation on size + number of files?-->

1. 如果要使用电子邮件发送优惠，请使用&#x200B;**[!UICONTROL 设置优惠]**&#x200B;按钮。

   之后，您可以使用个性化字段将它们插入电子邮件中。[了解如何发送优惠](offers.md)

1. 单击 **[!UICONTROL 编辑电子邮件正文]** 按钮，使用来结构和设计电子邮件的内容 [电子邮件设计工具](#start-authoring). 有关如何设计电子邮件内容的其他信息，请参阅以下章节：

   * [从头开始创作电子邮件](create-email-content.md)
   * [设置内容的样式](get-started-email-style.md)

   >[!NOTE]
   >
   >您还可以将鼠标悬停在电子邮件预览上并选择 **[!UICONTROL 打开电子邮件设计器]**.

1. 默认情况下，为投放启用跟踪。您可以从&#x200B;**[!UICONTROL 可选功能]**&#x200B;部分中禁用此选项。[了解如何添加链接和管理跟踪](message-tracking.md)

1. 定义电子邮件的内容后，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以在发送内容前检查其显示方式。[了解如何预览和测试电子邮件](../preview-test/preview-test.md)

