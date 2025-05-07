---
title: 连接到 Adobe Campaign Web 界面
description: 了解如何连接到 Adobe Campaign Web 用户界面
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
source-git-commit: 497335e6f176d33c4e9cd214abf46665ad75e1eb
workflow-type: ht
source-wordcount: '919'
ht-degree: 100%

---

# 连接到 Adobe Campaign {#connect-to-campaign}

Experience Cloud 是 Adobe 的数字营销应用程序、产品和服务的集成系列。通过其直观的界面，您可以快速访问云应用程序、产品功能和服务。了解如何连接到 Adobe Experience Cloud 并在此页面中访问 Adobe Campaign Web 界面。

## 登录到 Adobe Experience Cloud {#sign-in-to-exc}

仅可使用单点登录 (SSO) 连接到 Campaign。通常，Experience Cloud 管理员会授予对应用程序和服务的访问权限。按照邀请您加入 Experience Cloud 的电子邮件中的步骤操作。

要登录到 Adobe Experience Cloud，请遵循这些基本步骤：

1. 浏览到 [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。

1. 使用您的 Adobe ID 或 Enterprise ID 登录。请参阅[此文章](https://helpx.adobe.com/cn/enterprise/using/identity.html){target="_blank"}以了解有关 Adobe 身份标识类型的更多信息。

   登录到 Experience Cloud 后，您可以快速访问所有解决方案和应用程序。

   ![显示 Adobe Experience Cloud 主页的屏幕快照](assets/exc-home.png){zoomable="yes"}

1. 确认您当前所在的是正确的组织。

   ![显示 Adobe Experience Cloud 中的组织选择的屏幕快照](assets/exc-orgs.png){zoomable="yes"}{width="50%" align="left"}

   请参阅[此文章](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=zh-hans){target="_blank"}以了解有关 Adobe Experience Cloud 中的组织的更多信息。

## 访问 Adobe Campaign {#access-to-campaign}

要访问您的 Campaign 环境，请从 Adobe Experience Cloud 主页的&#x200B;**快速访问**&#x200B;部分选择 **Campaign**。

如果您已连接到另一个 Adobe Experience Cloud 解决方案，请从屏幕右上角的解决方案切换器浏览到您的 Campaign 环境。

![显示 Adobe Experience Cloud 中的解决方案切换器的屏幕快照](assets/solution-switcher.png){zoomable="yes"}

如果您有权访问多个环境（包括 Campaign 控制面板），请点击正确实例对应的&#x200B;**启动**&#x200B;按钮。

![显示 Adobe Campaign 启动按钮的屏幕快照](assets/launch-campaign.png){zoomable="yes"}

您现已连接到 Campaign。在[此页面](user-interface.md)中了解如何开始使用用户界面。

### 访问控制 {#access-control}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建此对象。"

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="此受众为只读"
>abstract="您无权编辑此受众。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="此服务为只读"
>abstract="您无权编辑此服务。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="收件人只读轮廓"
>abstract="您无权编辑此轮廓。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="此活动为只读"
>abstract="您无权编辑此活动。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="此投放为只读"
>abstract="您无权编辑此投放。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="此工作流为只读"
>abstract="您无权编辑此工作流。如果需要，请联系您的管理员以向您授予访问权限。"

访问控制会限制从主列表（如投放、收件人或工作流）中访问对象和数据的权限。这些限制在资源管理器导航树中也适用。此外，您需要权限才能从用户界面创建、删除、重复和编辑对象。

Campaign Web 中的所有权限都与 Campaign 客户端控制台权限同步。仅 Campaign 管理员能够定义和修改用户权限。

在浏览 Campaign Web 用户界面时，可以根据您的权限访问数据、对象和功能。例如，如果您无权访问某个文件夹，则您看不到它。您的权限还影响对象和数据管理。没有特定文件夹的写入权限，即无法在该文件夹中创建某个投放，即使您可在用户界面中看到它也是如此。

您可以在此处了解如何 [查看和管理权限](permissions.md)。

## Adobe Experience Cloud 顶部导航 {#top-bar}

浏览界面的顶部栏可：

* 分享有关 Campaign Web 用户界面的反馈。
* 在组织之间切换。
* 在 Adobe Experience Cloud 解决方案和应用程序之间切换。
* 搜索关于 [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=zh-hans){target="_blank"} 的帮助。
* 检查您的产品通知。
* 编辑您的 Adobe 轮廓和管理设置，如[更新您的常用语言](#language-pref)或[切换到浅色/深色主题](#dark-theme)。

![显示 Adobe Experience Cloud 顶部导航栏的屏幕快照](assets/do-not-localize/unified-shell.png){zoomable="yes"}{width="50%" align="left"}

## 支持的浏览器 {#browsers}

Adobe Campaign Web 所采用的设计使其能够在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中以最佳状态运行。在旧版本或其他浏览器中使用某些功能时，您可能会遇到问题。

## 语言偏好设置 {#language-pref}

Adobe Campaign Web 目前提供以下语言版本：

* 英语（美国）- EN-US
* 法语 - FR
* 德语 - DE
* 意大利语 - IT
* 西班牙语 - ES
* 葡萄牙语（巴西）- PTBR
* 日语 - JP
* 朝鲜语 - KR
* 简体中文 - CHS
* 繁体中文 - CHT

此外，受用户界面支持的各种语言变体也可能提供特定于区域设置的格式化（例如日期、时间、日历、数字）：

* 英语（以色列）
* 英语（英国）
* 西班牙语（墨西哥）
* 西班牙语（拉丁美洲）
* 法语（加拿大）

在您的用户轮廓中指定的首选语言决定您的 Campaign Web 默认语言。它与 Campaign 服务器和客户端控制台的语言无关。

要更改您的语言，请执行以下操作：

1. 单击右上角的个人档案图标，然后选择&#x200B;**偏好设置**。
1. 点击电子邮件地址下方显示的语言链接。
1. 选择您的首选语言并单击&#x200B;**保存**。如果您使用的组件未本地化为您的首选语言，可以选择第二语言。


## 深色和浅色主题 {#dark-theme}

Adobe Campaign 有浅色和深色主题可用。默认情况下，以浅色主题启用用户界面。要切换到深色主题，请单击您的轮廓图标，然后使用&#x200B;**深色主题**&#x200B;切换开关启用或禁用它。

有关用户轮廓设置和帐户偏好设置的详情，请参阅[本节内容](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=zh-hans#preferences){target="_blank"}。

请参阅[此文档](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=zh-hans){target="_blank"}以了解有关 Experience Cloud 中央界面组件的更多信息。