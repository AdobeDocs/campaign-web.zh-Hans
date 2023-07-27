---
audience: end-user
title: 设计推送通知投放
description: 了解如何使用Adobe Campaign Web设计推送通知投放
badge: label="Alpha"
source-git-commit: 1873e6105d9880295a3ace8f8be9ff7c02a3e683
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 5%

---

# 设计推送投放 {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="推送 Android 内容"
>abstract="定义推送 Android 内容。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="推送 iOS 内容"
>abstract="定义推送 iOS 内容。"

## 定义通知的内容 {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="推送iOS消息"
>abstract="定义推送iOS消息的标题和内容。 使用个性化对话框将内容个性化并添加条件。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="iOS的静默通知"
>abstract="静默推送模式允许将“静默”通知发送到移动应用程序。 用户不知道通知已到达。 它将直接传输到应用程序。"



>[!BEGINTABS]

>[!TAB Android]

使用Firebase Cloud Messaging，您可以选择两种类型的消息：

* 此 **[!UICONTROL 数据消息]** 由客户端应用程序处理。 这些消息直接发送到移动设备应用程序，后者在设备上生成并显示Android通知。 数据消息仅包含您的自定义应用程序变量。

  要定义内容、个性化数据并添加动态内容，请单击 **[!UICONTROL 消息]** 字段并使用表达式编辑器。 您可以访问此编辑器以自定义消息。
在 **[!UICONTROL 应用程序变量]** 菜单，则会自动添加应用程序变量。 这些变量允许您定义通知行为。 例如，您可以配置在用户激活通知时显示的特定应用程序屏幕。

  ![](assets/push_content_4.png)

* 此 **[!UICONTROL 通知消息]**，由FCM SDK自动处理。 FCM会代表客户端应用程序在用户设备上自动显示消息。 通知消息包含预定义的一组参数和选项，但仍可以使用自定义应用程序变量进一步个性化。

  要撰写消息，请单击 **[!UICONTROL 标题]** 和 **[!UICONTROL 正文]** 字段。 使用表达式编辑器定义内容、个性化数据和添加动态内容。

  要进一步个性化推送通知，您可以选择要添加到推送通知的图像，即要在用户档案设备上显示的通知图标及其颜色。

  ![](assets/push_content_3.png)

>[!TAB iOS]

要撰写消息，请单击 **[!UICONTROL 标题]** 和 **[!UICONTROL 正文]** 字段。 使用表达式编辑器定义内容、个性化数据和添加动态内容。

您可以添加 **[!UICONTROL 子标题]**，iOS通知有效负载的subtitle参数的值。 请参阅此部分。

静默推送模式允许将“静默”通知发送到移动应用程序。 用户不知道通知已到达。 它将直接传输到应用程序。

![](assets/push_content_1.png)

>[!ENDTABS]

## 推送通知高级设置 {#push-advanced}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_critical"
>title="iOS的严重警报模式"
>abstract="启用此选项可向通知添加声音，即使用户的手机设置为焦点模式或设备静音也是如此。 这可以确保在任何情况下都向用户通知重要警报。"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_count"
>title="iOS的徽章编号"
>abstract="使用此选项可设置直接显示在应用程序图标上的新未读信息数量。 这允许用户快速查看待处理通知的数量。"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="iOS的可变内容"
>abstract="使用此选项可允许移动应用程序下载与通知关联的媒体内容。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_score"
>title="iOS的相关性分数"
>abstract="将相关性得分从0设置为100，以优先处理通知摘要中的通知顺序。 分数越高，说明通知越重要。"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_app_variables"
>title="适用于iOS的应用程序变量"
>abstract="使用应用程序变量定义通知行为。 这些变量是完全可自定义的，并包含在发送到移动设备的消息有效负载中。"



