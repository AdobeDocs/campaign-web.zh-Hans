---
audience: end-user
title: 设计推送通知投放
description: 了解如何使用Adobe Campaign Web设计推送通知投放
badge: label="Alpha" type="Positive"
source-git-commit: fbedfc5d1886b86932c156574037549270480f44
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 13%

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

## 消息 {#push-message}

>[!BEGINTABS]

>[!TAB Android]

使用Firebase Cloud Messaging，您可以选择两种类型的消息：

* 此 **数据消息**，由客户端应用程序处理。 消息直接发送到移动应用程序，该应用程序将生成并向设备显示Android通知。 数据消息仅包含您的自定义应用程序变量。

   单击 **[!UICONTROL 消息]** 字段并使用表达式编辑器定义内容、个性化数据和添加动态内容。

* 通知消息，由FCM SDK自动处理。 FCM会代表客户端应用程序在用户的设备上自动显示消息。 通知消息包含预定义的一组参数和选项，但仍可以使用自定义应用程序变量进一步个性化。

   要撰写消息，请单击 **[!UICONTROL 标题]** 和 **[!UICONTROL 正文]** 字段。 使用表达式编辑器定义内容、个性化数据和添加动态内容。

   要进一步个性化推送通知，您可以选择要添加到推送通知的图像、要在用户档案的设备上显示的通知图标及其颜色。

>[!TAB iOS]

![](assets/push_content_1.png)

要撰写消息，请单击 **[!UICONTROL 标题]** 和 **[!UICONTROL 正文]** 字段。 使用表达式编辑器定义内容、个性化数据和添加动态内容。

您可以添加 **[!UICONTROL 字幕]**，iOS通知有效负载的字幕参数的值。 请参阅此章节。

静默推送模式允许将“静默”通知发送到移动应用程序。 用户未意识到通知的到达。 它将直接传输到应用程序。

>[!ENDTABS]

## 高级设置 {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 声音]** | 设置设备收到通知时播放的声音。 |
| **[!UICONTROL 通知次数]** | 设置直接在应用程序图标上显示的新未读信息数量。 |
| **[!UICONTROL 渠道 ID]** | 设置通知的渠道ID。 在收到任何使用此渠道ID的通知之前，应用程序必须使用此渠道ID创建一个渠道。 |
| **[!UICONTROL 点击操作]** | 设置与用户单击您的通知关联的操作。 |
| **[!UICONTROL 标记]** | 设置用于替换通知抽屉中现有通知的标识符。 |
| **[!UICONTROL 优先级]** | 将通知的优先级设置为“默认”、“最小”、“低”或“高”。 有关更多信息，请参阅FCM文档。 |
| **[!UICONTROL 可见性]** | 将通知的可见性级别设置为public、private或secret。 有关更多信息，请参阅FCM文档。 |
| **[!UICONTROL 粘性]** | 如果已停用，用户单击通知后会自动将其取消。 如果激活，则即使用户单击通知，该通知仍会显示。 |

>[!TAB iOS]

![](assets/push_content_2.png)

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 严重警报模式]** | 启用此选项，即使用户的手机设置为焦点模式或iPhone处于静音状态，也可以向通知中添加声音。 |
| **[!UICONTROL 清理徽章]** | 启用此选项以刷新标记值。 |
| **[!UICONTROL 通知次数]** | 设置一个数字，该数字将用于直接在应用程序图标上显示新未读信息的数量。 |
| **[!UICONTROL 容量]** | 音量从0到100。 |
| **[!UICONTROL 可变内容]** | 启用此选项可允许移动应用程序下载媒体内容。 有关更多信息，请参阅 [Apple 开发人员文档](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)。 |
| **[!UICONTROL 相关性分数]** | 将相关性得分从0设置为100。 系统使用此选项对通知摘要中的通知进行排序。 |
| **[!UICONTROL 中断级别]** | <ul> <li>**[!UICONTROL 活动]**：默认情况下，系统会立即显示通知，打开屏幕并播放声音。 通知不会突破焦点模式。</li><li>**[!UICONTROL 被动]**：系统会将通知添加到通知列表，而不会打开屏幕或播放声音。 通知不会突破焦点模式。</li><li>**[!UICONTROL 时效性]**：系统立即显示通知，打开屏幕，可以播放声音并突破聚焦模式。 此级别不需要Apple的特殊权限。</li> <li>**[!UICONTROL 关键]**：系统立即显示通知，在屏幕上亮起，并绕过静音开关或聚焦模式。 请注意，此级别需要Apple的特殊权限。</ul> |
| **[!UICONTROL Thread-id]** | 用于将相关通知分组在一起的标识符。 |
| **[!UICONTROL 类别]** | 将显示操作按钮的类别ID的名称。 这些通知为用户提供了一种更快的方式，无需在应用程序中打开或导航即可响应通知执行不同任务。 |
| **[!UICONTROL 目标内容 ID]** | 用于在打开通知时定向哪个应用程序窗口的标识符。 |
| **[!UICONTROL 启动图像]** | 要显示的启动图像文件的名称。 如果用户选择启动应用程序，将显示选定的图像而不是应用程序的启动屏幕。 |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



