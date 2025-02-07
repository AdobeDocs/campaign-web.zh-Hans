---
product: campaign
title: 使用投放
description: 了解如何在 Campaign Web 中创建您的第一个投放
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 803a20ac-e75f-45c6-af89-054b84eb3405
source-git-commit: 387a69abf4b97cd202c1a7e24bcf14c6af442714
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 88%

---

# 创建投放 {#create-delivery}

您可以从&#x200B;**[!UICONTROL 投放]**&#x200B;左侧菜单创建独立投放，也可以在工作流（包含或未包含在营销活动中）的上下文中创建投放。

浏览以下选项卡以了解如何创建投放：

>[!BEGINTABS]

>[!TAB 创建独立投放]

要创建独立投放，请执行以下步骤：

1. 浏览到左侧导航上的&#x200B;**[!UICONTROL 投放]**&#x200B;菜单，然后单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮。

   ![](assets/create-a-delivery.png){zoomable="yes"}

1. 选择投放的渠道。
1. 为主要目标和对照组定义投放受众。[了解有关受众的详细信息](../audience/about-recipients.md)。

   ![](assets/select-audience.png){zoomable="yes"}{width="70%" align="left"}

1. 定义消息内容。在以下各部分中了解有关投放渠道以及如何定义投放内容的更多信息：

   * [电子邮件渠道](../email/create-email.md)
   * [推送通知渠道](../push/gs-push.md)
   * [短信渠道](../sms/create-sms.md)

1. （可选）定义投放[计划](#gs-schedule)。如果未定义计划，则在单击&#x200B;**[!UICONTROL 发送]**&#x200B;按钮后立即发送消息。
1. 单击&#x200B;**[!UICONTROL 查看并发送]**&#x200B;按钮可检查您的设置。
1. 使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮可测试您的投放和个性化设置。在[此章节](../preview-test/preview-test.md)中详细了解消息模拟。
1. 单击&#x200B;**[!UICONTROL 准备]**&#x200B;按钮可计算目标群体并生成消息。准备步骤可能需要几分钟时间。准备完成后，消息随时即可发送。如果出现错误，请浏览到&#x200B;**日志**&#x200B;检查警报和警告。
1. 检查结果，然后单击&#x200B;**[!UICONTROL 发送]**&#x200B;按钮开始发送消息。
1. 发送消息后，浏览到&#x200B;**报告**&#x200B;部分以访问关键量度。在[此章节](../reporting/delivery-reports.md)中详细了解投放报告。

>[!TAB 在工作流中创建投放]

要在工作流中创建投放，请执行以下步骤：

1. 创建工作流或打开现有工作流。[了解有关工作流的详细信息](../workflows/gs-workflow-creation.md#gs-workflow-steps)
1. 添加和配置[**[!UICONTROL 构建受众]**](../workflows/activities/build-audience.md)活动。
1. 单击 `+` 图标并选择投放活动：**[!UICONTROL 电子邮件]**、**[!UICONTROL 短信]**、**[!UICONTROL 推送通知 (Android)]** 或&#x200B;**[!UICONTROL 推送通知 (iOS)]**。在[本节](../workflows/activities/channels.md)中进一步了解工作流中的投放渠道活动以及如何定义投放内容。

   ![](assets/add-delivery-in-wf.png){zoomable="yes"}

1. 启动工作流，并检查日志。

您还可以在不创建工作流的情况下在营销活动中添加投放。为此，请浏览到营销活动的&#x200B;**[!UICONTROL 投放]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮。

![](assets/new-campaign-delivery.png){zoomable="yes"}

配置步骤与独立投放类似。

有关如何配置营销活动和管理属于营销活动的投放的更多信息，请参阅[此章节](../campaigns/gs-campaigns.md)。

>[!ENDTABS]

## 添加个性化内容 {#personalization}

由 Adobe Campaign 投放的消息可以通过各种方式实现个性化。[详细了解个性化功能](../personalization/gs-personalization.md)。

使用 Campaign 创建动态内容并发送个性化消息。可以结合个性化功能来改进您的消息并创建自定义用户体验。

可以通过以下方式个性化邮件内容：

* 插入动态&#x200B;**个性化字段**

  个性化字段用于邮件的第一级个性化。您可以从个性化编辑器中选择数据库中可用的任何字段。对于投放，您可以选择与收件人、邮件或投放相关的任何字段。可将这些个性化属性插入邮件的主题行或正文中。[了解详情](../personalization/personalize.md)

* 正在插入预定义的&#x200B;**表达式片段**

  Campaign提供了一组表达式片段，其中包含您可以插入到投放中的特定渲染。 例如，您可以添加徽标、问候邮件或指向邮件的镜像页面的链接。表达式片段可从个性化编辑器中的专用条目获取。 此外，您还可以创建自己的表达式片段以满足您的需求。 [了解如何使用表达式片段](../content/use-expression-fragments.md)

* 创建&#x200B;**条件内容**

  例如，配置条件内容以根据收件人的轮廓添加动态个性化内容。满足特定条件时可插入文本块和/或图像。[了解详情](../personalization/conditions.md)

* 添加&#x200B;**个性化产品建议**

  根据收件人位置、当前天气或上次采购订单，在您的消息内容中插入个性化产品建议。[了解详情](../msg/offers.md)

## 预览和测试投放

定义消息内容后，您可以预览内容以控制消息的渲染，并使用测试轮廓检查个性化设置。[了解详情](../preview-test/preview-test.md)

## 安排发送投放 {#gs-schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="设置联系日期和时间"
>abstract="定义发送投放的日期和确切时间。通过选择最适合您的营销消息的时间，可尽量提高打开率。"

您可以设置发送信息的日期和确切时间。通过选择最适合您的营销消息的时间，可尽量提高打开率。

要安排发送投放，请打开您的投放并浏览到&#x200B;**[!UICONTROL 安排]**&#x200B;部分。使用&#x200B;**[!UICONTROL 启用安排]**&#x200B;切换开关以激活该功能，然后设置要发送的日期和时间。发送投放后，实际发送将在您定义的联系日期开始。

![](assets/schedule.png){zoomable="yes"}

默认情况下，**[!UICONTROL 启用发送前确认]**&#x200B;选项处于启用状态。此选项要求您在安排的日期和时间发送投放之前确认发送。如果您需要在安排的日期和时间自动发送投放，可禁用此选项。

在[此部分](../monitor/prepare-send.md#schedule-the-send)中了解发送计划投放的步骤。

## 监控和跟踪日志 {#gs-tracking-logs}

在发送后监控投放是确保营销活动有效并接触到客户的重要步骤。

您可以在发送投放后进行监控，并了解如何管理投放失败和隔离。

请参阅[本章节](../reporting/gs-reports.md)以详细了解监控和跟踪功能。
