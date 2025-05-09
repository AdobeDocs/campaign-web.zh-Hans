---
audience: end-user
title: 预览和发送直邮投放
description: 了解如何使用Adobe Campaign Web预览和发送直邮投放
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# 预览和发送直邮投放 {#send-direct-mail}

为直邮投放配置提取文件后，请使用测试用户档案进行预览。 如果包含个性化内容，请使用测试配置文件数据检查此内容在列中的显示方式。 这可以确保正确呈现文件内容并适当合并个性化元素。

当提取文件就绪后，发送直邮投放以生成文件并与直邮提供商共享。 [了解如何发送直邮投放](#dm-send)

## 预览提取文件 {#preview-dm}

预览提取文件的主要步骤如下。 有关如何预览投放的更多详细信息，请参阅[此部分](../preview-test/preview-content.md)。

1. 在投放内容页面中，使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;预览您的个性化内容。

   ![在投放内容页面中显示模拟内容选项的屏幕截图](assets/dm-simulate.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 添加测试配置文件]**&#x200B;以选择一个或多个配置文件并在提取文件内容中预览其数据。

1. 在右侧窗格中，查看提取文件的预览，其中个性化元素会动态替换为所选用户档案中的数据。

   ![在右窗格中显示提取文件预览的屏幕快照](assets/dm-preview-right.png){zoomable="yes"}

## 发送校样 {#test-dm}

使用&#x200B;**Adobe Campaign**，在将校样交付给主要受众之前发送校样。 此步骤将验证您的投放并识别任何问题。 测试收件人可审核个性化设置等元素，确保最佳性能和检测错误。 此流程可在联系主受众之前优化提取文件。

对于直邮投放，发送校样会使用来自所选测试用户档案的数据生成提取文件示例。 要访问它，请执行以下步骤：

1. 在模拟内容屏幕中，单击&#x200B;**[!UICONTROL 发送校样]**&#x200B;按钮，然后执行与任何类型的投放相同的步骤以发送校样。 [了解如何发送校样](../preview-test/test-deliveries.md)

1. 发送校样后，可从&#x200B;**[!UICONTROL 查看校样]**&#x200B;按钮或投放列表访问该校样。 [了解如何访问已发送的校样](../preview-test/test-deliveries.md#access-test-deliveries)

1. 在验证投放仪表板中，单击&#x200B;**[!UICONTROL 预览文件]**&#x200B;按钮以访问提取文件的预览。

   ![在验证投放仪表板中显示预览文件选项的屏幕截图](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >预览文件中只显示前100行。

## 发送直邮投放 {#send-dm}

准备好将直邮发送给客户后，请发送投放，以在指定的提取文件中开始数据提取。 为此，请执行以下步骤：

1. 设计提取文件的内容后，从&#x200B;**[!UICONTROL 投放]**&#x200B;页面单击&#x200B;**[!UICONTROL 审阅并发送]**。

   ![在投放页面中显示审阅和发送选项的屏幕截图](assets/dm-review-send.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 准备]**&#x200B;并监视提供的进度和统计信息。

   如果发生任何错误，请参阅&#x200B;**[!UICONTROL 日志]**&#x200B;菜单以了解有关失败的详细信息。

   ![显示准备选项和日志菜单的屏幕快照](assets/dm-prepare.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以继续最终发送过程，从而发送邮件。

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以确认发送操作。

   如果已计划直邮投放，请单击&#x200B;**[!UICONTROL 按计划发送]**&#x200B;按钮。 在[本节](../msg/gs-messages.md#schedule-the-delivery-sending)中了解有关投放计划的更多信息。

发送投放后，将自动生成提取文件并将其导出到在投放模板的[高级设置](../advanced-settings/delivery-settings.md)中选择的&#x200B;**[!UICONTROL 路由]**&#x200B;外部帐户中指定的位置。

跟踪投放页面中的KPI（关键绩效指标）数据和&#x200B;**[!UICONTROL 日志]**&#x200B;菜单中的数据。

开始使用内置报告衡量消息的影响。 [了解详情](../reporting/direct-mail.md)