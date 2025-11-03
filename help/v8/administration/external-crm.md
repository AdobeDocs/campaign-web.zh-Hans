---
title: 管理外部帐户
description: 了解如何配置CRM外部帐户
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# CRM外部帐户 {#external-crm}

使用外部CRM类型帐户将Adobe Campaign与第三方数据库连接。

此外部帐户的配置设置取决于您所连接的特定数据库引擎。 以下各节提供了每个受支持数据库的详细设置说明。

## Microsoft Dynamics CRM

Microsoft Dynamics CRM外部帐户允许您将Campaign实例连接到Microsoft Dynamics CRM外部数据库。

在Adobe Campaign Web用户界面中，配置您的Microsoft Dynamics CRM外部帐户。

1. [创建外部帐户](external-account.md)并选择&#x200B;**[!UICONTROL 外部数据库]**&#x200B;作为外部帐户的&#x200B;**[!UICONTROL 类型]**，选择Microsoft Dynamics CRM作为&#x200B;**[!UICONTROL 提供程序类型]**。

1. 单击&#x200B;**[!UICONTROL 创建]**。

1. 要配置&#x200B;**[!UICONTROL Microsoft Dynamics CRM]**&#x200B;外部帐户，请填写以下字段：

   ![显示Microsoft Dynamics CRM外部帐户配置字段的屏幕截图。](assets/crm-microsoft-1.png)

   +++ 对于CRM OAuth，类型：密码凭据

   * **[!UICONTROL 服务器]**：输入Microsoft CRM服务器的URL。

     要找到Microsoft CRM服务器URL，请登录到您的Microsoft Dynamics CRM帐户，选择Dynamics 365，然后打开您的应用程序。 服务器URL显示在浏览器的地址栏中，例如： `https://myserver.crm.dynamics.com/`。

   * **[!UICONTROL 帐户]**：指定用于登录到Microsoft CRM的帐户。

   * **[!UICONTROL 密码]**：输入与指定帐户关联的密码。

   * **[!UICONTROL 客户端标识符]**：输入在Microsoft Azure管理门户中找到的客户端ID。

   * **[!UICONTROL CRM版本]**：选择Dynamics CRM 365 CRM版本。

   +++

   </br>

   +++ 对于CRM O-Auth类型：证书

   * **[!UICONTROL 服务器]**：输入Microsoft CRM服务器的URL。

     要找到Microsoft CRM服务器URL，请登录到您的Microsoft Dynamics CRM帐户，选择Dynamics 365，然后打开您的应用程序。 服务器URL显示在浏览器的地址栏中，例如： `https://myserver.crm.dynamics.com/`。

   * **[!UICONTROL 私钥（Base64编码）]**：提供以Base64格式编码的私钥。

     为此，您可以使用Base64编码器帮助或使用适用于Linux的命令行`base64 -w0 private.key`。

   * **[!UICONTROL 自定义密钥标识符]**：输入用于证书的自定义密钥标识符。

   * **[!UICONTROL 密钥ID]**：输入与证书关联的密钥ID。

   * **[!UICONTROL 客户端标识符]**：输入在Microsoft Azure管理中找到的客户端ID

   * **[!UICONTROL CRM版本]**：选择Dynamics CRM 365 CRM版本。

   +++

1. 设置连接后，访问&#x200B;**[!UICONTROL Microsoft CRM配置向导]**&#x200B;以生成Microsoft CRM表列表。

   单击&#x200B;**[!UICONTROL 下一步]**&#x200B;以选择所需的表。

   ![显示Microsoft Dynamics CRM外部帐户配置字段的屏幕截图。](assets/crm-microsoft-2.png)

1. 选择要检索的Microsoft CRM表，或通过指定&#x200B;**[!UICONTROL 表标签]**&#x200B;和&#x200B;**[!UICONTROL 表内部名称]**&#x200B;添加远程表，然后启用&#x200B;**[!UICONTROL 选定项]**&#x200B;切换开关。

   单击&#x200B;**[!UICONTROL 下一步]**。

1. 单击&#x200B;**[!UICONTROL 开始]**&#x200B;以开始基于所选表创建Microsoft CRM架构。

1. 按照屏幕上的说明，将来自Adobe Campaign营销历史和订阅管理的页面直接插入到Microsoft Dynamics CRM中。

