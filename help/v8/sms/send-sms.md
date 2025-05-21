---
audience: end-user
title: 发送短信投放
description: 了解如何使用Adobe Campaign Web发送短信
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 12%

---

# 预览并发送短信投放 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新的隔离指标"
>abstract="投放失败（用户未知、域无效）后被隔离的地址总数与要投放的邮件数有关。"

## 预览短信投放 {#preview-sms}

定义消息内容后，使用测试用户档案进行预览和测试。 如果包含个性化内容，请使用测试用户档案数据检查此内容在消息中的显示方式。 这可确保消息按预期显示，并正确显示个性化信息。

预览短信投放的主要步骤如下。 有关如何预览投放的更多详细信息，请参阅[此部分](../preview-test/preview-content.md)。

1. 在投放内容页面中，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;预览您的个性化内容。

   ![预览个性化短信内容](assets/sms_send_1.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 添加测试轮廓]**&#x200B;以选择一个或多个测试轮廓。

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. 在右侧窗格中，查看SMS投放预览，其中个性化元素会动态替换为所选用户档案中的数据。

   ![显示个性化SMS投放的预览窗格](assets/sms_send_3.png){zoomable="yes"}

审阅短信消息并将其发送给受众。

## 测试短信投放 {#test-sms}

使用&#x200B;**Adobe Campaign**，在将消息发送给主受众之前对其进行测试。 此步骤将验证您的电子邮件促销活动并识别潜在问题。

发送校样对于确保投放的质量和有效性至关重要。 验证收件人会审查各种元素，如链接、选择退出链接和图像，并识别渲染、内容、个性化设置和短信配置中的任何错误。 此过程会在联系主受众之前彻底评估和优化您的短信。

![用于发送校样的书本图标](../assets/do-not-localize/book.png)了解如何在[此部分](../preview-test/test-deliveries.md)中发送校样。

![正在测试短信投放](assets/sms_send_6.png){zoomable="yes"}

## 发送短信投放 {#send-sms}

1. 个性化短信内容后，从&#x200B;**[!UICONTROL 投放]**&#x200B;页面单击&#x200B;**[!UICONTROL 审阅和发送]**。

   ![审阅并发送短信投放](assets/sms_send_4.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 准备]**&#x200B;并监视提供的进度和统计信息。

   如果发生错误，请参阅日志菜单以了解有关失败的详细信息。

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以继续最终发送过程，从而发送邮件。

   ![发送短信投放](assets/sms_send_5.png){zoomable="yes"}

   如果短信投放已计划，请单击&#x200B;**[!UICONTROL 按计划发送]**&#x200B;按钮。 在[本节](../msg/gs-messages.md#schedule-the-delivery-sending)中了解有关投放计划的更多信息。

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;按钮以确认发送操作。

发送投放后，从投放页面跟踪KPI（关键绩效指标）数据，并从&#x200B;**[!UICONTROL 日志]**&#x200B;菜单跟踪数据。

开始使用内置报告衡量消息的影响。 [了解详情](../reporting/sms-report.md)