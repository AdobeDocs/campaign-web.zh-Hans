---
audience: end-user
title: 预览电子邮件内容
description: 了解如何使用 Campaign Web UI 预览电子邮件内容
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha" type="Positive"
source-git-commit: acc6cdd89b78a26f7c2435e19fba148a71e4f18f
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 28%

---


# 预览电子邮件内容 {#preview-content}

使用 [!DNL Campaign] 内容模拟功能，可在发送电子邮件之前预览其内容。 这允许您控制个性化并检查向收件人显示的方式。

要预览电子邮件的内容，请执行以下步骤。

1. 浏览到电子邮件 [编辑内容](../content/edit-content.md) 屏幕或 [电子邮件设计工具](../content/get-started-email-designer.md).

1. 单击 **[!UICONTROL 模拟内容]** 按钮。

   ![](assets/simulate-button.png)

1. 使用 **[!UICONTROL 添加测试配置文件]** 按钮选择将用于预览个性化内容的用户档案。

1. 可以组合测试配置文件和配置文件以预览电子邮件。

   * **[!UICONTROL 测试配置文件]**&#x200B;选项卡将列出所有种子地址，这些地址是数据库中的额外和虚构的收件人。

     >[!NOTE]
     >
     >可在中创建测试用户档案 [!DNL Campaign] 控制台进入 **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子地址]** 文件夹。 了解详情，请参阅 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * **[!UICONTROL 配置文件]**&#x200B;选项卡列出了存储到 控制台的&#x200B;**[!UICONTROL 配置文件和目标]**&#x200B;文件夹中的所有收件人。[!DNL Campaign][了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. 单击 **[!UICONTROL 选择]** 以确认在两个选项卡中的选择。

   电子邮件的预览显示在的右侧窗格中 **[!UICONTROL 模拟]** 屏幕。 个性化元素被替换为在左窗格中选择的配置文件中的数据。

   ![](assets/simulate-preview.png)

1. 如果已添加多个配置文件，则可以在列表中切换它们以预览相应的电子邮件内容。您还可以添加更多测试用户档案，并使用左窗格上的相应按钮清除您的选择。

1. 您可以调整 **[!UICONTROL 缩放级别]** 并使用右上角的专用图标在桌面或移动设备上预览内容。

1. 从 **[!UICONTROL 模拟]** 屏幕您还可以：
   * 检查常用电子邮件客户端中的电子邮件渲染 —  [了解详情](email-rendering.md)
   * 向特定收件人发送测试电子邮件以进行验证 —  [了解详情](proofs.md)



