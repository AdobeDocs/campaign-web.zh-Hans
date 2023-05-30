---
audience: end-user
title: 跟踪您的邮件
description: 了解如何添加链接和跟踪已发送邮件
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha" type="Positive"
source-git-commit: 0703b872bb8f452773e76f2524d47bf774c687e0
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 96%

---

# 添加链接和跟踪邮件 {#tracking}

使用电子邮件设计器将链接添加到内容，并跟踪已发送邮件以监控收件人的行为。

## 插入链接 {#insert-links}

设计邮件时，可以添加指向内容的链接。

>[!NOTE]
>
>启用跟踪后，将跟踪邮件内容中包含的所有链接。

要在电子邮件内容中插入链接，请执行以下步骤：

1. 选择一个元素，并单击上下文工具栏中的&#x200B;**[!UICONTROL 插入链接]**。

   ![](assets/message-tracking-insert-link.png)

1. 添加&#x200B;**[!UICONTROL 标签]**&#x200B;和&#x200B;**[!UICONTROL 链接]**。

1. 保存您的更改。

1. 创建链接后，您仍然可以从以下位置对其进行修改： **[!UICONTROL 设置]** 选项卡。

   * 可以编辑链接并更改其&#x200B;**[!UICONTROL 目标]**。
   * 可以通过选中相应的选项来选择是否为链接加下划线。

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>营销类型的电子邮件必须包含一个选择退出链接，而事务性邮件不需要该链接。邮件类别（**[!UICONTROL 营销]**&#x200B;或&#x200B;**[!UICONTROL 事务性]**）在渠道表面（即邮件预设）级别以及创建邮件时进行定义。

应在所有电子邮件中添加指向镜像页面的特定链接。在[此章节](mirror-page.md)中详细了解镜像页面。

## 管理跟踪 {#manage-tracking}

[电子邮件设计器](create-email-content.md)允许您管理跟踪的 URL，例如编辑每个链接的跟踪类型。

1. 单击左侧窗格中的&#x200B;**[!UICONTROL 链接]**&#x200B;图标以显示要跟踪的内容的所有 URL 的列表。

   此列表提供一个集中式视图，让您能够找到电子邮件内容中的每个 URL。

1. 要编辑链接，请单击相应的铅笔图标。

   ![](assets/message-tracking-edit-links.png)

1. 如果需要，可以修改&#x200B;**[!UICONTROL 跟踪类型]**：

   ![](assets/message-tracking-edit-a-link.png)

   对于每个跟踪的 URL，可以将跟踪模式设置为下列值之一：

   * **[!UICONTROL 已跟踪]**：激活对此 URL 的跟踪。
   * **[!UICONTROL 选择禁用]**：将此 URL 视为选择退出或退订 URL。
   * **[!UICONTROL 镜像页面]**：将此 URL 视为镜像页面 URL。
   * **[!UICONTROL 从不]**：从不激活对此 URL 的跟踪。<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 将&#x200B;**[!UICONTROL 类别]**&#x200B;添加到链接以对跟踪的链接进行分组，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/message-tracking-edit-a-link_2.png)

1. 发送您的投放后，访问您的投放报告。在&#x200B;**[!UICONTROL 跟踪]**&#x200B;菜单下方，**[!UICONTROL URL 和点击流]**&#x200B;报告显示了投放中访问次数最多的 URL。[了解详情](../reporting/gs-reports.md)
