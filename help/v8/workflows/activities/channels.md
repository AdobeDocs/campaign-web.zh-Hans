---
audience: end-user
title: 使用投放工作流活动
description: 了解如何添加投放工作流活动（电子邮件、推送、短信、直邮）
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 40%

---

# 电子邮件、短信、推送、直邮活动 {#channel}

通过Adobe Campaign Web，您可以跨电子邮件、短信、直邮和推送渠道自动执行营销活动。 可将渠道活动合并到工作流画布中，以创建可根据客户行为和数据触发操作的跨渠道工作流。

例如，创建一个欢迎电子邮件促销活动，其中包含跨不同渠道的一系列消息，例如电子邮件、短信、推送和直邮。 您还可以在客户完成购买后发送跟进电子邮件，或通过短信向客户发送个性化的生日消息。

通过使用渠道活动，创建全面的个性化营销活动，在多个接触点吸引客户并促进转化。

>[!NOTE]
>
>您还可以在营销活动工作流上下文之外创建一次性投放。 请参阅以下部分以了解详情：
>* [创建独立电子邮件投放](../../email/create-email.md)
>* [创建独立SMS投放](../../sms/create-sms.md)
>* [创建独立推送投放](../../push/create-push.md)
>* [创建独立直邮投放](../../direct-mail/create-direct-mail.md)

## 先决条件 {#channel-activity-prereq}

开始使用相关活动构建工作流：

* 在插入渠道活动之前，请定义受众。 受众是投放的主要目标：接收消息的用户档案。 在营销活动工作流的上下文中发送消息时，未在渠道活动中定义消息受众，而是在专用活动中进行定义，例如：

   * **生成受众**&#x200B;活动。 [了解详情](build-audience.md)。

     ![在工作流中添加投放的屏幕截图](../../msg/assets/add-delivery-in-wf.png)

   * **加载文件**&#x200B;活动，后跟&#x200B;**协调**&#x200B;活动。 [了解详情](load-file.md)。

     ![显示工作流协调条件的屏幕截图](../assets/workflow-reconciliation-criteria.png)

* 要发送定期投放，请使用&#x200B;**调度程序**&#x200B;活动启动工作流。 对一次性投放使用&#x200B;**调度程序**&#x200B;活动来设置该投放的联系日期。 还可以在投放设置中设置该联系日期。 请参阅[此小节](scheduler.md)。

## 配置“渠道”活动 {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="”电子邮件“活动"
>abstract="电子邮件活动有助于在工作流程中发送电子邮件，允许一次性和重复发送消息。它可自动将电子邮件发送到在同一工作流程中计算的目标。可将渠道活动合并到工作流画布中，以创建可根据客户行为和数据触发操作的跨渠道工作流。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="”短信“活动"
>abstract="短信活动有助于在工作流程中发送短信，允许一次性和重复发送消息。它可自动将短信发送到在同一工作流程中计算的目标。可将渠道活动合并到工作流画布中，以创建可根据客户行为和数据触发操作的跨渠道工作流。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="”推送 iOS“ 活动"
>abstract="推送 iOS 活动简化作为工作流的一部分发送 iOS 推送通知的过程。可一次性和重复投放，自动将 iOS 推送通知发送到同一工作流程中的预定义目标。可将渠道活动合并到工作流画布中，以创建可根据客户行为和数据触发操作的跨渠道工作流。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="”推送 Android“ 活动"
>abstract="推送 Android 活动简化作为工作流的一部分发送 Android 推送通知的过程。可一次性和重复投放，自动将 Android 推送通知发送到同一工作流程中的预定义目标。可将渠道活动合并到工作流画布中，以创建可根据客户行为和数据触发操作的跨渠道工作流。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="”直邮“活动"
>abstract="直邮活动有助于在工作流中直接发送邮件，允许一次性和重复发送消息。它可自动生成直邮提供商所需的提取文件。可将渠道活动合并到工作流画布中，以创建可根据客户行为和数据触发操作的跨渠道工作流。"

要在工作流上下文中设置投放，请执行以下步骤：

1. 添加渠道活动：**[!UICONTROL 电子邮件]**、**[!UICONTROL 短信]**、**[!UICONTROL 推送通知(Android)]**、**[!UICONTROL 推送通知(iOS)]**&#x200B;或&#x200B;**[!UICONTROL 直邮]**。

1. 选择&#x200B;**投放类型**：单次或循环。

   * **单次投放**&#x200B;是只发送一次的一次性投放，如“黑色星期五”电子邮件。
   * 根据在[调度程序活动](scheduler.md)中定义的执行频率，多次发送&#x200B;**循环投放**。 每次运行工作流时，都会重新计算受众，并将投放内容发送到更新后的受众，其中包含更新的内容。 这可以是每周新闻稿或定期生日电子邮件。

1. 选择投放&#x200B;**模板**。模板是特定于渠道的预配置投放设置。 每个渠道都有内置模板可用，默认情况下会预填充。 [了解详情](../../msg/delivery-template.md)

   ![显示工作流中投放活动的屏幕截图](../assets/delivery-activity-in-wf.png)

   从渠道活动配置左窗格中选择模板。 如果之前选择的受众与渠道不兼容，则无法选择模板。 要解决此问题，请更新&#x200B;**生成受众**&#x200B;活动，以选择具有正确目标映射的受众。在[本节](../../audience/targeting-dimensions.md)中了解有关目标映射的详细信息。

1. 单击&#x200B;**创建投放**。定义消息设置和内容的方式与创建独立投放的方式相同。测试和模拟内容。 [了解详情](../../msg/gs-messages.md)

1. 导航回工作流。 要继续工作流，请切换&#x200B;**生成叫客过渡**&#x200B;选项以在渠道活动后添加过渡。

1. 单击&#x200B;**开始**&#x200B;启动您的工作流。

   默认情况下，启动工作流会触发消息准备阶段，而不会立即发送消息。

1. 打开您的渠道活动，通过&#x200B;**查看和发送**&#x200B;按钮确认发送。

1. 在投放仪表板中，单击&#x200B;**发送**。

## 示例 {#cross-channel-workflow-sample}

这是一个具有分段和两次投放的跨渠道工作流示例。 该工作流面向居住在巴黎并对咖啡机感兴趣的所有客户。 在此群体中，会向常规客户发送电子邮件，向VIP客户发送短信。

![显示跨渠道工作流示例的屏幕截图](../assets/workflow-channel-example.png)

您还可以创建一个循环工作流，以便在每个月的第一天晚上8点向所有居住在巴黎的客户发送个性化短信。

![显示循环工作流示例的屏幕截图](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->