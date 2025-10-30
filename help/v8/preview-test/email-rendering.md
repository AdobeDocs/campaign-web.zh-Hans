---
audience: end-user
title: 测试电子邮件渲染
description: 了解如何在Campaign Web用户界面中测试电子邮件渲染
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 2%

---

# 测试电子邮件渲染 {#email-rendering}

在发送电子邮件之前，请确保消息以最佳方式显示在各种Web客户端和设备中的收件人。

要实现此目的，请使用&#x200B;**中您的** Litmus[!DNL Adobe Campaign]帐户，在不同上下文中即时预览电子邮件渲染。 这允许您检查与主要桌面应用程序、Web邮件服务、移动设备等的兼容性。

>[!CAUTION]
>
>在Campaign中使用电子邮件渲染会向第三方系统发送验证。 将您的Litmus帐户与[!DNL Campaign]连接后，即表示您确认Adobe对您可能发送到该第三方的任何数据不承担任何责任。 Litmus的电子邮件数据保留策略适用于这些电子邮件，包括可能包含在这些验证中的个性化数据。 要访问或删除此类数据，请直接与Litmus联系。

要访问电子邮件渲染功能，请完成以下先决条件：

* 拥有Litmus帐户。
* 选择配置文件和/或测试配置文件。 在[本节](preview-content.md)中了解详情。

然后，执行以下步骤。

1. 在[编辑内容](../email/edit-content.md)屏幕或[电子邮件Designer](../email/get-started-email-designer.md)中，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮。

1. 选择&#x200B;**[!UICONTROL 渲染电子邮件]**&#x200B;按钮。

   在电子邮件编辑器中![模拟内容按钮](assets/simulate-rendering-button.png){zoomable="yes"}

1. 单击右上角的&#x200B;**连接您的Litmus帐户**。

   电子邮件渲染界面中的![Litmus帐户连接选项](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. 输入您的凭据并登录。

   ![Litmus帐户登录屏幕](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. 单击&#x200B;**运行测试**&#x200B;按钮以生成电子邮件预览。

1. 在常用的桌面、移动和基于Web的客户端中查看电子邮件内容。

   ![跨不同客户端的电子邮件渲染预览](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile, and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![Preview pane showing email rendering across selected clients](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->