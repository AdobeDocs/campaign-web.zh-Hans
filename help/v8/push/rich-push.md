---
audience: end-user
title: 设计富推送通知投放
description: 了解如何使用Adobe Campaign Web设计Android富推送通知投放
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 7%

---

# 设计 Android 富推送投放 {#rich-push}



>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="丰富的推送投放"
>abstract="您现在可以通过 Android 发送富推送通知。目前，此功能可用性有限。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hans" text="请参阅发行说明"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="稍后提醒按钮"
>abstract="**稍后提醒**&#x200B;按钮提供了计划提醒的选项。时间戳字段需要一个表示 epoch 的值（以秒为单位）。"

>[!AVAILABILITY]
>
>此功能位于 **有限可用性** （洛杉矶）。

使用Firebase Cloud Messaging，您可以选择两种类型的消息：

* 此 **[!UICONTROL 数据消息]** 由客户端应用程序处理。 这些消息直接发送到移动设备应用程序，后者在设备上生成并显示Android通知。 数据消息仅包含您的自定义应用程序变量。

* 此 **[!UICONTROL 通知消息]**，由FCM SDK自动处理。 FCM会代表客户端应用程序在用户设备上自动显示消息。 通知消息包含预定义的一组参数和选项，但仍可以使用自定义应用程序变量进一步个性化。

![](assets/rich_push.png){zoomable="yes"}

## 定义通知的内容 {#push-message}

创建推送投放后，即可定义其内容。 提供了三个模板：

* **默认模板** 允许您发送带有简单图标和随附图像的通知。

* **基本模板** 可以在通知中包含文本、图像和按钮。

* **轮播模板** 允许您发送包含用户可以轻扫的文本和多个图像的通知。

浏览以下选项卡，详细了解如何个性化这些模板。

>[!BEGINTABS]

>[!TAB 默认模板]

1. 从 **[!UICONTROL 模板]** 下拉列表，选择 **[!UICONTROL 默认]**.

   ![](assets/rich_push_default.png)

1. 要撰写消息，请在 **[!UICONTROL 标题]** 和 **[!UICONTROL 消息]** 字段。

   ![](assets/rich_push_default_2.png)

1. 使用表达式编辑器定义内容、个性化数据和添加动态内容。 [了解更多信息](../personalization/personalize.md)

1. 定义 **[!UICONTROL 点击操作]** 与用户单击您的通知相关联。 这会确定用户与通知交互时的行为，例如打开特定屏幕或在应用程序中执行特定操作。

1. 要进一步个性化您的推送通知，您可以选择 **[!UICONTROL 图像]** 添加到推送通知和通知的URL **[!UICONTROL 图标]** 以在用户档案的设备上显示。

   ![](assets/rich_push_default_3.png)

