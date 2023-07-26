---
audience: end-user
title: 发送短信投放
description: 了解如何使用Adobe Campaign Web发送短信
badge: label="Alpha"
source-git-commit: 554e839c2ac715ddc69ed6acfea0844c5436c07a
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 16%

---

# 预览并发送短信投放 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新的隔离指标"
>abstract="投放失败（用户未知、域无效）后被隔离的地址总数与要投放的邮件数有关。"

## 预览短信投放{#preview-sms}

定义消息内容后，即可使用测试用户档案对其进行预览和测试。 如果您已包含个性化内容，则可以使用测试用户档案数据检查此内容在消息中的显示方式。 这样，您就可以确保消息按预期显示，并且任何个性化信息均可正确显示。

预览短信投放的主要步骤如下。 有关如何预览投放的更多详细信息，请参阅 [本节](../preview-test/preview-content.md).

1. 在投放内容页面中，使用 **[!UICONTROL 模拟内容]** 以预览您的个性化内容。

   ![](assets/sms_send_1.png)

1. 单击&#x200B;**[!UICONTROL 添加测试配置文件]**&#x200B;以选择一个或多个测试配置文件。

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png)
    -->

1. 在右侧窗格中，您将找到短信投放预览，其中个性化元素会动态替换为所选用户档案中的数据。

   ![](assets/sms_send_3.png)

现在可审查短信消息并将其发送到受众。

## 测试短信投放 {#test-sms}

替换为 **Adobe Campaign**，则能够在将消息发送到主受众之前对其进行测试，这是验证电子邮件营销活动和识别潜在问题的重要步骤。

发送测试短信是确保投放质量和效果的重要步骤。 测试收件人可以检查各种元素，如链接、选择退出链接和图像，并识别渲染、内容、个性化设置和短信配置中的任何错误。 此过程可帮助您在联系主受众之前彻底评估和优化短信。

![](../assets/do-not-localize/book.png) 了解如何在中发送测试短信 [本节](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png)

## 发送短信投放 {#send-sms}

1. 个性化短信内容后，单击 **[!UICONTROL 审阅并发送]** 来自您的 **[!UICONTROL 投放]** 页面。

   ![](assets/sms_send_4.png)

1. 单击 **[!UICONTROL 准备]** 并监测所提供的进度和统计数据。

   如果发生任何错误，请参阅日志菜单以了解有关失败的详细信息。

1. 通过单击 **[!UICONTROL 发送]** 以继续进行最终的发送过程。

   ![](assets/sms_send_5.png)

1. 通过单击 **[!UICONTROL 发送]** 按钮。

发送投放后，您可以从投放页面跟踪KPI（关键绩效指标）数据，并从 **[!UICONTROL 日志]** 菜单。

您现在可以开始使用内置报告来衡量消息的影响。 [了解详情](../reporting/sms-report.md)




