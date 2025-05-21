---
audience: end-user
title: 设计推送通知投放
description: 了解如何使用Adobe Campaign Web设计推送通知投放
exl-id: 031bc38a-2435-4468-8ee6-3bcf1132da55
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 39%

---


# 设计推送投放 {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="推送 Android 内容"
>abstract="定义您用于 Android 设备的推送通知的内容。要开始编写消息，请单击&#x200B;**编辑内容**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="推送 iOS 内容"
>abstract="定义您用于 iOS 设备的推送通知的内容。要开始编写消息，请单击&#x200B;**编辑内容**&#x200B;按钮。"

## 定义通知的内容 {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="推送 iOS 消息"
>abstract="定义您用于 iOS 设备的推送通知的内容。要编写消息，请单击&#x200B;**标题**&#x200B;和&#x200B;**消息**&#x200B;字段。使用表达式编辑器使数据个性化并添加动态内容。有关更多自定义配置，请浏览到&#x200B;**高级设置**&#x200B;部分。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_msg"
>title="推送 Android 消息"
>abstract="定义您用于 Android 设备的推送通知的内容。要编写消息，请单击&#x200B;**标题**&#x200B;和&#x200B;**消息**&#x200B;字段。使用表达式编辑器使数据个性化并添加动态内容。要进一步使推送通知个性化，可选择要添加到推送通知的图像、要在您的轮廓的设备上显示的通知图标及其颜色。有关更多自定义配置，请浏览到&#x200B;**高级设置**&#x200B;部分。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="iOS 的静默通知"
>abstract="通过静默推送模式，可将“静默”通知发送到移动设备应用程序。其中并不通知用户已送达通知。而是直接将通知传送到应用程序。"

创建推送投放后，请定义其内容。 参数和设置取决于移动设备操作系统：Android或iOS。 浏览以下选项卡，了解如何为每个操作系统编写消息。

>[!BEGINTABS]

>[!TAB Android]

使用Firebase Cloud Messaging时，请选择两种类型的消息：

* **[!UICONTROL 数据消息]**&#x200B;由客户端应用程序处理。 这些消息将直接发送到移动设备应用程序，后者在设备上生成并显示Android通知。 数据消息仅包含您的自定义应用程序变量。

  要定义内容、个性化数据并添加动态内容，请单击&#x200B;**[!UICONTROL 消息]**&#x200B;字段并使用表达式编辑器。 访问此编辑器以自定义消息。
在&#x200B;**[!UICONTROL 应用程序变量]**&#x200B;菜单中，您的应用程序变量将自动添加。 这些变量允许您定义通知行为。 例如，配置在用户激活通知时显示的特定应用程序屏幕。

  ![描述：在Android通知中为数据消息定义内容的示例](assets/push_content_4.png){zoomable="yes"}

* **[!UICONTROL 通知消息]**，由FCM SDK自动处理。 FCM会代表客户端应用程序在用户设备上自动显示消息。 通知消息包含预定义的一组参数和选项，但仍可以使用自定义应用程序变量进一步个性化。

  要编写消息，请单击&#x200B;**[!UICONTROL 标题]**&#x200B;和&#x200B;**[!UICONTROL 消息]**&#x200B;字段。使用表达式编辑器定义内容、个性化数据和添加动态内容。

  要进一步个性化推送通知，请选择要添加到推送通知的图像、要在用户档案设备上显示的通知图标及其颜色。

  ![描述：在Android通知中为通知消息定义内容的示例](assets/push_content_3.png){zoomable="yes"}

>[!TAB iOS]

要编写消息，请单击&#x200B;**[!UICONTROL 标题]**&#x200B;和&#x200B;**[!UICONTROL 消息]**&#x200B;字段。使用表达式编辑器定义内容、个性化数据和添加动态内容。

您可以添加&#x200B;**[!UICONTROL Subtitle]**，它是iOS通知有效负载的subtitle参数的值。 请参阅此章节。

通过静默推送模式，可将“静默”通知发送到移动设备应用程序。其中并不通知用户已送达通知。而是直接将通知传送到应用程序。

![描述：定义iOS通知内容的示例](assets/push_content_1.png){zoomable="yes"}

>[!ENDTABS]

## 推送通知高级设置 {#push-advanced}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings"
>title="推送通知的高级设置"
>abstract="定义推送通知的高级设置，例如其优先级、关联的通知计数、应用程序变量等。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_critical"
>title="重要警报模式"
>abstract="启用此选项以将声音添加到您的通知，即使将用户的手机设置为专注模式或将设备设为静音也是如此。这样确保用户在任何情况下均可收到重要警告的通知。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_count"
>title="通知次数"
>abstract="使用此选项设置要直接显示在应用程序图标上的未读通知数。这样用户即可迅速了解待处理通知的数量。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="可变内容"
>abstract="使用此选项使移动设备应用程序可下载与通知关联的媒体内容。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_score"
>title="相关性分数"
>abstract="设置 0 至 100 的相关性分数以划分通知在通知摘要中的顺序。分数越高，通知就越重要。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_app_variables"
>title="应用程序变量"
>abstract="使用应用程序变量定义通知行为。可完全自定义这些变量，并将其纳入发送到移动设备的消息负载。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_category"
>title="类别 ID"
>abstract="指定与通知关联的类别 ID 的名称。这样可显示操作按钮，使用户不必打开应用程序，即可直接从通知中执行各种任务。"

