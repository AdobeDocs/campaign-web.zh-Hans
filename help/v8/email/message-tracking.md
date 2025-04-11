---
audience: end-user
title: 跟踪您的邮件
description: 了解如何添加链接和跟踪已发送邮件
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 23%

---

# 添加链接和跟踪邮件 {#tracking}

使用电子邮件Designer向您的内容添加链接并跟踪发送的消息，从而允许您监控收件人的行为。

## 插入链接 {#insert-links}

设计邮件时，可以添加指向内容的链接。

>[!NOTE]
>
>启用跟踪后，将跟踪邮件内容中包含的所有链接。

要在电子邮件内容中插入链接，请执行以下步骤：

1. 选择一个元素，然后单击上下文工具栏中的&#x200B;**[!UICONTROL 插入链接]**。

1. 选择要创建的链接类型：

   ![屏幕截图显示用于在邮件跟踪工具中插入链接的接口](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL 外部链接]**：插入指向外部URL的链接。

     >[!AVAILABILITY]
     >
     >以下功能（链接到&#x200B;**[!UICONTROL 登陆页面]**、**[!UICONTROL 订阅链接]**&#x200B;和&#x200B;**[!UICONTROL 退订链接]**）在有限可用性(LA)中。 这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。

   * **[!UICONTROL 登陆页面]**：插入指向登陆页面的链接。 如果选择动态登陆页面（选择了&#x200B;**[!UICONTROL 来自URL的服务]**&#x200B;选项），则可以从列表中选择任何服务。 [了解详情](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![屏幕截图显示了链接到Email Designer中的登陆页面的界面](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL 订阅链接]**：插入订阅服务的链接。 当用户单击该链接时，会被定向到所选服务中引用的订阅登陆页面。 [了解详情](../audience/manage-services.md#create-service)

     ![屏幕截图，其中显示了用于在Service Tool中创建默认订阅链接的界面](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL 退订链接]**：插入退订服务的链接。 订阅者单击该链接时，会被定向到所选服务中引用的退订登陆页面。 [了解详情](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. 在相应字段中输入所需的URL，或者选择登陆页面或服务，然后定义链接设置和样式。

1. 添加&#x200B;**[!UICONTROL 标签]**&#x200B;和&#x200B;**[!UICONTROL 链接]**。

1. 保存您的更改。

1. 创建链接后，根据需要从&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中修改链接。

   * 编辑链接并更改其&#x200B;**[!UICONTROL 目标]**。
   * 选择是否通过勾选相应的选项为链接加下划线。

   ![显示用于修改消息跟踪工具中链接属性的设置界面的屏幕截图](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>营销类型的电子邮件必须包含一个选择退出链接，而事务性邮件不需要该链接。消息类别（**[!UICONTROL Marketing]**&#x200B;或&#x200B;**[!UICONTROL Transactional]**）在渠道表面级别和创建消息时定义。

在您的所有电子邮件中都加入指向镜像页面的特定链接。 在[此章节](mirror-page.md)中详细了解镜像页面。

## 管理跟踪 {#manage-tracking}

[电子邮件Designer](create-email-content.md)允许您管理跟踪的URL，例如编辑每个链接的跟踪类型。

1. 单击左窗格中的&#x200B;**[!UICONTROL 链接]**&#x200B;图标，以显示要跟踪的内容中所有URL的列表。

   此列表提供了一个集中式视图，并有助于找到电子邮件内容中的每个URL。

1. 要编辑链接，请单击相应的铅笔图标。

   ![显示用于编辑邮件跟踪工具中链接的界面的屏幕截图](assets/message-tracking-edit-links.png){zoomable="yes"}

1. 根据需要修改&#x200B;**[!UICONTROL 跟踪类型]**：

   ![屏幕截图显示了用于编辑邮件跟踪工具中的跟踪类型的界面](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   对于每个跟踪的URL，请将跟踪模式设置为以下值之一：

   * **[!UICONTROL 已跟踪]**：激活此URL的跟踪。
   * **[!UICONTROL 选择退出]**：将此URL标记为选择退出或退订URL。
   * **[!UICONTROL 镜像页面]**：将此URL标记为镜像页面URL。
   * **[!UICONTROL 从不]**：阻止跟踪此URL。<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 向链接添加&#x200B;**[!UICONTROL 类别]**&#x200B;以分组跟踪链接，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![屏幕截图显示了向邮件跟踪工具中的跟踪链接添加类别的界面](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. 发送您的投放后，访问您的投放报告。在&#x200B;**[!UICONTROL 跟踪]**&#x200B;菜单下方，**[!UICONTROL URL 和点击流]**&#x200B;报告显示了投放中访问次数最多的 URL。[了解详情](../reporting/gs-reports.md)