1. 配置 **[!UICONTROL 高级设置]** 的推送通知。 [了解更多信息](#push-advanced)

定义消息内容后，您可以使用测试订阅者来预览和测试消息。

>[!TAB 基本模板]

1. 从 **[!UICONTROL 模板]** 下拉列表，选择 **[!UICONTROL 基本]**.

   ![](assets/rich_push_basic.png)

1. 要撰写消息，请在 **[!UICONTROL 标题]**， **[!UICONTROL 消息]** 和 **[!UICONTROL 扩展的消息]** 字段。

   此 **[!UICONTROL 消息]** 文本显示在折叠的视图中，而 **[!UICONTROL 扩展的消息]** 在展开通知时显示。

   ![](assets/rich_push_basic_2.png)

1. 使用表达式编辑器定义内容、个性化数据和添加动态内容。 [了解更多信息](../personalization/personalize.md)

1. 添加定义 **[!UICONTROL 点击操作]** 与用户单击您的通知相关联。 这会确定用户与通知交互时的行为，例如打开特定屏幕或在应用程序中执行特定操作。

1. 选择 **[!UICONTROL 链接类型]** 您添加到的 **[!UICONTROL 点击操作]** 字段：

   * **[!UICONTROL Web URL]**：Web URL可将用户指引到在线内容。 单击后，它们将提示设备的默认Web浏览器打开并导航到指定的URL。

   * **[!UICONTROL 深层链接]**：深层链接是指引导用户访问应用程序中特定部分的URL，即使应用程序已关闭。 单击时，会显示一个对话框，允许用户从能够处理链接的各种应用程序中进行选择。

   * **[!UICONTROL 打开应用程序]**：打开应用程序URL，以便直接连接到应用程序中的内容。 它使您的应用程序能够绕过消除歧义对话框，将自身确立为特定类型链接的默认处理程序。

   有关如何处理Android应用程序链接的更多信息，请参阅 [Android开发人员文档](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. 要进一步个性化您的推送通知，您可以选择 **[!UICONTROL 图像]** 添加到推送通知和通知的URL **[!UICONTROL 图标]** 以在用户档案的设备上显示。

1. 单击 **[!UICONTROL “添加”按钮]** 并填写以下字段：

   * **[!UICONTROL 标签]**：按钮上显示的文本。
   * **[!UICONTROL 链接URI]**：指定单击按钮时要执行的URI。
   * **[!UICONTROL 链接类型]**：链接类型 **[!UICONTROL Web URL]**， **[!UICONTROL 深层链接]**，或 **[!UICONTROL 打开应用程序]**.

   您可以选择在推送通知中最多包含三个按钮。 如果您选择 **[!UICONTROL “稍后提醒”按钮]**&#x200B;中，您最多只能包含两个按钮。

   ![](assets/rich_push_basic_4.png)

1. 单击 **[!UICONTROL 稍后添加提醒]** 按钮以向推送通知添加稍后提醒选项。 输入 **[!UICONTROL 标签]** 和 **[!UICONTROL 时间戳]**.

   时间戳字段需要一个表示纪元的值（以秒为单位）。

   ![](assets/rich_push_basic_5.png)

1. 配置 **[!UICONTROL 高级设置]** 的推送通知。 [了解更多信息](#push-advanced)

定义消息内容后，您可以使用测试订阅者来预览和测试消息。

>[!TAB 轮播模板]

1. 从 **[!UICONTROL 模板]** 下拉列表，选择 **[!UICONTROL 轮播]**.

   ![](assets/rich_push_carousel.png)

1. 要撰写消息，请在 **[!UICONTROL 标题]**， **[!UICONTROL 消息]** 和 **[!UICONTROL 扩展的消息]** 字段。

   此 **[!UICONTROL 消息]** 文本显示在折叠的视图中，而 **[!UICONTROL 扩展的消息]** 在展开通知时显示。

   ![](assets/rich_push_carousel_1.png)

1. 使用表达式编辑器定义内容、个性化数据和添加动态内容。 [了解更多信息](../personalization/personalize.md)

1. 添加定义 **[!UICONTROL 点击操作]** 与用户单击您的通知相关联。 这会确定用户与通知交互时的行为，例如打开特定屏幕或在应用程序中执行特定操作。

1. 选择 **[!UICONTROL 链接类型]** 您添加到的 **[!UICONTROL 点击操作]** 字段：

   * **[!UICONTROL Web UR]**L： Web URL可将用户指引到在线内容。 单击后，它们将提示设备的默认Web浏览器打开并导航到指定的URL。

   * **[!UICONTROL 深层链接]**：深层链接是指引导用户访问应用程序中特定部分的URL，即使应用程序已关闭。 单击时，会显示一个对话框，允许用户从能够处理链接的各种应用程序中进行选择。

   * **[!UICONTROL 打开应用程序]**：打开应用程序URL，以便直接连接到应用程序中的内容。 它使您的应用程序能够绕过消除歧义对话框，将自身确立为特定类型链接的默认处理程序。

   有关如何处理Android应用程序链接的更多信息，请参阅 [Android开发人员文档](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. 要进一步个性化您的推送通知，您可以选择通知的 **[!UICONTROL 图标]** 以在用户档案的设备上显示。

1. 选择如何 **[!UICONTROL 轮播]** 运行：

   * **[!UICONTROL 自动]**：将图像作为幻灯片自动循环，以预定义的时间间隔转换。
   * **[!UICONTROL 手动]**：允许用户在幻灯片之间手动滑动以浏览图像。

     启用 **[!UICONTROL 影片胶片]** 选项，在主幻灯片旁包括上一张和下一张图像的预览。

1. 单击 **[!UICONTROL 添加图像]** 并输入图像URL和文本。

   确保您至少包含三个图像，最多包含五个图像。

   ![](assets/rich_push_carousel_3.png)

1. 使用向下和向上箭头处理图像的顺序。

1. 配置 **[!UICONTROL 高级设置]** 的推送通知。 [了解更多信息](#push-advanced)

定义消息内容后，您可以使用测试订阅者来预览和测试消息。

>[!ENDTABS]

## 推送通知高级设置 {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| 参数 | 说明 |
|---------|---------|
| **[!UICONTROL 图标颜色]** | 使用十六进制颜色代码设置图标的颜色。 |
| **[!UICONTROL 标题颜色]** | 使用十六进制颜色代码设置标题的颜色。 |
| **[!UICONTROL 消息文本颜色]** | 使用十六进制颜色代码设置消息文本的颜色。 |
| **[!UICONTROL 通知背景颜色]** | 使用十六进制颜色代码设置通知背景的颜色。 |
| **[!UICONTROL 声音]** | 设置设备收到通知时播放的声音。 |
| **[!UICONTROL 通知计数]** | 设置直接在应用程序图标上显示的新未读信息数。 这样用户即可迅速了解待处理通知的数量。 |
| **[!UICONTROL 渠道ID]** | 设置通知的渠道ID。 在收到任何具有此渠道ID的通知之前，应用程序必须创建具有此渠道ID的渠道。 |
| **[!UICONTROL 标记]** | 设置用于替换通知抽屉中现有通知的标识符。 这有助于防止累积多个通知，并确保只显示最新的相关通知。 |
| **[!UICONTROL 优先级]** | 设置通知的优先级，可以是默认、最小、低或高。 优先级决定了通知的重要性和紧迫性，会影响通知的显示方式以及它是否可以绕过某些系统设置。 有关详细信息，请参见 [FCM文档](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL 可见性]** | 设置通知的可见性级别，可以是公共、私有或机密。 可见性级别确定通知内容在锁屏界面和其他敏感区域上显示的程度。 欲了解更多信息，请参见 [FCM文档](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL 粘性通知]** | 激活后，通知仍保持可见，即使用户单击它也是如此。 <br>如果停用，则当用户与通知交互时，会自动取消通知。 粘性行为允许重要通知在屏幕上保留较长时间。 |
| **[!UICONTROL 应用程序变量]** | 允许您定义通知行为。 可完全自定义这些变量，并将其纳入发送到移动设备的消息负载。 |
