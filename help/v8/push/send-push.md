---
audience: end-user
title: 发送推送通知投放
description: 了解如何使用Adobe Campaign Web发送推送通知投放
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 5%

---

# 预览并发送推送投放 {#send-push-delivery}

## 预览推送通知投放 {#preview-push}

定义消息内容后，您可以利用测试订阅者来预览和测试消息。 如果您已包含个性化内容，则可以使用测试用户档案数据检查此内容在消息中的显示方式。 这样，您就可以确保消息正确呈现，并正确合并个性化元素。

预览推送通知的主要步骤如下。 有关如何预览投放的更多详细信息，请参阅 [本节](../preview-test/preview-content.md).

1. 在投放内容页面中，使用 **[!UICONTROL 模拟内容]** 以预览您的个性化内容。

   ![](assets/push_send_1.png){zoomable=&quot;yes&quot;}

1. 单击 **[!UICONTROL 添加订阅者]** 选择一个或多个用户档案，以在推送通知内容中预览其数据。


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. 在右侧窗格中，您将找到推送通知的预览，其中个性化元素会动态替换为所选用户档案中的数据。

   ![](assets/push_send_7.png){zoomable=&quot;yes&quot;}

您现在可以查看推送通知并将其发送给受众。

## 测试您的推送通知投放 {#test-push}

使用 **Adobe Campaign**，则能够在将验证发送到主受众之前发送它们。 此步骤对于验证您的投放和识别任何问题都非常重要。

测试用户档案是验证收件人。 他们可以查看和验证组件和设置（如链接、图像和个性化），确保最佳性能并检测任何错误。 此过程可帮助您在联系主受众之前优化推送通知。 [了解如何发送校样](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable=&quot;yes&quot;}

## 发送推送通知投放 {#send-push}

1. 个性化推送通知内容后，单击 **[!UICONTROL 审阅并发送]** 来自您的 **[!UICONTROL 投放]** 页面。

   ![](assets/push_send_2.png){zoomable=&quot;yes&quot;}

1. 单击 **[!UICONTROL 准备]** 并监测所提供的进度和统计数据。

   如果发生任何错误，请参阅日志菜单以了解有关失败的详细信息。

   ![](assets/push_send_3.png){zoomable=&quot;yes&quot;}

1. 通过单击 **[!UICONTROL 发送]** 以继续进行最终的发送过程。

1. 通过单击 **[!UICONTROL 发送]**.

   如果已计划推送传送，请单击 **[!UICONTROL 按计划发送]** 按钮。 在中了解有关投放计划的更多信息 [本节](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png){zoomable=&quot;yes&quot;}

发送投放后，您可以从投放页面跟踪KPI（关键绩效指标）数据，并从 **[!UICONTROL 日志]** 菜单。

您现在可以开始使用内置报告来衡量消息的影响。 [了解详情](../reporting/push-report.md)
