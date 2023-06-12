---
audience: end-user
title: 发送测试电子邮件
description: 了解如何定义和发送测试电子邮件
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positive"
source-git-commit: acc6cdd89b78a26f7c2435e19fba148a71e4f18f
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 40%

---

# 发送测试电子邮件 {#send-test-emails}

**[!UICONTROL Adobe Campaign]** 用于在将消息发送到主受众之前对其进行测试。

发送测试电子邮件是一个用于验证电子邮件营销活动和识别潜在问题的重要步骤。

测试的收件人可以检查各种元素，如链接、选择退出链接、图像和镜像页面，并检测渲染、内容、个性化设置和电子邮件配置中的任何错误。

## 选择测试收件人 {#test-recipients}

可以将测试电子邮件发送给两类收件人：

* **测试用户档案**  — 向种子地址发送测试电子邮件，这些地址是数据库中的其他虚构收件人。 它们可以在以下位置创建： [!DNL Campaign] 控制台进入 **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子地址]** 文件夹。 了解详情，请参阅 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* **从主要目标替换**  — 模拟现有用户档案时将测试电子邮件发送到特定电子邮件地址。 这使您能够像收件人那样体验电子邮件，从而准确表示配置文件将收到的邮件。

要选择电子邮件测试的收件人，请执行以下步骤。

1. 访问电子邮件 [编辑内容](../content/edit-content.md) 屏幕或 [电子邮件设计工具](../content/get-started-email-designer.md)，然后单击 **[!UICONTROL 模拟内容]** 按钮。

1. 单击 **[!UICONTROL 测试]** 按钮。

   ![](assets/simulate-test-button.png)

1. 使用&#x200B;**[!UICONTROL 模式]**&#x200B;下拉列表来选择接收测试电子邮件的收件人的类型：

   * **测试用户档案** 定位虚构的收件人

   * **从主要目标替换** 在显示现有用户档案中的数据时将测试发送到特定电子邮件地址。

   ![](assets/simulate-profile-mode.png)

   >[!NOTE]
   >
   >默认情况下， **[!UICONTROL 使用测试用户档案]** 模式处于选中状态。 如果您已选择配置文件来在内容模拟屏幕中预览电子邮件，则会将这些配置文件预选定为测试收件人。您可以清除选定内容和/或添加其他收件人。

1. 要将测试电子邮件发送到替换用户档案，请选择 **[!UICONTROL 从目标替换]** 模式，然后按照以下步骤操作：

   1. 单击&#x200B;**[!UICONTROL 添加地址]**&#x200B;按钮，并指定接收测试电子邮件的电子邮件地址。

      您可以输入任意电子邮件地址。这允许您向任何用户发送测试电子邮件，即使他们不是的用户 [!DNL Adobe Campaign].

   1. 从目标中选择要用作替换的配置文件。 您还可以让 [!DNL Adobe Campaign] 从目标中选择一个随机配置文件。 所选用户档案中的用户档案数据将显示在测试电子邮件中。

   1. 确认收件人并重复该操作以添加所需数量的地址。

      ![](assets/simulate-profile-substitute.png)

1. 选择测试收件人后，您可以 [发送测试电子邮件](#send-test).

   >[!NOTE]
   >
   >要同时向测试电子邮件的收件人发送最终电子邮件，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

## 发送测试电子邮件 {#send-test}

要将测试电子邮件发送给选定的收件人，请执行以下步骤。

1. 单击 **[!UICONTROL 发送测试电子邮件]**.

1. 确认发送。

   ![](assets/simulate-send-test.png)

1. 发送所需数量的测试电子邮件，直到您最终确定投放内容。

完成此操作后，您可以 [准备并发送电子邮件](../monitor/prepare-send.md) 到主目标。

## 访问已发送的测试电子邮件 {#access-proofs}

在发送测试电子邮件后，可以使用&#x200B;**[!UICONTROL 查看测试电子邮件日志]**&#x200B;按钮访问专用日志。

这些日志可让您访问为所选投放发送的所有测试电子邮件，并可视化与其发送相关的特定统计数据。[了解如何监控投放日志](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

您还可以从访问已发送测试电子邮件 [投放列表](../msg/gs-messages.md)，与任何投放一样。

![](assets/simulate-deliveries-list.png)
