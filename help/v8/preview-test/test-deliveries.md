---
audience: end-user
title: 发送测试投放
description: 了解如何定义和发送测试投放
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Beta"
source-git-commit: c7be20a41d3188f67225a60a5559ed3166cd3ca4
workflow-type: tm+mt
source-wordcount: '1145'
ht-degree: 11%

---

# 发送测试投放 {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="预览模式"
>abstract="通过将测试群体包括在主目标中而预览和测试消息。"

定义消息内容后，您可以通过发送测试投放（也称为）来预览和测试该内容。 “验证”)。 如果插入个性化内容，则可以使用测试用户档案数据检查此内容在消息中的显示方式。

要检测消息内容或个性化设置中可能出现的错误，请先将测试消息发送到测试用户档案，然后再将其发送给目标受众。 每次进行更改时都应发送测试消息，以验证最新内容。 发送测试投放（以前称为“验证”）是验证营销活动和识别潜在问题的重要步骤。 测试消息的收件人可以检查各种元素，例如链接、选择退出链接、图像或镜像页面，并检测渲染、内容、个性化设置和投放配置中的任何错误。

## 选择测试收件人 {#test-recipients}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="测试群体"
>abstract="选择测试群体模式。"

根据您使用的渠道，可以将测试消息发送到三种类型的收件人：

