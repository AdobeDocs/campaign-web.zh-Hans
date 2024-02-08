---
audience: end-user
title: 预览投放内容
description: 了解如何使用Campaign Web用户界面预览投放内容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="有限发布版"
source-git-commit: 462725104d28a967dd8a072ef6064b74dad91c58
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 1%

---


# 预览消息内容 {#preview-content}

使用 [!DNL Campaign] 内容模拟功能，可在发送消息之前预览消息内容。 这允许您控制个性化并检查向收件人显示的方式。

要预览投放内容，请执行以下步骤。

1. 浏览到投放的编辑内容屏幕或 [电子邮件设计工具](../email/get-started-email-designer.md).

1. 单击 **[!UICONTROL 模拟内容]** 按钮。

   ![](assets/simulate-button.png)

1. 要选择将用于预览个性化内容的配置文件，请使用：

   * **[!UICONTROL 添加测试配置文件]** 用于预览电子邮件和短信投放

   * **[!UICONTROL 添加订阅者]** 用于预览推送通知

1. 您可以组合用户档案和测试用户档案，以预览电子邮件或短信消息。

   * 此 **[!UICONTROL 测试用户档案]** 选项卡列出了所有测试用户档案，它们是数据库中的其他虚构收件人。 [了解如何使用测试用户档案](../audience/test-profiles.md)

   * 此 **[!UICONTROL 配置文件]** 选项卡列出了数据库中存储的所有用户档案。 [了解如何使用用户档案](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png)

1. 在浏览测试用户档案或用户档案列表时，您可以使用过滤器来优化搜索。

   ![](assets/simulate-test-profile-filter.png)

   例如，您可以定义规则以查找所有测试用户档案，其中 **[!UICONTROL 潜在客户]** 状态。 [了解如何使用查询建模器添加规则](../query/query-modeler-overview.md).

1. 单击 **[!UICONTROL 选择]** 以确认您的选择。

   投放内容的预览显示在的右侧窗格中 **[!UICONTROL 模拟]** 屏幕。 个性化元素被替换为在左窗格中选择的配置文件中的数据。

   ![](assets/simulate-preview.png)

1. 如果您添加了多个用户档案，则可以在列表中的这些用户档案之间切换以预览相应的投放内容。 您还可以添加更多测试用户档案，并使用左窗格上的相应按钮清除您的选择。

1. 对于电子邮件投放，您可以调整 **[!UICONTROL 缩放级别]** 并使用右上角的专用图标在桌面或移动设备上预览内容。

1. 从 **[!UICONTROL 模拟]** 屏幕您还可以：
   * 将测试投放发送给特定收件人进行验证 —  [了解详情](test-deliveries.md)
   * 访问已发送测试投放的日志 —  [了解详情](test-deliveries.md#access-test-deliveries)
   * 仅对于电子邮件，检查常用电子邮件客户端中的消息内容呈现 —  [了解详情](email-rendering.md)



