---
audience: end-user
title: 测试电子邮件渲染
description: 了解如何在 Campaign Web UI 中测试电子邮件渲染
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 8%

---


# 测试电子邮件渲染 {#email-rendering}

在发送电子邮件之前，请确保以最佳方式在各种Web客户端和设备上向收件人显示您的消息。

为此，您可以利用 **利特默斯** 帐户至 [!DNL Adobe Campaign] 即时预览不同上下文中的电子邮件呈现，并检查主要桌面和应用程序（Web邮件、消息服务、移动设备等）中的兼容性。

>[!CAUTION]
>
>在Campaign中使用电子邮件渲染会向第三方系统发送测试电子邮件。 将您的Litmus帐户与 [!DNL Campaign]，则您确认该Adobe对您可能发送给该第三方的任何数据概不负责。 Litmus数据保留电子邮件策略适用于这些电子邮件，包括可能包含在这些测试消息中的个性化数据。 要访问或删除此类数据，您需要直接联系Litmus。

要访问电子邮件渲染功能，您需要：

* 拥有Litmus帐户
* 选择测试配置文件 — 了解如何 [本节](preview-content.md)

然后，执行以下步骤。

1. 在 [编辑内容](../content/edit-content.md) 屏幕或 [电子邮件设计工具](../content/get-started-email-designer.md)，单击 **[!UICONTROL 模拟内容]** 按钮。

1. 选择 **[!UICONTROL 呈现电子邮件]** 按钮。

   ![](assets/simulate-rendering-button.png)

1. 单击 **连接您的Litmus帐户** 在右上角。

   ![](assets/simulate-rendering-litmus.png)

1. 输入您的凭据并登录。

   ![](assets/simulate-rendering-credentials.png)

1. 单击 **运行测试** 按钮以生成电子邮件预览。

1. 在常用的桌面、移动和基于Web的客户端中查看您的电子邮件内容。

   ![](assets/simulate-rendering-previews.png)

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
