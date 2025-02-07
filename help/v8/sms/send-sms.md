---
audience: end-user
title: 发送短信投放
description: 了解如何使用Adobe Campaign Web发送短信
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 14%

---

# 预览并发送短信投放 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新的隔离指标"
>abstract="投放失败（用户未知、域无效）后被隔离的地址总数与要投放的邮件数有关。"

## 预览短信投放{#preview-sms}

定义消息内容后，即可使用测试用户档案对其进行预览和测试。 如果您已包含个性化内容，则可以使用测试用户档案数据检查此内容在消息中的显示方式。 这样，您就可以确保消息按预期显示，并且任何个性化信息均可正确显示。

预览短信投放的主要步骤如下。 有关如何预览投放的更多详细信息，请参阅[此部分](../preview-test/preview-content.md)。

1. 在投放内容页面中，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;预览您的个性化内容。

   ![](assets/sms_send_1.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 添加测试轮廓]**&#x200B;以选择一个或多个测试轮廓。

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. 在右侧窗格中，您将找到短信投放预览，其中个性化元素会动态替换为所选用户档案中的数据。

   ![](assets/sms_send_3.png){zoomable="yes"}

现在可审查短信消息并将其发送到受众。

## 测试短信投放 {#test-sms}

使用&#x200B;**Adobe Campaign**，您可以在将邮件发送给主要受众之前对其进行测试，这是验证电子邮件促销活动和识别潜在问题的关键步骤。

发送校样是确保投放质量和效果的重要步骤。 验证收件人可以检查各种元素，如链接、选择退出链接和图像，并识别渲染、内容、个性化设置和短信配置中的任何错误。 此过程可帮助您在联系主受众之前彻底评估和优化短信。

![](../assets/do-not-localize/book.png)在[本节](../preview-test/test-deliveries.md)中了解如何发送校样。

![](assets/sms_send_6.png){zoomable="yes"}

## 发送短信投放 {#send-sms}

1. 个性化短信内容后，从&#x200B;**[!UICONTROL 投放]**&#x200B;页面单击&#x200B;**[!UICONTROL 审阅和发送]**。

   ![](assets/sms_send_4.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 准备]**&#x200B;并监视提供的进度和统计信息。

   如果发生任何错误，请参阅日志菜单以了解有关失败的详细信息。

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以继续最终发送过程，从而发送邮件。

   ![](assets/sms_send_5.png){zoomable="yes"}

   如果短信投放已计划，请单击&#x200B;**[!UICONTROL 按计划发送]**&#x200B;按钮。 在[本节](../msg/gs-messages.md#schedule-the-delivery-sending)中了解有关投放计划的更多信息。


1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;按钮以确认发送操作。

发送投放后，您可以从投放页面跟踪KPI（关键绩效指标）数据，并从&#x200B;**[!UICONTROL 日志]**&#x200B;菜单跟踪数据。

您现在可以开始使用内置报告来衡量消息的影响。 [了解详情](../reporting/sms-report.md)
