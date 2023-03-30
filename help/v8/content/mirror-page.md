---
audience: end-user
title: 添加指向镜像页面的链接
description: 了解如何添加和管理指向镜像页面的链接
source-git-commit: b85bf75da466502e4579a061c02a2c4ce4361cd5
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


# 添加指向镜像页面的链接{#mirror-page}

## 关于镜像页面{#about-mirror-page}

镜像页面是您电子邮件的在线版本。

虽然大多数电子邮件客户端在渲染图像时没有出现问题，但出于安全原因，某些预设可以避免显示图像。 用户可以浏览电子邮件的镜像页面，例如，当他们尝试在收件箱中查看电子邮件时遇到呈现问题或图像损坏时。 还建议出于无障碍原因提供在线版本，或鼓励社交共享。

由Adobe Campaign生成的镜像页面包含所有个性化数据。

![镜像链接示例](assets/mirror-page-link.png){width="600" align="left"}

## 添加指向镜像页面的链接{#link-to-mirror-page}

插入指向镜像页面的链接是一种好做法。 此链接可以是“在浏览器中查看此电子邮件”或“在线阅读此内容”。 它通常位于电子邮件的页眉或页脚。

在Adobe Campaign中，您可以使用 **个性化块**. 内置 **链接到镜像页面** 个性化块在电子邮件内容中插入以下代码： `<%@ include view='MirrorPage' %>`.


要在电子邮件中添加指向镜像页面的链接，请执行以下操作：

1. 选择元素并单击 **[!UICONTROL 插入链接]** 中。

   ![](assets/message-tracking-mirror-page.png)

1. 选择 **[!UICONTROL 插入链接]** 图标以访问个性化菜单。

   ![](assets/message-tracking-mirror-page_2.png)

1. 从 **[!UICONTROL 内容块]** 菜单，选择 **[!UICONTROL 镜像页面URL]** 单击 **[!UICONTROL 添加]**.

   ![](assets/message-tracking-mirror-page_3.png)

   有关自定义内容块插入的更多信息，请参阅 [此部分](../personalization/personalize.md#personalize-emails).

将自动创建镜像页面。

>[!IMPORTANT]
>
>镜像页面链接是自动生成的，无法编辑。 它们包含呈现原始电子邮件所需的所有加密个性化数据。 因此，使用具有大值的个性化属性可能会生成较长的镜像页面URL，这会阻止该链接在URL长度最大的Web浏览器中工作。

发送电子邮件后，当收件人单击镜像页面链接时，电子邮件的内容会显示在其默认的Web浏览器中。

>[!NOTE]
>
>在发送给测试用户档案的测试电子邮件中，指向镜像页面的链接不处于活动状态。 它仅在最终消息中激活。

默认情况下，镜像页面的保留期为60天。 延迟后，镜像页面将不再可用。


## 镜像页面生成{#mirror-page-generation}

默认情况下，如果电子邮件内容不为空，并且包含指向镜像页面的链接（即镜像链接），则Adobe Campaign会自动生成镜像页面。

您可以控制电子邮件镜像页面的生成模式。 提交属性中提供了相应选项。 [了解详情](../advanced-settings/delivery-settings.md#mirror)
