---
title: 管理外部帐户
description: 了解如何配置外部帐户
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# 管理外部帐户 {#external-accounts}

>[!AVAILABILITY]
>
>* 外部帐户当前仅适用于退回邮件(POP3)、路由和执行实例。 稍后将添加其他帐户类型。
>
>* 在Adobe Campaign控制台中创建的不受支持的外部帐户在Web用户界面中可见，但无法编辑或访问。

Adobe Campaign包括预配置的外部帐户，可轻松与各种系统集成。 要连接到其他平台或自定义连接以适合您的工作流，请使用Web用户界面创建新的外部帐户。 这可确保无缝的数据传输。

## 创建外部帐户 {#create-ext-account}

要创建新的外部帐户，请执行以下步骤。 详细设置取决于外部帐户的类型。 [了解详情](#campaign-specific)

1. 从左窗格菜单中选择&#x200B;**[!UICONTROL 管理]**&#x200B;下的&#x200B;**[!UICONTROL 外部帐户]**。

1. 单击&#x200B;**[!UICONTROL 创建外部帐户]**。

   ![屏幕截图显示了在Web用户界面中创建外部帐户的选项。](assets/external_account_create_1.png)

1. 输入您的&#x200B;**[!UICONTROL 标签]**&#x200B;并选择外部帐户&#x200B;**[!UICONTROL 类型]**。

   >[!NOTE]
   >
   >[此部分](#campaign-specific)中详细介绍了Campaign特定类型的设置。

   ![显示用于输入标签和选择外部帐户类型的字段的屏幕截图。](assets/external_account_create_2.png)

1. 单击&#x200B;**[!UICONTROL 创建]**。

1. 从&#x200B;**[!UICONTROL 其他选项]**&#x200B;下拉列表中，根据需要更改&#x200B;**[!UICONTROL 内部名称]**&#x200B;或&#x200B;**[!UICONTROL 文件夹]**&#x200B;路径。

   ![显示内部名称和文件夹路径配置的其他选项的屏幕截图。](assets/external_account_create_3.png)

1. 启用&#x200B;**[!UICONTROL 自动导出包]**&#x200B;选项，以自动导出由此外部帐户管理的数据。<!--Exported where??-->

   ![显示包中启用自动导出选项的屏幕截图。](assets/external_account_create_exported.png)

1. 在&#x200B;**[!UICONTROL 详细信息]**&#x200B;部分中，通过基于所选外部帐户类型指定凭据来配置对帐户的访问权限。 [了解详情](#bounce)

1. 单击&#x200B;**[!UICONTROL 测试连接]**&#x200B;以验证配置是否正确。

1. 从&#x200B;**[!UICONTROL 更多……]**&#x200B;菜单，复制或删除您的外部帐户。

   ![屏幕截图显示“更多”菜单，其中包含复制或删除外部帐户的选项。](assets/external_account_create_4.png)

1. 配置完成后，单击&#x200B;**[!UICONTROL 保存]**。

## Campaign特定的外部帐户 {#campaign-specific}

根据您选择的外部帐户类型，执行以下步骤以配置帐户设置。

### 退回电子邮件 (POP3) {#bounce}

>[!AVAILABILITY]
>
> 当前不支持OAuth 2.0。

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

### 路由 {#routing}

要为外部投放配置特定的外部帐户，请执行以下步骤。

1. 创建外部帐户。 [了解详情](../administration/external-account.md#create-ext-account)

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

### 执行实例 {#instance-exec}

如果您具有分段体系结构，请确定与控制实例相关联的执行实例，并在它们之间建立连接。 事务性消息模板部署在执行实例上。

![显示执行实例外部帐户配置字段的屏幕截图。](assets/external_account_exec.png)

要配置&#x200B;**[!UICONTROL 执行实例]**&#x200B;外部帐户：

* **[!UICONTROL URL]** — 安装执行实例的服务器的URL。

* **[!UICONTROL 帐户]** — 帐户的名称，与operator文件夹中定义的消息中心代理匹配。

* **[!UICONTROL 密码]** — 操作员文件夹中定义的帐户密码。

* **[!UICONTROL 方法]** — 在Web服务或联合数据访问(FDA)之间进行选择。

  对于FDA，选择您的FDA帐户。 请注意，与外部系统的Campaign连接仅限于高级用户，并且只能从客户端控制台中使用。 [了解详情](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL 创建存档工作流]** — 对于在消息中心中注册的每个执行实例，无论您拥有一个还是多个实例，请为与该执行实例关联的每个外部帐户创建单独的存档工作流。