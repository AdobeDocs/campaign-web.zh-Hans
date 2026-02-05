---
audience: end-user
title: 使用Adobe Experience Manager创建多语言电子邮件
description: 了解如何使用Campaign Web中的Adobe Experience Manager语言副本创建多语言电子邮件投放。
feature: Email
topic: Content Management
role: User
level: Intermediate
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 2%

---


# 使用Adobe Experience Manager创建多语言电子邮件 {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Manager实时和语言副本"
>abstract="您现在可以直接在Campaign中访问Adobe Experience Manager语言和活动副本。 实时内容刷新消除了手动同步以简化多语言工作流。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

通过Adobe Experience Manager集成，您可以使用Adobe Experience Manager语言副本创建多语言电子邮件投放。 这允许您管理不同语言的内容变体，并根据收件人语言偏好提供个性化电子邮件。

## 先决条件 {#prerequisites}

在创建多语言电子邮件投放之前，请确保您已：

* 访问为Adobe Campaign Web界面集成配置的Adobe Experience Manager实例。
* 已创建和批准带有语言副本的Adobe Experience Manager内容。 在[Adobe Experience Manager文档](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)中了解有关语言复制向导的更多信息
* 配置为接收Adobe Experience Manager内容的电子邮件投放模板。 请参阅[启用多语言模式](#enable-multilingual)部分中详述的步骤。

## 创建多语言投放

要创建多语言电子邮件投放，您首先需要在投放设置中启用多语言选项。 系统会自动检测可用的语言副本，并允许您选择要添加的语言副本。

### 启用多语言模式 {#enable-multilingual}

创建新投放并在高级设置中启用多语言选项。

1. 从&#x200B;**[!UICONTROL 投放]**&#x200B;菜单中，单击&#x200B;**[!UICONTROL 创建投放]**。

   ![](assets/lg-copy-1.png)

1. 选择包含AEM内容的&#x200B;**[!UICONTROL 电子邮件投放]**&#x200B;模板，然后单击&#x200B;**[!UICONTROL 创建投放]**。

   ![](assets/lg-copy-2.png)

1. 输入投放标签并配置受众。 [了解详情](../email/create-email.md)

1. 访问您的投放&#x200B;**[!UICONTROL 设置]**，然后导航到&#x200B;**[!UICONTROL 高级]**&#x200B;部分。

1. 启用&#x200B;**[!UICONTROL 启用AEM多语言]**&#x200B;选项。

   ![](assets/lg-copy-3.png)

1. 确保：

   * **[!UICONTROL 内容编辑模式]**&#x200B;设置为&#x200B;**[!UICONTROL AEM]**。
   * 选择了正确的Adobe Experience Manager **[!UICONTROL 外部帐户]**。

1. 单击&#x200B;**[!UICONTROL 保存并关闭]**。

### 创建内容变体 {#create-variants}

选择您的Adobe Experience Manager内容，然后选择要包含在投放中的语言变体。

1. 单击&#x200B;**[!UICONTROL 编辑内容]**。

1. 选择&#x200B;**[!UICONTROL 创建内容变体]**。

   ![](assets/lg-copy-4.png)

1. 从列表中选择您的Adobe Experience Manager内容。

   ![](assets/lg-copy-5.png)

1. 系统检测与选定内容（父子关系）关联的所有语言副本，例如，如果您的Adobe Experience Manager内容具有法语、德语和意大利语的变体，则所有变体都可供选择。

   选择要包含在投放中的语言变体。

   ![](assets/lg-copy-6.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

1. 在内容编辑器中查看您的语言变体。 您现在可以[单独管理每个变体](#manage-variants)或继续[发送投放](../monitor/prepare-send.md)。

   ![](assets/lg-copy-7.png)

## 管理语言变体 {#manage-variants}

创建内容变体后，您可以直接在投放中管理它们：

1. 要设置默认语言，请访问所选变体的高级菜单，然后选择&#x200B;**[!UICONTROL 设置为默认语言]**。 如果未设置用户档案的语言首选项或与任何可用变体不匹配，则使用默认语言。

   单击&#x200B;**[!UICONTROL 删除]**&#x200B;以从投放中删除任何变体。

   ![](assets/lg-copy-8.png)

1. 从“内容变体”高级菜单中，单击&#x200B;**[!UICONTROL 管理区域设置]**&#x200B;以将其他区域设置添加到您的投放中。

   ![](assets/lg-copy-9.png)

1. 选择其他语言副本以包含更多变体，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/lg-copy-11.png)

1. 如果在Adobe Experience Manager中更新了内容，请单击&#x200B;**[!UICONTROL 刷新AEM内容]**&#x200B;以将所有变体与最新版本同步。

   ![](assets/lg-copy-10.png)

1. 如果要直接在Campaign中编辑内容或断开与AEM的链接，请单击&#x200B;**[!UICONTROL 取消链接Adobe Experience Manager内容]**。

   >[!CAUTION]
   >
   >取消链接后，无法从Adobe Experience Manager刷新内容或创建新变体。 该内容将独立于Adobe Experience Manager。