1. 单击&#x200B;**[!UICONTROL 显示营销历史URL]**&#x200B;可查看用于集成营销历史页面的URL，或单击&#x200B;**[!UICONTROL 显示潜在客户订阅的URL]**&#x200B;可查看用于集成订阅管理页面的URL。

   ![显示Microsoft Dynamics CRM外部帐户配置字段的屏幕截图。](assets/crm-microsoft-3.png)

1. 配置Microsoft CRM外部帐户后，单击&#x200B;**[!UICONTROL 保存]**。

1. 创建外部帐户后，您现在可以单击&#x200B;**[!UICONTROL 同步枚举……]**&#x200B;以自动将枚举从Microsoft CRM同步到Adobe Campaign Web用户界面。

   ![显示Microsoft CRM CRM外部帐户配置字段的屏幕截图。](assets/crm-microsoft-4.png)

1. 选择与Microsoft CRM枚举匹配的Adobe Campaign枚举。

   要将Adobe Campaign值替换为Microsoft CRM值，请启用&#x200B;**[!UICONTROL 替换]**&#x200B;选项。

## Salesforce {#salesforce}

要配置Salesforce外部帐户以使其与Adobe Campaign配合使用，您需要提供以下详细信息：

1. [创建外部帐户](external-account.md)并选择&#x200B;**[!UICONTROL 外部数据库]**&#x200B;作为外部帐户的&#x200B;**[!UICONTROL 类型]**，Salesforce.com作为&#x200B;**[!UICONTROL 提供程序类型]**。

   ![显示Salesforce外部帐户配置字段的屏幕截图。](assets/crm-salesforce-1.png)

1. 单击&#x200B;**[!UICONTROL 创建]**。

1. 要配置&#x200B;**[!UICONTROL Salesforce]**&#x200B;外部帐户，请填写以下字段：

   * **[!UICONTROL CRM O-Auth类型]**： **[!UICONTROL 密码凭据]**&#x200B;或&#x200B;**[!UICONTROL 凭据]**

   * **[!UICONTROL 帐户]**：用于登录到Salesforce CRM的帐户。

   * **[!UICONTROL 密码]**：输入与指定帐户关联的密码。

   * **[!UICONTROL 安全令牌]**：输入与帐户关联的Salesforce安全令牌。

   * **[!UICONTROL API版本]**：选择版本49。

   ![显示Salesforce外部帐户配置字段的屏幕截图。](assets/crm-salesforce-2.png)

1. 打开&#x200B;**[!UICONTROL Salesforce CRM配置向导]**&#x200B;以生成Salesforce CRM表列表，然后单击&#x200B;**[!UICONTROL 下一步]**。

   ![显示Salesforce CRM外部帐户配置字段的屏幕截图。](assets/crm-salesforce-3.png)

1. 选择要检索的Salesforce表，或通过输入&#x200B;**[!UICONTROL 表标签]**&#x200B;和&#x200B;**[!UICONTROL 表内部名称]**&#x200B;添加远程表，然后启用&#x200B;**[!UICONTROL 选定项]**&#x200B;切换开关。

   单击&#x200B;**[!UICONTROL 下一步]**。

1. 单击&#x200B;**[!UICONTROL 开始]**&#x200B;以开始基于所选表创建Salesforce CRM架构。

1. 单击&#x200B;**[!UICONTROL Salesforce链接创建向导……]**&#x200B;以在Salesforce中生成Web链接。

   然后，单击&#x200B;**[!UICONTROL 下一步]**&#x200B;从Salesforce检索&#x200B;**潜在客户**&#x200B;和&#x200B;**联系人**&#x200B;的Web链接。

1. 选择要导出到Salesforce Web链接列表的链接。

1. 按照屏幕上的说明将Adobe Campaign Web用户界面中的&#x200B;**营销历史记录**&#x200B;和&#x200B;**订阅管理**&#x200B;页面插入到Salesforce CRM中。

1. 配置Salesforce CRM外部帐户后，单击&#x200B;**[!UICONTROL 保存]**。

1. 创建外部帐户后，您现在可以单击&#x200B;**[!UICONTROL 同步枚举……]**&#x200B;以自动将枚举从Salesforce同步到Adobe Campaign Web用户界面。

   ![显示Salesforce CRM外部帐户配置字段的屏幕截图。](assets/crm-salesforce-4.png)

1. 选择与Adobe Campaign枚举匹配的Salesforce枚举。

   要将Adobe Campaign值替换为Salesforce值，请启用&#x200B;**[!UICONTROL 替换]**&#x200B;选项。

   ![显示Salesforce CRM外部帐户配置字段的屏幕截图。](assets/crm-salesforce-5.png)

