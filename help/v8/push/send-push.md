---
audience: end-user
title: 发送推送通知投放
description: 了解如何使用Adobe Campaign Web发送推送通知投放
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---

# 预览并发送推送投放 {#send-push-delivery}

## 预览推送通知投放 {#preview-push}

定义消息内容后，使用测试订阅者来预览和测试消息。 如果包含个性化内容，请使用测试用户档案数据检查此内容在消息中的显示方式。 这可以确保消息正确呈现，并适当合并个性化元素。

预览推送通知的主要步骤如下。 有关如何预览投放的更多详细信息，请参阅[此部分](../preview-test/preview-content.md)。

1. 在投放内容页面中，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;预览您的个性化内容。

   ![在投放内容页面中预览个性化内容](assets/push_send_1.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 添加订阅者]**&#x200B;可选择一个或多个用户档案，以便在推送通知内容中预览其数据。

   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. 在右侧窗格中，查找推送通知的预览，其中个性化元素会动态替换为所选用户档案中的数据。

   ![显示个性化元素已被配置文件数据替换的预览窗格](assets/push_send_7.png){zoomable="yes"}

查看您的推送通知并将其发送给受众。

## 测试您的推送通知投放 {#test-push}

使用&#x200B;**Adobe Campaign**，在将校样交付给主要受众之前发送校样。 此步骤将验证您的投放并识别任何问题。

测试用户档案充当验证收件人。 他们审查并验证组件和设置（如链接、图像和个性化），确保最佳性能和检测错误。 此流程可在联系主受众之前优化推送通知。 [了解如何发送校样](../preview-test/test-deliveries.md#subscribers)。

![正在测试具有证明收件人的推送通知投放](assets/push_send_6.png){zoomable="yes"}

## 发送推送通知投放 {#send-push}

1. 个性化推送通知内容后，从&#x200B;**[!UICONTROL 投放]**&#x200B;页面中单击&#x200B;**[!UICONTROL 审阅并发送]**。

   在投放页面上![查看和发送按钮](assets/push_send_2.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 准备]**&#x200B;并监视提供的进度和统计信息。

   如果发生错误，请参阅日志菜单以了解有关失败的详细信息。

   ![正在监视准备进度和统计信息](assets/push_send_3.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以继续最终发送过程，从而发送邮件。

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以确认发送操作。

   如果计划了推送传送，请单击&#x200B;**[!UICONTROL 按计划发送]**&#x200B;按钮。 在[本节](../msg/gs-messages.md#schedule-the-delivery-sending)中了解有关投放计划的更多信息。

   针对计划的推送传递![按计划发送按钮](assets/push_send_4.png){zoomable="yes"}

发送投放后，从投放页面跟踪关键绩效指标(KPI)数据，并从&#x200B;**[!UICONTROL 日志]**&#x200B;菜单跟踪数据。

开始使用内置报告衡量消息的影响。 [了解详情](../reporting/push-report.md)。