---
audience: end-user
title: 跟踪您的邮件
description: 了解如何添加链接和跟踪已发送邮件
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 66%

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

1. 选择要创建的链接类型：

   ![](assets/message-tracking-insert-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL 外部链接]**：插入指向外部URL的链接。

     >[!AVAILABILITY]
     >
     >以下功能(链接到 **[!UICONTROL 登陆页面]**， **[!UICONTROL 订阅链接]** 和 **[!UICONTROL 退订链接]**)在有限可用性(LA)中。 它们仅限于迁移的客户 **从Adobe Campaign Standard到Adobe Campaign v8**&#x200B;和无法部署在任何其他环境中。

   * **[!UICONTROL 登陆页面]**：插入指向登陆页面的链接。 如果您选择动态登陆页面(使用 **[!UICONTROL 来自URL的服务]** 选项)，您可以从列表中选择任何服务。 [了解详情](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL 订阅链接]**：插入指向订阅服务的链接。 当用户单击该链接时，将被定向到所选服务中引用的订阅登陆页面。 [了解详情](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL 退订链接]**：插入指向退订服务的链接。 当订阅者单击该链接时，将被定向到所选服务中引用的退订登陆页面。 [了解详情](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. 在相应字段中输入所需的URL，或者选择登陆页面或服务，然后定义链接设置和样式。

1. 添加&#x200B;**[!UICONTROL 标签]**&#x200B;和&#x200B;**[!UICONTROL 链接]**。

1. 保存您的更改。

1. 创建链接后，仍可以从&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡修改它。

   * 可以编辑链接并更改其&#x200B;**[!UICONTROL 目标]**。
   * 可以通过选中相应的选项来选择是否为链接加下划线。

   ![](assets/message-tracking-link-settings.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>营销类型的电子邮件必须包含一个选择退出链接，而事务性邮件不需要该链接。消息类别(**[!UICONTROL 营销]** 或 **[!UICONTROL 事务性]**)在渠道平面级别和创建消息时定义。

应在所有电子邮件中添加指向镜像页面的特定链接。在[此章节](mirror-page.md)中详细了解镜像页面。

## 管理跟踪 {#manage-tracking}

[电子邮件设计器](create-email-content.md)允许您管理跟踪的 URL，例如编辑每个链接的跟踪类型。

1. 单击左侧窗格中的&#x200B;**[!UICONTROL 链接]**&#x200B;图标以显示要跟踪的内容的所有 URL 的列表。

   此列表提供一个集中式视图，让您能够找到电子邮件内容中的每个 URL。

1. 要编辑链接，请单击相应的铅笔图标。

   ![](assets/message-tracking-edit-links.png){zoomable=&quot;yes&quot;}

1. 如果需要，可以修改&#x200B;**[!UICONTROL 跟踪类型]**：

   ![](assets/message-tracking-edit-a-link.png){zoomable=&quot;yes&quot;}

   对于每个跟踪的 URL，可以将跟踪模式设置为下列值之一：

   * **[!UICONTROL 已跟踪]**：激活对此 URL 的跟踪。
   * **[!UICONTROL 选择禁用]**：将此 URL 视为选择退出或退订 URL。
   * **[!UICONTROL 镜像页面]**：将此 URL 视为镜像页面 URL。
   * **[!UICONTROL 从不]**：从不激活对此 URL 的跟踪。<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 将&#x200B;**[!UICONTROL 类别]**&#x200B;添加到链接以对跟踪的链接进行分组，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/message-tracking-edit-a-link_2.png){zoomable=&quot;yes&quot;}

1. 发送您的投放后，访问您的投放报告。在&#x200B;**[!UICONTROL 跟踪]**&#x200B;菜单下方，**[!UICONTROL URL 和点击流]**&#x200B;报告显示了投放中访问次数最多的 URL。[了解详情](../reporting/gs-reports.md)