* [测试用户档案](#test-profiles)  — 发送 **测试电子邮件和短信** 种子地址，即数据库中的其他收件人。 它们可以在以下位置创建： [!DNL Campaign] 控制台进入 **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子地址]** 文件夹。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* [从主要目标替换](#substitution-profiles)  — 发送 **测试电子邮件和短信** 到特定电子邮件地址或电话号码。 这样，您就可以像收件人一样体验消息，从而准确地表示用户档案将收到的内容。

* [订阅者](#subscribers)  — 发送 **测试推送通知** 添加到数据库的虚拟订阅者。 与测试用户档案一样，也可以在以下位置创建测试用户档案： [!DNL Campaign] 控制台进入 **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子地址]** 文件夹。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

要选择测试投放的收件人，请根据要使用的用户档案类型执行以下步骤。

### 测试用户档案 {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="验证目标"
>abstract="如果要在发送到主要目标之前测试投放，可再上传一个文件作为“验证目标”。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="上传配置文件"
>abstract="如果要用与您用于主要目标的集合不同的集合测试投放，可再上传一个文件，其中包含其他配置文件。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="模板文件"
>abstract="文件的格式必须与原始文件相同。<br/>支持的文件格式：txt、csv。最大文件大小：15 MB。使用第一行作为列标题。"


测试用户档案是种子地址，是数据库中的其他收件人。 它们可以在以下位置创建： [!DNL Adobe Campaign] 将客户端控制台移入 **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子地址]** 文件夹。 将测试消息发送到种子地址的步骤详述如下。

1. 浏览到电子邮件或短信投放的编辑内容屏幕，然后单击 **[!UICONTROL 模拟内容]** 按钮。

1. 单击 **[!UICONTROL 测试]** 按钮。

   >[!NOTE]
   >
   >如果您已经选择用户档案到 [预览投放](preview-content.md)，它们会列在左窗格中。

   ![](assets/simulate-test-button-email.png)

1. 从 **[!UICONTROL 模式]** 下拉列表，选择 **[!UICONTROL 测试用户档案]** 定位将接收测试电子邮件或短信投放的虚构收件人。

   ![](assets/simulate-profile-mode.png)

1. 如果您已经选择用户档案到 [预览消息](preview-content.md) 在内容模拟屏幕中，会预选这些用户档案作为测试收件人。 您可以清除所做的选择和/或使用 **[!UICONTROL 添加测试配置文件]** 按钮。

   >[!NOTE]
   >
   >默认情况下， **[!UICONTROL 使用测试用户档案]** 模式处于选中状态。

1. 要将最终消息发送给测试投放的收件人，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

1. 选择测试用户档案后，您可以 [发送测试投放](#send-test).

### 替换配置文件 {#substitution-profiles}

要在显示来自的某个现有配置文件的数据时向特定的电子邮件地址或电话号码发送测试电子邮件或短信，请执行以下操作 [!DNL Adobe Campaign] 数据库，使用替换配置文件，如下所述：

1. 在发送测试之前，请确保为投放定义目标受众。 [了解详情](../audience/about-recipients.md)

1. 浏览到电子邮件或短信投放的编辑内容屏幕，然后单击 **[!UICONTROL 模拟内容]** 按钮。

1. 单击 **[!UICONTROL 测试]** 按钮。

   ![](assets/simulate-test-button-email.png)

1. 从 **[!UICONTROL 模式]** 下拉列表，选择 **[!UICONTROL 从主要目标替换]** 在显示现有配置文件的数据时，将测试发送到特定的电子邮件地址或电话号码。

   >[!CAUTION]
   >
   >如果您尚未选择 [受众](../audience/about-recipients.md) 对于您的投放， **[!UICONTROL 从主要目标替换]** 选项将灰显，您将无法选择替换配置文件。

1. 单击 **[!UICONTROL 添加地址]** 按钮，并指定要接收测试投放的电子邮件地址或电话号码。

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >您可以输入任何电子邮件地址或电话号码。 这样，您可以将测试投放发送给任何收件人，即使他们不是的用户 [!DNL Adobe Campaign].

1. 从为投放定义的目标中选择要用作替换的用户档案。 您还可以让 [!DNL Adobe Campaign] 从目标中选择一个随机配置文件。 来自所选用户档案的用户档案数据将显示在测试投放中。

1. 确认收件人并重复该操作，根据需要添加任意数量的电子邮件地址或电话号码。

   ![](assets/simulate-profile-substitute.png)

1. 要将最终消息发送给测试投放的收件人，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

1. 选择替代配置文件后，您可以 [发送测试投放](#send-test).

### 订阅者 {#subscribers}

使用推送通知时，测试投放只能发送给应用程序订阅者。 要选择它们，请执行以下步骤。

1. 浏览到投放的编辑内容屏幕，然后单击 **[!UICONTROL 模拟内容]** 按钮。

1. 单击 **[!UICONTROL 测试]** 按钮。

   ![](assets/simulate-test-button-push.png)

1. 如果您已选择订阅者 [预览投放](preview-content.md) 在内容模拟屏幕中，预先选择这些用户档案作为测试订阅者。

   您可以使用专用按钮清除选择和/或添加其他订阅者。

   ![](assets/simulate-test-subscribers.png)

1. 要同时向测试订阅者发送最终推送通知，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

1. 选择订阅者后，您可以 [发送测试投放](#send-test).

## 发送测试投放 {#send-test}

要将测试投放发送给选定的收件人，请执行以下步骤。

1. 单击 **[!UICONTROL 发送测试]** 按钮。

1. 确认发送。

   ![](assets/simulate-send-test.png)

1. 发送所需数量的测试，直到最终确定投放内容为止。

完成后，您可以准备投放并将其发送到主目标。 请在以下专用部分中了解具体操作步骤：

* [发送电子邮件](../monitor/prepare-send.md)
* [发送推送通知](../push/send-push.md#send-push)
* [发送短信投放](../sms/send-sms.md#send-sms)

## 访问已发送的测试投放 {#access-proofs}

发送测试投放后，您可以从 **[!UICONTROL 查看测试日志]** 按钮。

利用这些日志，可访问为选定投放发送的所有测试，并可视化与其发送相关的特定统计信息。 [了解如何监控投放日志](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

您还可以从访问已发送的测试 [投放列表](../msg/gs-messages.md)，与任何投放一样。

![](assets/simulate-deliveries-list.png)
