---
audience: end-user
title: 编辑电子邮件内容
description: 了解如何在 Campaign Web UI 中编辑电子邮件内容
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: f04e8aa5ecb12fca02da640b0037441d4cd7d4d3
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 69%

---

# 编辑电子邮件内容 {#configure-content}

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

要开始创建电子邮件内容，请单击电子邮件创建屏幕上的&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。[](../email/create-email.md)

![](assets/email-edit-content.png)

打开的屏幕允许您定义基本详细信息、执行一些其他操作（如添加附件或设置优惠），以及访问Email Designer以构建内容。

![](assets/email-edit-content-dashboard.png)

编辑电子邮件内容的步骤如下：

1. 在 **[!UICONTROL 发件人姓名]** 字段中，使用易于收件人识别的名称（如您的品牌名称）来提高投放的打开率。

1. 定义电子邮件&#x200B;**[!UICONTROL 主题行]**。要执行该操作，请直接在专用字段中键入您的主题，或打开表达式编辑器以使用各种属性和内容块或优惠来定义或添加个性化内容。[了解如何个性化内容](../personalization/personalize.md)
为进一步改善收件人的体验，您可以添加一个人的姓名，例如“Emma from Megastore”。

1. 在 **[!UICONTROL 发件人电子邮件]** 地址字段，确保地址域与您委派给Adobe的子域相同。

   您可以更改“@”之前的部分，但不能更改域地址。

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. 定义电子邮件&#x200B;**[!UICONTROL 主题行]**。在专用字段中直接键入主题，或打开表达式编辑器以使用各种属性和内容块或选件添加个性化。 [了解如何个性化内容](../personalization/personalize.md)

1. 如果要将文件附加到电子邮件，请单击&#x200B;**[!UICONTROL 添加附件]**&#x200B;按钮，然后选择一个或多个文件。

   >[!NOTE]
   >
   >    为了避免出现性能问题，建议每封电子邮件不要附加多个附件。

   <!--limitation on size + number of files?-->

1. 如果要使用电子邮件发送优惠，请使用&#x200B;**[!UICONTROL 设置优惠]**&#x200B;按钮。

   之后，您可以使用个性化字段将它们插入电子邮件中。[了解如何发送优惠](offers.md)

1. 单击&#x200B;**[!UICONTROL 编辑电子邮件正文]**&#x200B;按钮以构造和设计电子邮件内容。有关如何设计电子邮件内容的其他信息，请参阅以下章节：

   * [了解如何设计电子邮件](create-email-content.md)
   * [设置内容的样式](get-started-email-style.md)

1. 默认情况下，为投放启用跟踪。您可以从&#x200B;**[!UICONTROL 可选功能]**&#x200B;部分中禁用此选项。[了解如何添加链接和管理跟踪](message-tracking.md)

1. 定义电子邮件的内容后，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以在发送内容前检查其显示方式。[了解如何预览和测试电子邮件](../preview-test/preview-test.md)
