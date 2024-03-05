---
audience: end-user
title: 添加指向镜像页面的链接
description: 了解如何添加和管理指向镜像页面的链接
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 96%

---

# 添加指向镜像页面的链接{#mirror-page}

镜像页面是电子邮件的在线版本。

大多数电子邮件客户端可以轻松渲染图像，但出于安全原因，某些预设可以避免显示图像。例如，如果用户尝试在收件箱中查看电子邮件时遇到渲染问题或损坏的图像，则可以浏览到电子邮件的镜像页面。此外，建议提供在线版本以方便访问或鼓励社交共享。

Adobe Campaign 生成的镜像页面包含所有个性化数据。

![镜像链接示例](assets/mirror-page-link.png){width="600" align="left"}

## 添加指向镜像页面的链接{#link-to-mirror-page}

插入指向镜像页面的链接是一种好的做法。例如，此链接可以是“在浏览器中查看此电子邮件”或“在线阅读此电子邮件”。它通常位于电子邮件的页眉或页脚。

在 Adobe Campaign 中，您可以使用专用&#x200B;**个性化块**&#x200B;在电子邮件内容中插入指向镜像页面的链接。内置的&#x200B;**指向镜像页面的链接**&#x200B;个性化块会在电子邮件内容中插入以下代码：`<%@ include view='MirrorPage' %>`。

要在电子邮件中添加指向镜像页面的链接，请执行以下操作：

1. 选择一个元素，并单击上下文工具栏中的&#x200B;**[!UICONTROL 插入链接]**。

   ![](assets/message-tracking-mirror-page.png){zoomable=&quot;yes&quot;}

1. 选择&#x200B;**[!UICONTROL 添加个性化]**&#x200B;图标以访问个性化菜单。

   ![](assets/message-tracking-mirror-page_2.png){zoomable=&quot;yes&quot;}

1. 从&#x200B;**[!UICONTROL 内容块]**&#x200B;菜单中，选择&#x200B;**[!UICONTROL 镜像页面 URL]**，然后单击&#x200B;**[!UICONTROL 添加]**。

   ![](assets/message-tracking-mirror-page_3.png){zoomable=&quot;yes&quot;}

   有关自定义内容块插入的更多信息，请参阅[此章节](../personalization/personalize.md#personalize-emails)。

镜像页面是自动创建的。

>[!IMPORTANT]
>
>镜像页面链接是自动生成的，并且无法编辑。它们包含渲染原始电子邮件所需的所有加密的个性化数据。因此，使用具有较大值的个性化属性可能会生成冗长的镜像页面 URL，从而导致无法在具有最大 URL 长度限制的 Web 浏览器中访问链接。

发送电子邮件后，当收件人单击镜像页面链接时，电子邮件的内容将显示在他们的默认 Web 浏览器中。

>[!NOTE]
>
>在发送到测试用户档案的验证中，指向镜像页面的链接无效。 它仅在最终邮件中激活。

默认情况下，镜像页面的保留期为 60 天。在此延迟之后，镜像页面将不再可用。


## 镜像页面生成{#mirror-page-generation}

默认情况下，如果电子邮件内容不为空，并且包含指向镜像页面的链接（也称为镜像链接），则 Adobe Campaign 会自动生成镜像页面。

您可以控制电子邮件镜像页面的生成方式。投放属性中提供了选项。[了解详情](../advanced-settings/delivery-settings.md#mirror)
