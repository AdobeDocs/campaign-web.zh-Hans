---
audience: end-user
title: 预览投放内容
description: 了解如何使用Campaign Web用户界面预览投放内容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 1%

---

# 预览消息内容 {#preview-content}

使用[!DNL Campaign]内容模拟功能在发送邮件之前预览邮件内容。 此功能允许您控制个性化并检查消息向收件人显示的方式。

要预览投放内容，请执行以下步骤：

1. 浏览到投放的编辑内容屏幕或[通过电子邮件发送Designer](../email/get-started-email-designer.md)。

1. 单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮。

   ![显示模拟内容按钮的图像](assets/simulate-button.png){zoomable="yes"}

1. 选择用于预览内容的配置文件。 要执行此操作，请单击&#x200B;**[!UICONTROL 添加测试配置文件]**&#x200B;按钮（适用于电子邮件和短信）或&#x200B;**[!UICONTROL 添加订阅者]**&#x200B;按钮（适用于推送通知）。

1. 组合用户档案和测试用户档案以预览电子邮件或短信消息。

   * **[!UICONTROL 测试用户档案]**&#x200B;选项卡列出了所有测试用户档案，它们是数据库中的其他虚构收件人。 [了解如何使用测试用户档案](../audience/test-profiles.md)。

   * **[!UICONTROL 配置文件]**&#x200B;选项卡列出了数据库中存储的所有配置文件。 [了解如何使用用户档案](../audience/about-recipients.md)。

   ![显示所选配置文件的图像](assets/simulate-select-profiles.png){zoomable="yes"}

1. 浏览测试配置文件或配置文件列表时，请使用筛选条件来优化搜索。 例如，定义规则以查找所有状态为&#x200B;**[!UICONTROL 潜在客户]**&#x200B;的测试配置文件。 [了解如何使用查询建模器](../query/query-modeler-overview.md)添加规则。

   ![显示应用于测试用户档案的过滤器的图像](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 选择]**&#x200B;以确认您的选择。

   投放内容的预览显示在&#x200B;**[!UICONTROL 模拟]**&#x200B;屏幕的右窗格中。 个性化元素被替换为在左窗格中选择的配置文件中的数据。

   ![显示投放内容预览的图像](assets/simulate-preview.png){zoomable="yes"}

1. 如果添加了多个用户档案，请在列表中的这些用户档案之间切换以预览相应的投放内容。 使用左窗格中的相应按钮添加更多测试配置文件或清除您的选择。

1. 对于电子邮件投放，请调整&#x200B;**[!UICONTROL 缩放级别]**，并使用右上角的专用图标在桌面或移动设备上预览您的内容。

1. 从&#x200B;**[!UICONTROL 模拟]**&#x200B;屏幕中，您还可以：
   * 将校样发送给特定收件人进行验证 — [了解更多](test-deliveries.md)。
   * 访问已发送校样的日志 — [了解更多](test-deliveries.md#access-test-deliveries)。
   * 仅对于电子邮件，请检查常见电子邮件客户端中的邮件内容渲染 — [了解更多](email-rendering.md)。