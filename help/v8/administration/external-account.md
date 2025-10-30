---
title: 管理外部帐户
description: 了解如何配置外部帐户
exl-id: 24e70106-3312-4138-bf2d-ffad74e2962d
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 2%

---

# Campaign特定的外部帐户 {#external-account}

按照以下步骤操作，根据您选择的外部帐户类型配置帐户设置。

## 退回电子邮件 (POP3) {#bounce}

退回邮件外部帐户指定用于连接到电子邮件服务的外部POP3帐户。 所有配置为POP3访问的服务器都可以接收回邮。

![显示退回邮件(POP3)外部帐户配置字段的屏幕截图。](assets/external_account_bounce.png)

要配置&#x200B;**[!UICONTROL 退回邮件(POP3)]**&#x200B;外部帐户，请填写以下字段：

* **[!UICONTROL 服务器]** - POP3服务器的URL。

* **[!UICONTROL 端口]** - POP3连接端口号（默认端口为110）。

* **[!UICONTROL 帐户]** — 用户的名称。

* **[!UICONTROL 密码]** — 用户帐户密码。

* **[!UICONTROL 加密]** — 选择的加密类型，包括：
   * 默认情况下（如果端口110，则为POP3；如果端口995，则为POP3）。
   * 发送STARTTLS后切换到SSL的POP3。
   * POP3不安全（默认使用端口110）。
   * POP3在SSL上安全（默认使用端口995）。

* **[!UICONTROL 功能]** — 选择&#x200B;**[!UICONTROL 入站电子邮件]**&#x200B;配置接收入站电子邮件的帐户或选择&#x200B;**[!UICONTROL SOAP路由器]**&#x200B;处理SOAP请求。

>[!IMPORTANT]
>
>在使用Microsoft OAuth 2.0配置POP3外部帐户之前，您首先需要在Azure门户中注册应用程序。 有关详细信息，请参见[此页面](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}。

要使用Microsoft OAuth 2.0配置POP3外部连接，请选中Microsoft OAuth 2.0选项并填写以下字段：

* **[!UICONTROL Azure租户]**

  Azure ID(或目录（租户） ID)可以在Azure门户的应用程序概述的Essentials下拉菜单中找到。

* **[!UICONTROL Azure客户端ID]**

  可以在Azure门户中应用程序概述的Essentials下拉菜单中找到客户端ID(或应用程序（客户端）ID)。

* **[!UICONTROL Azure客户端密钥]**

  可以在Azure门户中应用程序的证书和密码菜单的“客户端密码”列中找到客户端密码ID。

* **[!UICONTROL Azure重定向URL]**

  可在Azure门户中应用程序的身份验证菜单中找到重定向URL。 它应以下列语法nl/jsp/oauth.jsp结尾，如`https://redirect.adobe.net/nl/jsp/oauth.jsp`。

安装和使用客户端控制台中的“测试连接”按钮需要Internet访问。 设置完成后，inMail进程可以与Microsoft服务器通信，而无需互联网。

输入不同的凭据后，可以单击“设置”连接以完成外部帐户配置。

## 路由 {#routing}

要为外部投放配置特定的外部帐户，请执行以下步骤。

1. 创建外部帐户。 [了解详情](create-external-account.md)

1. 选择&#x200B;**[!UICONTROL 路由]**&#x200B;类型。

   ![显示路由外部帐户类型选择的屏幕截图。](assets/external-account-routing.png){zoomable="yes"}

1. 选择所需的渠道并单击&#x200B;**[!UICONTROL 创建]**。

1. 在外部帐户&#x200B;**[!UICONTROL 详细信息]**&#x200B;部分中，**[!UICONTROL 外部]**&#x200B;默认被选为&#x200B;**[!UICONTROL 传递模式]**。

   ![显示路由外部帐户的传递模式配置的屏幕截图。](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >当前，**[!UICONTROL External]**&#x200B;是唯一可用的模式。

1. 要在投放执行后处理该流程，请将其外部化到后处理工作流。 创建具有[外部信号](../workflows/activities/external-signal.md)活动的工作流，并从&#x200B;**[!UICONTROL 后处理]**&#x200B;字段中选择它。

   ![显示路由外部帐户后处理字段配置的屏幕截图。](assets/external-account-post-processing.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 活动]**&#x200B;字段中，编辑日志中显示的后处理工作流活动的名称。<!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## 执行实例 {#instance-exec}

如果您具有分段体系结构，请确定与控制实例相关联的执行实例，并在它们之间建立连接。 事务性消息模板部署在执行实例上。

![显示执行实例外部帐户配置字段的屏幕截图。](assets/external_account_exec.png)

要配置&#x200B;**[!UICONTROL 执行实例]**&#x200B;外部帐户：

* **[!UICONTROL URL]** — 安装执行实例的服务器的URL。

* **[!UICONTROL 帐户]** — 帐户的名称，与operator文件夹中定义的消息中心代理匹配。

* **[!UICONTROL 密码]** — 操作员文件夹中定义的帐户密码。

* **[!UICONTROL 方法]** — 在Web服务或联合数据访问(FDA)之间进行选择。

  对于FDA，选择您的FDA帐户。 请注意，与外部系统的Campaign连接仅限于高级用户，并且只能从客户端控制台中使用。 [了解详情](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL 创建存档工作流]** — 对于在消息中心中注册的每个执行实例，无论您拥有一个还是多个实例，请为与该执行实例关联的每个外部帐户创建单独的存档工作流。
