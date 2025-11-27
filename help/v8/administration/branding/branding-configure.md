---
title: 品牌化
description: 了解如何配置您的品牌
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 29%

---

# 配置品牌 {#branding-configure}

>[!IMPORTANT]
>
>最终用户不能创建或修改品牌：必须由 Adobe Campaign 技术管理员执行这些操作。如有任何需求，请与 Adobe 客户关怀部门联系。

在Adobe Campaign V8中，可以在&#x200B;**[!UICONTROL 管理>平台>品牌]**&#x200B;菜单中找到品牌。

**[!UICONTROL 品牌]**&#x200B;由以下特征定义：

* 用于定义和个性化品牌的&#x200B;**[!UICONTROL 标识]**。此部分包含以下字段：

   * 显示在界面中的 **[!UICONTROL Label]**
   * **[!UICONTROL ID]**
   * **[!UICONTROL Brand name]**
   * 品牌的 **[!UICONTROL Website URL]** 和 **[!UICONTROL Website label]**
   * **[!UICONTROL Brand logo]**

  ![](assets/branding_1.png)

* **[!UICONTROL 已发送电子邮件的标题参数]**，可个性化营销策划的收件人将看到的内容。 此部分包含以下字段：

   * 使用品牌电子邮件地址的 **[!UICONTROL Sender (email address)]**。
   * 使用品牌名称的 **[!UICONTROL Sender (name)]**。
   * 带有客户回信用电子邮件地址的 **[!UICONTROL Reply to (email address)]**。
   * 带有品牌名称的 **[!UICONTROL Reply to (name)]**。
   * 带有出错回复用电子邮件地址的 **[!UICONTROL Error (email address)]**。

  >[!IMPORTANT]
  >
  >更新了电子邮件的标题参数后，如果从模板创建的电子邮件中发件人的名称和电子邮件地址没有变化，请检查模板的高级设置。

  ![](assets/branding_2.png)

* **[!UICONTROL 品牌配置]**&#x200B;定义了用于跟踪以及用于登陆页面访问的服务器。 此部分包含以下字段：

   * **[!UICONTROL Brand子域]**&#x200B;是指向Adobe请求委派的特定于该品牌的指定子域URL。

  请注意，跟踪、镜像和应用程序服务器的配置存储在与路由关联的单独外部帐户中。 这些设置将在配置期间应用，且不得修改。 要显示URL，请从外部帐户访问&#x200B;**[!UICONTROL 品牌前缀]**&#x200B;选项卡。

  ![](assets/branding_3.png)

* 通过&#x200B;**[!UICONTROL 跟踪URL配置]**&#x200B;菜单，您可以通过定义用于与Adobe Analytics和Google Analytics等Web分析工具集成的其他参数来增强URL跟踪。

  使用&#x200B;**[!UICONTROL 其他URL参数]**&#x200B;菜单创建其他参数作为键值对及其适用条件。 每个参数名称都必须唯一且非空，并且每个参数值都必须非空。 适用性条件可以为空，但所有这些值都不能包含JST标记。

  这些参数将应用于与&#x200B;**[!UICONTROL 域名列表]**&#x200B;中指定的任何域名匹配的跟踪URL，这些URL可以包括正则表达式。

  **示例：**&#x200B;如果为该域配置了其他参数`https://www.example.com`和`https://www.example.com/?age=21&deliveryName=DM101`，则诸如`age=21`之类的跟踪URL将变为`deliveryName=DM101`。

## 为事务性消息配置品牌策略 {#branding-transactional-config}

>[!IMPORTANT]
>
>本节仅适用于事务型消息传递（消息中心）。
>
>虽然事务型功能在Campaign Web UI中可用，但必须在Campaign v8客户端控制台（控制实例）中执行以下步骤。

如果您将事务型消息传递（消息中心）与品牌策略结合使用，则需要额外配置。

### 实时实例的跟踪公式

在实时(RT)控制实例上激活品牌策略时，会使用特定的跟踪选项来管理跟踪公式。 这些公式在RT Control实例上集中配置，而不是在每个RT Execution实例上单独配置。

以下选项定义RT投放使用的跟踪公式：

* **`NmsTracking_RT_ClickFormula`**：指定用于对RT实例进行点击跟踪的公式

* **`NmsTracking_RT_OpenFormula`**：指定用于在RT实例上打开跟踪的公式

如果您的实施需要事务型消息的自定义跟踪公式，请使用以下选项：

* **`Branding_RT_ListXtkOptions_toPublish`**：在此处列出自定义公式的XTK选项名称（用逗号分隔）。 这可确保RT投放可以应用自定义跟踪公式。