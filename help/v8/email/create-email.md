---
audience: end-user
title: 发送您的第一封电子邮件
description: 了解如何使用Campaign Web用户界面发送您的第一封电子邮件
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '1403'
ht-degree: 66%

---


# 创建您的第一封电子邮件 {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="开始使用电子邮件"
>abstract="可创建独立的电子邮件投放或在营销活动工作流程的环境下创建电子邮件。了解如何创建投放、选择受众和设计电子邮件内容。"


<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="开始使用电子邮件"
>abstract="可创建独立的电子邮件投放或在营销活动工作流程的环境下创建电子邮件。了解如何创建投放、选择受众和设计电子邮件内容。"

<!--TO REMOVE ABOVE-->



了解如何创建您的第一封定向电子邮件。在此用例中，您计划在特定日期向银牌和金牌忠诚度会员发送电子邮件。

基于预定义的 [设计模板](../email/create-email-templates.md)中，该电子邮件还根据客户配置文件属性提供了个性化内容。

## 创建电子邮件投放 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="选择电子邮件模板"
>abstract="电子邮件模板是一种特定的投放配置，其中包含预定义的设置，例如类型规则、个性化或路由参数。模板在 Campaign 客户端控制台中定义。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="定义电子邮件属性"
>abstract="这些属性是常见的投放参数，可帮助您为投放命名和分类。其他设置为可选。如果您的投放基于在 Adobe Campaign v8 控制台中定义的扩展架构，则有一些特定的&#x200B;**自定义选项**&#x200B;字段可用。"

可创建独立的电子邮件投放或在营销活动工作流程的环境下创建电子邮件。以下步骤详细介绍了独立（一次性）电子邮件投放的过程。 在中详细了解Adobe Campaign中的投放创建步骤 [此页面](../msg/gs-deliveries.md).

要创建新的独立电子邮件投放，请执行以下步骤。

1. 浏览至 **[!UICONTROL 投放]** 菜单，然后单击  **[!UICONTROL 创建投放]** 按钮。

   ![](../msg/assets/create-a-delivery.png)

1. 选择 **[!UICONTROL 电子邮件]** 作为渠道，并从列表中选择电子邮件投放模板。

   >[!NOTE]
   >
   >模板是已保存以供将来使用的预配置的投放设置。[了解详情](../msg/delivery-template.md)

   ![](assets/channel-template.png){zoomable=&quot;yes&quot;}

1. 单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮以进行确认。
1. 输入投放的标签并根据需要配置其他选项：

   * **[!UICONTROL 内部名称]**：为投放分配唯一标识符。
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中。
   * **[!UICONTROL 投放代码]**：使用此字段可根据您自己的命名惯例组织投放。
   * **[!UICONTROL 描述]**：指定投放描述。
   * **[!UICONTROL 性质]**：指定电子邮件的性质以进行分类。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >如果您已使用特定的自定义字段扩展架构，则可在&#x200B;**[!UICONTROL 自定义选项]**&#x200B;部分中访问它们。

   ![](assets/email-properties.png){zoomable=&quot;yes&quot;}

1. 此外，高级设置（如类型规则和目标映射）也可以通过 **[!UICONTROL 设置]** 按钮。 这些设置已在所选模板中预先配置，但可根据需要对此特定电子邮件进行编辑。 [了解详情](../advanced-settings/delivery-settings.md)

## 定义受众 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="为投放选择受众"
>abstract="选择最适合营销消息的最佳受众。可选择（已在 Campaign v8 实例中或从 Adobe Experience Platform 定义的）现有受众、使用查询建模器创建新受众或上传包含您的受众的文件。没有为&#x200B;**从文件选择**&#x200B;选项启用对照组，反之亦然。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=zh-Hans" text="选择主要受众"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=zh-Hans" text="设置对照组"

在此使用案例中，您将向现有受众发送电子邮件。

有关如何使用受众的其他说明，请参阅[此章节](../audience/about-recipients.md)。

