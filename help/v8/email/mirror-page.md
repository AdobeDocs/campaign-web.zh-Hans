---
audience: end-user
title: 添加指向镜像页面的链接
description: 了解如何添加和管理指向镜像页面的链接
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 16%

---

# 镜像页面 {#mirror-page}

镜像页面是电子邮件的在线版本。 在电子邮件营销中，最佳做法是添加指向镜像页面的链接。 例如，如果用户在收件箱中查看电子邮件时遇到渲染问题或图像损坏，则可以访问电子邮件的镜像页面。 出于无障碍原因或鼓励社交共享的原因，还建议提供在线版本。

Adobe Campaign生成的镜像页面包含所有个性化数据。

![电子邮件中的镜像链接示例](assets/mirror-page-link.png){width="600" align="left"}

## 添加指向镜像页面的链接 {#link-to-mirror-page}

在Adobe Campaign中，使用专用的&#x200B;**个性化块**&#x200B;在电子邮件内容中插入指向镜像页面的链接。 内置的&#x200B;**指向镜像页面的链接**&#x200B;个性化块会在电子邮件内容中插入以下代码：`<%@ include view='MirrorPage' %>`。

要在电子邮件中添加指向镜像页面的链接，请执行以下步骤：

1. 选择一个元素（文本或图像），然后单击上下文工具栏中的&#x200B;**[!UICONTROL 插入链接]**。

   ![显示“插入链接”选项的上下文工具栏](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. 选择&#x200B;**[!UICONTROL 添加个性化]**&#x200B;图标以访问个性化菜单。

   Adobe Campaign中的![Personalization菜单](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. 从&#x200B;**[!UICONTROL 片段]**&#x200B;菜单中，选择&#x200B;**[!UICONTROL 镜像页面URL]**，然后单击&#x200B;**[!UICONTROL 添加]**。 [了解如何使用表达式片段](../content/use-expression-fragments.md)

   “片段”菜单中的![镜像页面URL选项](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

镜像页面是自动创建的。

发送电子邮件后，单击镜像页面链接的收件人会看到其默认Web浏览器中显示的电子邮件内容。

默认情况下，镜像页面的保留期为&#x200B;**60天**。 在此时段后，镜像页面不再可用。

>[!CAUTION]
>
>* 镜像页面链接是自动生成的，无法编辑。 其中包括呈现原始电子邮件所需的所有加密个性化数据。 使用值较大的个性化属性可能会生成过长的镜像页面URL，从而阻止链接在URL长度最大化的Web浏览器中工作。
>
>* 在发送到测试用户档案的验证中，指向镜像页面的链接无效。 它仅在最终消息中处于活动状态。

## 镜像页面生成 {#mirror-page-generation}

默认情况下，如果电子邮件内容不为空并且包含指向镜像页面的链接（也称为镜像链接），Adobe Campaign会自动生成镜像页面。

通过投放属性中可用的选项控制电子邮件镜像页面的生成模式。 [了解详情](../advanced-settings/delivery-settings.md#mirror)