高级选项取决于移动设备操作系统：Android或iOS。 浏览以下选项卡，了解如何为每个操作系统定义消息的选项。

>[!BEGINTABS]

>[!TAB Android]

![描述： Android通知的高级设置示例](assets/push_content_5.png){zoomable="yes"}

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 声音]** | 设置设备收到通知时播放的声音。 |
| **[!UICONTROL 通知计数]** | 设置直接在应用程序图标上显示的新未读信息数。 这样用户即可迅速了解待处理通知的数量。 |
| **[!UICONTROL 渠道ID]** | 设置通知的渠道ID。 在收到任何具有此渠道ID的通知之前，应用程序必须创建具有此渠道ID的渠道。 |
| **[!UICONTROL 单击操作]** | 定义与用户单击您的通知关联的操作。 这会确定用户与通知交互时的行为，例如打开特定屏幕或在应用程序中执行特定操作。 |
| **[!UICONTROL 标记]** | 设置用于替换通知抽屉中现有通知的标识符。 这有助于防止累积多个通知，并确保只显示最新的相关通知。 |
| **[!UICONTROL 优先级]** | 设置通知的优先级，可以是默认、最小、低或高。 优先级决定了通知的重要性和紧迫性，会影响通知的显示方式以及它是否可以绕过某些系统设置。 有关详细信息，请参阅[FCM文档](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority)。 |
| **[!UICONTROL 可见性]** | 设置通知的可见性级别，可以是公共、私有或机密。 可见性级别确定通知内容在锁屏界面和其他敏感区域上显示的程度。 有关详细信息，请参阅[FCM文档](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility)。 |
| **[!UICONTROL 粘性]** | 激活后，通知仍保持可见，即使用户单击它也是如此。 <br>如果停用，则当用户与通知交互时，该通知将自动取消。 粘性行为允许重要通知在屏幕上保留较长时间。 |
| **[!UICONTROL 应用程序变量]** | 允许您定义通知行为。 可完全自定义这些变量，并将其纳入发送到移动设备的消息负载。 |

>[!TAB iOS]

![描述： iOS通知的高级设置示例](assets/push_content_2.png){zoomable="yes"}

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 严重警报模式]** | 启用此选项以将声音添加到您的通知，即使将用户的手机设置为专注模式或将设备设为静音也是如此。这可确保用户注意到重要警报。 选中后，可以使用音量级别栏调整通知的音量。 条形图上方的0到100之间的数字反映了您的设置。 |
| **[!UICONTROL 清理徽章]** | 启用此选项以刷新应用程序图标上显示的标记值。 它确保徽章准确地反映新的未读信息的数量。 |
| **[!UICONTROL 通知计数]** | 设置一个将直接显示在应用程序图标上的数字，指示新的未读信息数量。 为用户提供了快速的可视化参考。 |
| **[!UICONTROL 卷]** | 声音的音量从0到100。 |
| **[!UICONTROL 可变内容]** | 启用此选项可允许移动应用程序下载与通知关联的媒体内容。 有关更多信息，请参阅 [Apple 开发人员文档](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)。 |
| **[!UICONTROL 相关性得分]** | 设置 0 至 100 的相关性分数以划分通知在通知摘要中的顺序。分数越高，通知就越重要。 |
| **[!UICONTROL 中断级别]** | <ul> <li>**[!UICONTROL 活动]**：默认设置，系统立即显示通知，打开屏幕并播放声音。 通知不会突破焦点模式。</li><li>**[!UICONTROL 被动]**：系统将通知添加到通知列表，而不打开屏幕或播放声音。 通知不会突破焦点模式。</li><li>**[!UICONTROL 时效性]**：系统立即显示通知，打开屏幕，可以播放声音，并突破焦点模式。 此级别不需要Apple的特殊权限。</li> <li>**[!UICONTROL 关键]**：系统立即显示通知，在屏幕上亮起，并绕过静音开关或聚焦模式。 请注意，此级别需要Apple的特殊权限。</ul> |
| **[!UICONTROL 线程ID]** | 用于将相关通知分组在一起的标识符。 具有相同线程ID的通知在通知列表中被组织为单个对话或线程。 |
| **[!UICONTROL 类别]** | 指定与通知关联的类别 ID 的名称。这样可显示操作按钮，使用户不必打开应用程序，即可直接从通知中执行各种任务。 |
| **[!UICONTROL 目标内容ID]** | 用于在打开通知时定位要前转的应用程序窗口的标识符。 |
| **[!UICONTROL 启动图像]** | 指定用户选择从通知中启动应用程序时要显示的启动图像文件的名称。 将显示选定的图像，而不是应用程序常规启动屏幕。 |
| **[!UICONTROL 应用程序变量]** | 允许您定义通知行为。 可完全自定义这些变量，并将其纳入发送到移动设备的消息负载。 |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->
