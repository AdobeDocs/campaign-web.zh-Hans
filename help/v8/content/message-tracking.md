---
audience: end-user
title: 跟踪邮件
description: 了解如何添加链接和跟踪已发送的消息
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha" type="Informitive"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# 添加链接和跟踪消息 {#tracking}

使用Email designer添加指向内容的链接并跟踪发送的消息，以监控收件人的行为。

## 插入链接 {#insert-links}

在设计消息时，您可以添加指向内容的链接。

>[!NOTE]
>
>启用跟踪后，将跟踪消息内容中包含的所有链接。

要在电子邮件内容中插入链接，请执行以下步骤：

1. 选择元素并单击 **[!UICONTROL 插入链接]** 中。

   ![](assets/message-tracking-insert-link.png)

1. 添加 **[!UICONTROL 标签]** 和 **[!UICONTROL 链接]**.

1. 保存更改。

1. 创建链接后，您仍可以从 **[!UICONTROL 组件设置]** 窗格。

   * 您可以编辑链接并更改其 **[!UICONTROL Target]**.
   * 您可以通过选中相应的选项来选择是否为链接添加下划线。

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>营销类型电子邮件必须包含选择退出链接，这对于事务型消息不是必需的。 消息类别(**[!UICONTROL 营销]** 或 **[!UICONTROL 事务型]**)在渠道表面（即消息预设）级别定义，并在创建消息时定义。

应在所有电子邮件中添加指向镜像页面的特定链接。 了解有关镜像页面的更多信息，请参阅 [此部分](mirror-page.md).

## 管理跟踪 {#manage-tracking}

的 [Email Designer](create-email-content.md) 用于管理跟踪的URL，例如编辑每个链接的跟踪类型。

1. 单击 **[!UICONTROL 链接]** 图标，以显示要跟踪的内容的所有URL的列表。

   利用此列表，可以集中查看并查找电子邮件内容中的每个URL。

1. 要编辑链接，请单击相应的铅笔图标。

   ![](assets/message-tracking-edit-links.png)

1. 您可以修改 **[!UICONTROL 跟踪类型]** （如果需要）：

   ![](assets/message-tracking-edit-a-link.png)

   对于每个跟踪的URL，您可以将跟踪模式设置为以下值之一：

   * **[!UICONTROL 跟踪]**:在此URL上激活跟踪。
   * **[!UICONTROL 选择禁用]**:将此URL视为选择退订或退订URL。
   * **[!UICONTROL 镜像页面]**:将此URL视为镜像页面URL。
   * **[!UICONTROL 从不]**:从不激活此URL的跟踪。 <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 添加 **[!UICONTROL 类别]** 链接，以将跟踪链接分组，然后单击 **[!UICONTROL 保存]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. 发送投放后，访问投放报告。 在 **[!UICONTROL 跟踪]** 菜单 **[!UICONTROL URL和点击流]** 报表显示投放中哪些URL的访问次数最多。 [了解详情](../reporting/reports.md)
