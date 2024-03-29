---
audience: end-user
title: 发送校样
description: 了解如何定义和发送验证
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 15%

---

# 发送校样 {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="预览模式"
>abstract="通过将测试群体包括在主目标中而预览和测试消息。"

定义消息内容后，您可以通过向测试用户档案发送校样来预览和测试该内容。 如果插入个性化内容，则可以使用测试用户档案数据检查此内容在消息中的显示方式。

要检测消息内容或个性化设置中可能出现的错误，请先向测试用户档案发送校样，然后再将其发送给目标受众。 每次进行更改时都应发送校样，以验证最新内容。 发送校样是验证营销活动和识别潜在问题的重要步骤。 校样收件人可以检查各种元素，如链接、选择退出链接、图像或镜像页面，并检测渲染、内容、个性化设置和投放配置中的任何错误。

## 使用测试用户档案模拟内容 {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="测试群体"
>abstract="选择测试群体模式。"

在发送验证之前，请确保为投放定义目标受众。 [了解详情](../audience/add-audience.md)

要开始测试消息内容，请执行以下操作：

1. 编辑投放的内容。
1. 单击 **[!UICONTROL 模拟内容]** 按钮。
1. 单击 **[!UICONTROL 发送验证]** 按钮以发送校样。

   ![](assets/simulate-test-button-email.png){zoomable=&quot;yes&quot;}

1. 选择校样收件人。

   根据消息渠道，校样可以发送给以下类型的收件人：

   * 对于短信和电子邮件，您可以使用 [测试用户档案](#test-profiles)，即数据库中的其他特定收件人。 您也可以使用 [从主目标替换](#substitution-profiles) 模式，用于将验证发送到电子邮件测试地址或电话号码，并使用现有配置文件的个性化数据。 这样，您就可以像收件人一样体验消息，从而准确地表示用户档案将收到的内容。

   * 对于推送消息，您可以使用 [订阅者](#subscribers)，这些是添加到数据库中的虚拟订阅者。 它们创建于 [!DNL Campaign] 控制台。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   下面提供了每种模式的详细配置。

## 使用测试配置文件 {#test-profiles}

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

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="将测试配置文件包含在主要受众中"
>abstract="启用此选项还可将最终消息发送给验证收件人。"

测试用户档案是数据库中的其他收件人。 它们是从 **[!UICONTROL 客户管理]** > **[!UICONTROL 配置文件]** 菜单。 [了解详情](../audience/test-profiles.md#create-test-profiles)

将验证发送到测试用户档案的步骤详述如下。

1. 从投放内容中，单击 **[!UICONTROL 模拟内容]** 按钮，以及 **[!UICONTROL 发送验证]** 按钮。

1. 从 **[!UICONTROL 模式]** 下拉列表，选择 **[!UICONTROL 测试用户档案]** 定位将接收验证或短信投放的虚构收件人。

   ![](assets/simulate-profile-mode.png){zoomable=&quot;yes&quot;}

1. 如果您已经选择用户档案到 [预览消息](preview-content.md) 在内容模拟屏幕中，预先选择这些用户档案作为验证收件人。 您可以清除所做的选择和/或使用 **[!UICONTROL 添加测试配置文件]** 按钮。

1. 在浏览测试用户档案或用户档案列表时，您可以使用过滤器来优化搜索。 例如，您可以定义规则以查找所有测试用户档案，其中 **[!UICONTROL 潜在客户]** 状态。 了解如何使用 [查询建模器](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. 要将最终消息发送给验证的收件人，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

   ![](assets/simulate-include-test.png){zoomable=&quot;yes&quot;}

1. 选择测试用户档案后，您可以 [发送证明](#send-test).

## 替换用户档案数据 {#substitution-profiles}

使用配置文件替换将验证发送到特定的电子邮件地址或电话号码，同时显示来自的现有配置文件的数据 [!DNL Adobe Campaign] 数据库。 仅当已定义投放的受众时，才能选择此模式。

要替换主目标中的用户档案数据，请执行以下步骤：

1. 从投放内容中，单击 **[!UICONTROL 模拟内容]** 按钮，以及 **[!UICONTROL 发送验证]** 按钮。

1. 从 **[!UICONTROL 模式]** 下拉列表，选择 **[!UICONTROL 从主要目标替换]** 在显示现有用户档案中的数据时将验证发送到特定电子邮件地址或电话号码。

   >[!CAUTION]
   >
   >如果您尚未选择 [受众](../audience/about-recipients.md) 对于您的投放， **[!UICONTROL 从主要目标替换]** 选项将灰显，您将无法选择替换配置文件。

1. 单击 **[!UICONTROL 添加地址]** 按钮并指定将接收验证的电子邮件地址或电话号码。

   ![](assets/simulate-add-substitution-address.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >您可以输入任何电子邮件地址或电话号码。 这允许您向任何收件人发送验证，即使他们不是的用户 [!DNL Adobe Campaign].

1. 从为投放定义的目标中选择要用作替换的用户档案。 您还可以让 [!DNL Adobe Campaign] 从目标中选择一个随机配置文件。 所选用户档案中的用户档案数据将显示在验证中。

1. 确认收件人并重复该操作，根据需要添加任意数量的电子邮件地址或电话号码。

   ![](assets/simulate-profile-substitute.png){zoomable=&quot;yes&quot;}

1. 要将最终消息发送给验证的收件人，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

1. 选择替代配置文件后，您可以 [发送证明](#send-test).

## 向应用程序订阅者发送验证 {#subscribers}

在设计推送通知时，只能将验证发送给应用程序订阅者。 要选择它们，请执行以下步骤。

1. 在推送投放的内容中，单击 **[!UICONTROL 模拟内容]** 按钮，以及 **[!UICONTROL 发送验证]** 按钮。

   ![](assets/simulate-test-button-push.png){zoomable=&quot;yes&quot;}

1. 如果您已选择订阅者 [预览投放](preview-content.md) 在内容模拟屏幕中，预先选择这些用户档案作为测试订阅者。

   您可以使用专用按钮清除选择和/或添加其他订阅者。

   ![](assets/simulate-test-subscribers.png){zoomable=&quot;yes&quot;}

1. 要同时向测试订阅者发送最终推送通知，请选择 **[!UICONTROL 在主要目标中包含测试群体]** 选项。

1. 选择订阅者后，您可以 [发送证明](#send-test).

## 发送证明 {#send-test}

要将校样发送给选定的收件人，请执行以下步骤。

1. 单击 **[!UICONTROL 发送验证]** 按钮。

1. 确认发送。

   ![](assets/simulate-send-test.png){zoomable=&quot;yes&quot;}

1. 发送所需数量的校样，直到完成投放内容为止。

完成后，您可以准备投放并将其发送到主目标。 请在以下专用部分中了解具体操作步骤：

* [发送电子邮件](../monitor/prepare-send.md)
* [发送推送通知](../push/send-push.md#send-push)
* [发送短信投放](../sms/send-sms.md#send-sms)

## 访问已发送的校样 {#access-test-deliveries}

发送校样后，您可以从访问其日志 **[!UICONTROL 模拟内容]** 屏幕。

利用这些日志，可访问为所选投放发送的所有验证，并可视化与其发送相关的特定统计信息。 [了解如何监控投放日志](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable=&quot;yes&quot;}

您还可以从以下位置访问已发送的校样 [投放列表](../msg/gs-messages.md)，与任何投放一样。

![](assets/simulate-deliveries-list.png){zoomable=&quot;yes&quot;}