1. 要选择电子邮件的受众，请单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮，并从列表中选择一个现有受众。

   在此示例中，我们希望使用定位属于银牌和金牌忠诚度积分等级的客户的现有受众。

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >列表中的可用受众源自您的Campaign v8实例，或者如果您已在实例上配置了目标/源集成，则来自Adobe Experience Platform。 利用此集成，可将Experience Platform区段发送到Adobe Campaign，并将Campaign投放和跟踪日志发送到Adobe Experience Platform。 了解如何在中使用Campaign和Adobe Experience Platform [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. 选择受众后，可以通过应用其他规则来进一步细化目标。

   ![](assets/audience-selected.png){zoomable=&quot;yes&quot;}

1. 您还可以设置一个对照组来分析比较电子邮件收件人的行为与非定向人员的行为。[了解如何使用对照组](../audience/control-group.md)

## 定义电子邮件的内容 {#create-content}

要开始创建电子邮件内容，请执行以下步骤。 在此使用案例中，您使用预定义的电子邮件 [投放模板](../msg/delivery-template.md) 设计电子邮件。<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. 在电子邮件投放仪表板中，单击 **[!UICONTROL 编辑内容]** 按钮。

   ![](assets/email-edit-content.png){zoomable=&quot;yes&quot;}

   这会将您带到专用界面，您可以在其中配置电子邮件内容并访问Email Designer。 [了解详情](edit-content.md)

   ![](assets/edit-content.png){zoomable=&quot;yes&quot;}

1. 输入电子邮件的主题行，并使用表达式编辑器对其进行个性化设置。[了解如何个性化您的内容](../personalization/personalize.md)

   ![](assets/subject-line.png){zoomable=&quot;yes&quot;}

1. 要设计电子邮件的内容，请单击&#x200B;**[!UICONTROL 编辑电子邮件正文]**&#x200B;按钮。

   选择要用于创建电子邮件内容的方法。在此示例中，使用 [预定义内容模板](create-email-templates.md).

   ![](assets/select-template.png){zoomable=&quot;yes&quot;}

1. 选择模板后，该模板将显示在 [电子邮件设计工具](create-email-content.md)，您可以在此处进行任何必要的编辑并添加个性化。

   例如，要向电子邮件标题添加个性化内容，请选择组件块并单击&#x200B;**[!UICONTROL 添加个性化内容]**。

   ![](assets/add-perso.png){zoomable=&quot;yes&quot;}

1. 在对内容感到满意后，请保存并关闭您的设计。单击&#x200B;**[!UICONTROL 保存]**&#x200B;返回电子邮件创建屏幕。

   ![](assets/save-content.png){zoomable=&quot;yes&quot;}

## 安排发送 {#schedule}

在工作流上下文中发送投放时，您必须使用 **计划程序** 活动。 了解详情，请参阅 [此页面](../workflows/activities/scheduler.md). 以下步骤仅适用于独立投放。

1. 浏览至 **[!UICONTROL 计划]** 投放属性的部分。

1. 使用 **[!UICONTROL 启用计划]** 切换以激活它。

1. 设置所需的发送日期和时间。

   ![](assets/schedule.png){zoomable=&quot;yes&quot;}

发送投放后，实际发送从您定义的联系日期开始。

在中了解有关投放计划的更多信息 [本节](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## 预览和测试电子邮件 {#preview-test}

在发送电子邮件之前，您可以预览和测试电子邮件以确保符合您的期望。

在此用例中，您可以预览电子邮件并将测试版本发送到特定的电子邮件地址，同时模拟一些定向配置文件。

有关如何预览和测试电子邮件的其他信息，请参阅[此章节](../preview-test/preview-test.md)。

1. 要查看您的电子邮件，请单击&#x200B;**[!UICONTROL 查看并发送]**。这将显示您的电子邮件预览，以及所有已配置的属性、受众和计划。可以通过单击修改按钮来编辑这些元素中的任一元素。

1. 要预览电子邮件并发送测试版本，请单击 **[!UICONTROL 模拟内容]** 按钮。

   ![](assets/review-email.png){zoomable=&quot;yes&quot;}

1. 在左侧，选择要用于预览电子邮件的配置文件。

   右侧窗格显示基于所选配置文件的电子邮件预览。如果已添加多个配置文件，则可以在它们之间进行切换来预览相应的电子邮件。

   ![](assets/preview.png){zoomable=&quot;yes&quot;}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. 要发送电子邮件的测试版本，请单击&#x200B;**[!UICONTROL 测试]**&#x200B;按钮，然后选择要使用的模式。

   在此示例中，使用&#x200B;**[!UICONTROL 从主要目标替代]**&#x200B;模式，它将测试版本发送到特定的电子邮件地址，同时模拟电子邮件所针对的一些配置文件。

   ![](assets/proof-mode.png){zoomable=&quot;yes&quot;}

1. 单击&#x200B;**[!UICONTROL 添加地址]**&#x200B;并指定接收测试版本的电子邮件地址。

   对于每个电子邮件地址，选择要模拟的配置文件。您还可以让 Adobe Campaign 从目标中选择一个随机配置文件。

   ![](assets/proof-test-profile.png){zoomable=&quot;yes&quot;}

1. 单击&#x200B;**[!UICONTROL 发送测试电子邮件]**&#x200B;并确认发送。

   使用选定的配置文件与 **[Proof x]** 前缀将测试版本发送到指定的电子邮件地址。

   ![](assets/proof-sent.png){zoomable=&quot;yes&quot;}

   可以随时单击模拟内容屏幕中的&#x200B;**[!UICONTROL 查看测试电子邮件日志]**&#x200B;按钮，来查看发送状态和访问已发送的测试电子邮件。

## 发送和监控电子邮件 {#prepare-send}

查看并测试您的电子邮件后，可以启动其准备工作并发送它。

1. 要启动电子邮件准备，请单击&#x200B;**[!UICONTROL 准备]**。[了解如何准备电子邮件](../monitor/prepare-send.md)

   ![](assets/preparation.png){zoomable=&quot;yes&quot;}

1. 准备好发送电子邮件后，单击&#x200B;**[!UICONTROL 发送]**&#x200B;按钮（如果您已计划发送，则单击&#x200B;**[!UICONTROL 按计划发送]**）并确认发送。

1. 在发送过程中，您可以直接在该屏幕中实时跟踪发送进度和查看统计数据。

   ![](assets/sending-email.png){zoomable=&quot;yes&quot;}

   <!--
    ![](assets/sent-email.png){zoomable="yes"}-->

   还可以单击&#x200B;**[!UICONTROL 日志]**&#x200B;按钮来访问有关发送的详细信息。[了解如何监控投放日志](../monitor/delivery-logs.md)

1. 发送电子邮件后，可以通过单击&#x200B;**[!UICONTROL 报告]**&#x200B;按钮来访问专用报告以进行深入分析。

![](assets/reports.png){zoomable=&quot;yes&quot;}
