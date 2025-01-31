---
title: 外部帐户
description: 了解如何配置外部帐户
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 15%

---

# 配置外部帐户 {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="外部帐户"
>abstract="您现在可以连接到其他平台或自定义连接以适合您的工作流程，并轻松创建新的外部帐户以满足您的特定需求并确保无缝数据传输。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"


>[!AVAILABILITY]
>
> 请注意，外部帐户当前仅适用于退回邮件(POP3)和执行实例，并且将来会添加其他帐户类型。
> 在Adobe Campaign控制台中创建的不受支持的外部帐户在Web用户界面中可见，但无法编辑或访问。

Adobe Campaign附带一组预配置的外部帐户，可轻松与各种系统集成。 如果您需要连接到其他平台或自定义连接以适合您的工作流程，您现在可以使用Web用户界面轻松创建新的外部帐户，以满足您的特定需求并确保无缝数据传输。

## 创建外部帐户 {#create-ext-account}

要创建新的外部帐户，请执行以下步骤。 详细设置取决于外部帐户的类型。

1. 从左窗格菜单中选择&#x200B;**[!UICONTROL 管理]**&#x200B;下的&#x200B;**[!UICONTROL 外部帐户]**。

1. 单击&#x200B;**[!UICONTROL 创建外部帐户]**。

   ![](assets/external_account_create_1.png)

1. 输入您的&#x200B;**[!UICONTROL 标签]**&#x200B;并选择您的外部帐户&#x200B;**[!UICONTROL 类型]**。

   ![](assets/external_account_create_2.png)

1. 单击&#x200B;**[!UICONTROL 创建]**。

1. 从&#x200B;**[!UICONTROL 高级选项]**&#x200B;下拉列表中，您可以根据需要更改&#x200B;**[!UICONTROL 内部名称]**&#x200B;或&#x200B;**[!UICONTROL 文件夹]**&#x200B;路径。

   ![](assets/external_account_create_3.png)

1. 如果希望自动导出由此外部帐户管理的数据，请启用&#x200B;**[!UICONTROL 自动导出]**。

1. 根据所选外部帐户类型指定凭据，以配置对帐户的访问权限。

1. 单击&#x200B;**[!UICONTROL 测试连接]**&#x200B;以检查配置是否正确

1. 从&#x200B;**[!UICONTROL 更多……]**&#x200B;菜单，复制或删除您的外部帐户。

   ![](assets/external_account_create_4.png)

1. 配置完成后，单击&#x200B;**[!UICONTROL 保存]**。

## Campaign特定的外部帐户 {#campaign-specific}

### 退回电子邮件 (POP3) {#bounce}

>[!AVAILABILITY]
>
> 当前不支持OAuth 2.0。

退回邮件外部帐户指定用于连接到电子邮件服务的外部POP3帐户。 所有配置为POP3访问的服务器都可以接收回邮。

![](assets/external_account_bounce.png)

要配置&#x200B;**[!UICONTROL 退回邮件(POP3)]**&#x200B;外部帐户：

* **[!UICONTROL 服务器]**

  POP3服务器的URL

* **[!UICONTROL 端口]**

  POP3连接端口号（默认端口为110）

* **[!UICONTROL 帐户]**

  用户的名称

* **[!UICONTROL 密码]**

  用户帐户密码

* **[!UICONTROL 加密]**

  选择的加密类型，介于：

   * 默认情况下（如果是端口 110，则为 POP3；如果是端口 995，则为 POP3S）
   * 发送 STARTTLS 后切换到 SSL 的 POP3
   * POP3 非安全端口（默认为端口 110）
   * SSL 上方的 POP3 安全端口（默认为端口 995）

* **[!UICONTROL 函数]**

  入站电子邮件（当外部帐户配置为接收传入电子邮件时）或SOAP路由器(用于处理SOAP请求)。

### 执行实例{#instance-exec}

如果您具有分段体系结构，则必须确定与控制实例关联的执行实例并在它们之间建立连接。 事务性消息模板部署在执行实例上。

![](assets/external_account_exec.png)

要配置&#x200B;**[!UICONTROL 执行实例]**&#x200B;外部帐户：

* **[!UICONTROL URL]**

  安装执行实例的服务器的URL。

* **[!UICONTROL 帐户]**

  帐户的名称，它必须与操作员文件夹中定义的消息中心代理匹配。

* **[!UICONTROL 密码]**

  运算符文件夹中定义的帐户密码。

* **[!UICONTROL 方法]**

  在Web服务或联合数据访问(FDA)之间进行选择。
对于FDA方法，请选择您的FDA帐户。 请注意，与外部系统的Campaign连接仅限于高级用户，并且只能从客户端控制台中使用。 [了解详情](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL 创建存档工作流]**

  对于在消息中心注册的每个执行实例，无论您拥有一个还是多个实例，都需要为与该执行实例关联的每个外部帐户创建单独的归档工作流。