>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 声音]** | 设置设备收到通知时播放的声音。 |
| **[!UICONTROL 通知次数]** | 设置直接在应用程序图标上显示的新未读信息数。 这允许用户快速查看待处理通知的数量。 |
| **[!UICONTROL 渠道 ID]** | 设置通知的渠道ID。 在收到任何具有此渠道ID的通知之前，应用程序必须创建具有此渠道ID的渠道。 |
| **[!UICONTROL 点击操作]** | 定义与用户单击您的通知关联的操作。 这会确定用户与通知交互时的行为，例如打开特定屏幕或在应用程序中执行特定操作。 |
| **[!UICONTROL 标记]** | 设置用于替换通知抽屉中现有通知的标识符。 这有助于防止累积多个通知，并确保只显示最新的相关通知。 |
| **[!UICONTROL 优先级]** | 设置通知的优先级，可以是默认、最小、低或高。 优先级决定了通知的重要性和紧迫性，会影响通知的显示方式以及它是否可以绕过某些系统设置。 有关详细信息，请参见 [FCM文档](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL 可见性]** | 设置通知的可见性级别，可以是公共、私有或机密。 可见性级别确定通知内容在锁屏界面和其他敏感区域上显示的程度。 欲了解更多信息，请参见 [FCM文档](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL 粘性]** | 激活后，通知仍保持可见，即使用户单击它也是如此。 <br>如果停用，则当用户与通知交互时，会自动取消通知。 粘性行为允许重要通知在屏幕上保留较长时间。 |
| **[!UICONTROL 应用程序变量]** | 允许您定义通知行为。 这些变量是完全可自定义的，并包含在发送到移动设备的消息有效负载中。 |

>[!TAB iOS]

![](assets/push_content_2.png)

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 严重警报模式]** | 启用此选项可向通知添加声音，即使用户的手机设置为焦点模式或设备静音也是如此。 这可确保用户注意到重要警报。 |
| **[!UICONTROL 清洁徽章]** | 启用此选项以刷新应用程序图标上显示的标记值。 它确保徽章准确地反映新的未读信息的数量。 |
| **[!UICONTROL 通知次数]** | 设置一个将直接显示在应用程序图标上的数字，指示新的未读信息数量。 为用户提供了快速的可视化参考。 |
| **[!UICONTROL 容量]** | 声音的音量从0到100。 |
| **[!UICONTROL 可变内容]** | 启用此选项可允许移动应用程序下载与通知关联的媒体内容。 有关更多信息，请参阅 [Apple 开发人员文档](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)。 |
| **[!UICONTROL 相关性分数]** | 将相关性得分从0设置为100，以优先处理通知摘要中的通知顺序。 分数越高，说明通知越重要。 |
| **[!UICONTROL 中断级别]** | <ul> <li>**[!UICONTROL 活动]**：默认情况下，系统会立即显示通知，打开屏幕并播放声音。 通知不会突破焦点模式。</li><li>**[!UICONTROL 被动]**：系统将通知添加到通知列表，而不打开屏幕或播放声音。 通知不会突破焦点模式。</li><li>**[!UICONTROL 时效性]**：系统立即显示通知，打开屏幕，可以播放声音并突破聚焦模式。 此级别不需要Apple的特殊权限。</li> <li>**[!UICONTROL 关键]**：系统立即显示通知，在屏幕上亮起，并绕过静音开关或聚焦模式。 请注意，此级别需要Apple的特殊权限。</ul> |
| **[!UICONTROL Thread-id]** | 用于将相关通知分组在一起的标识符。 具有相同线程ID的通知在通知列表中被组织为单个对话或线程。 |
| **[!UICONTROL 类别]** | 指定与通知关联的类别ID的名称。 这将启用操作按钮的显示，允许用户直接从通知执行各种任务，而无需打开应用程序。 |
| **[!UICONTROL 目标内容 ID]** | 用于在打开通知时定位要转发的应用程序窗口的标识符。 |
| **[!UICONTROL 启动图像]** | 指定用户选择从通知中启动应用程序时要显示的启动图像文件的名称。 将显示选定的图像，而不是应用程序常规启动屏幕。 |
| **[!UICONTROL 应用程序变量]** | 允许您定义通知行为。 这些变量是完全可自定义的，并包含在发送到移动设备的消息有效负载中。 |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



