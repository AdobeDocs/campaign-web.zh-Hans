---
audience: end-user
title: 跟踪邮件
description: 了解如何添加链接和跟踪已发送的消息
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: c1d433ba1d12e840c5ae219b319e80c1bcdc7686
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# 添加链接和跟踪消息 {#tracking}

>[!NOTE]
>
>此文档正在构建中并且经常更新。 此内容的最终版本将于2023年1月准备就绪。

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

## 链接到镜像页面 {#mirror-page}

镜像页面是可通过Web浏览器在线访问的HTML页面。 其内容与电子邮件的内容相同。

要在电子邮件中添加指向镜像页面的链接，请执行以下操作：

1. 选择元素并单击 **[!UICONTROL 插入链接]** 中。

   ![](assets/message-tracking-mirror-page.png)

1. 选择 **[!UICONTROL 插入链接]** 图标以访问个性化菜单。

   ![](assets/message-tracking-mirror-page_2.png)

1. 从 **[!UICONTROL 内容块]** 菜单，选择 **[!UICONTROL 镜像页面URL]** 单击 **[!UICONTROL 添加]**.

   ![](assets/message-tracking-mirror-page_3.png)

将自动创建镜像页面。

>[!IMPORTANT]
>
>镜像页面链接是自动生成的，无法编辑。 它们包含呈现原始电子邮件所需的所有加密个性化数据。 因此，使用具有大值的个性化属性可能会生成较长的镜像页面URL，这会阻止该链接在URL长度最大的Web浏览器中工作。

发送电子邮件后，当收件人单击镜像页面链接时，电子邮件的内容会显示在其默认的Web浏览器中。

>[!NOTE]
>
>在发送到测试用户档案的校样中，指向镜像页面的链接不处于活动状态。 它仅在最终消息中激活。

镜像页面的保留期为60天。 延迟后，镜像页面将不再可用。

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
