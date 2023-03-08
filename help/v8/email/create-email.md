---
audience: end-user
title: 发送您的第一封电子邮件
description: 了解如何使用Campaign Web UI发送您的第一封电子邮件
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 773d15912aba9804cbd1ad681f7c02a7433ffa66
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# 发送您的第一封电子邮件 {#first-email}

![](../assets/do-not-localize/badge.png)

了解如何创建您的第一个定向电子邮件。 在此使用案例中，您安排在特定日期向银牌和金牌会员发送电子邮件。

基于预定义的设计模板，电子邮件还根据客户配置文件属性提供个性化内容。

![](assets/delivery-list.png)

## 创建电子邮件 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="选择电子邮件模板"
>abstract="电子邮件模板是特定的投放配置，其中包含预定义设置，例如类型规则、个性化或路由参数。 模板是在Campaign客户端控制台中定义的。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="电子邮件属性"
>abstract="属性是常见的投放参数，可帮助您对投放进行命名和分类。 如果您的投放基于Adobe Campaign v8控制台中定义的扩展架构，则某些特定的 **自定义选项** 字段可用。"

1. 要创建新投放，请浏览到 **[!UICONTROL 投放]** 菜单，然后单击  **[!UICONTROL 创建投放]** 按钮。

1. 选择 **[!UICONTROL 电子邮件]** 作为渠道并选择模板。

   >[!NOTE]
   >
   >模板是保存以供将来使用的预配置投放设置。 管理员用户可以在Adobe Campaign控制台中创建它们。 [了解如何使用投放模板](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. 单击 **[!UICONTROL 创建投放]** 按钮进行确认。
1. 输入投放标签，并根据需要配置其他选项：

   * **[!UICONTROL 内部名称]**：为投放分配唯一标识符，
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中，
   * **[!UICONTROL 投放代码]**：使用此字段可根据您自己的命名惯例组织投放，
   * **[!UICONTROL 描述]**：指定投放的描述，
   * **[!UICONTROL 自然]**：指定电子邮件的性质以进行分类。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >如果您已使用特定自定义字段扩展了架构，则可以在以下位置访问它们： **[!UICONTROL 自定义选项]** 部分。

   ![](assets/email-properties.png)

   此外，通过单击位于投放名称旁边的按钮，还可以访问高级设置，例如类型规则和目标映射。 这些设置在所选模板中进行了预配置，但可以根据需要对此特定电子邮件进行编辑。

## 创建电子邮件内容 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="了解如何设计电子邮件内容"
>abstract="了解如何使用电子邮件设计器。"

有关如何配置电子邮件内容的详细说明，请参阅 [本节](../content/edit-content.md).

在此使用案例中，您使用预定义模板来设计电子邮件。

1. 要开始创建电子邮件内容，请打开您的电子邮件投放并单击 **[!UICONTROL 编辑内容]** 按钮。

   这会将您带到专用界面，您可以在其中配置电子邮件内容并使用Email Designer进行设计。

   ![](assets/edit-content.png)

1. 输入电子邮件的主题行，然后使用表达式编辑器对其进行个性化设置。 [了解如何个性化您的内容](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. 要设计电子邮件的内容，请单击 **[!UICONTROL 编辑电子邮件正文]** 按钮。

   选择用于创建电子邮件内容的方法。 在此示例中，使用预定义的设计模板。

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. 选择模板后，该模板将显示在Email Designer中，您可以在其中进行任何必要的编辑并添加个性化。

   例如，要将个性化添加到电子邮件标题，请选择组件块并单击 **[!UICONTROL 添加个性化]**.

   ![](assets/add-perso.png)

1. 对内容满意后，保存并关闭设计。 单击 **[!UICONTROL 保存]** 以返回到电子邮件创建屏幕。

   ![](assets/save-content.png)

## 定义受众 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="定义受众"
>abstract="为您的营销消息选择最佳受众。 您可以选择已在Campaign v8实例中定义的现有受众，也可以从Adobe Experience Platform中选择现有受众，也可以使用规则生成器创建新受众。"

在此使用案例中，您将向现有受众发送电子邮件。 有关如何使用受众的其他说明，请参见 [本节](../audience/about-audiences.md).

1. 要选择电子邮件的受众，请单击 **[!UICONTROL 选择受众]** 按钮并从列表中选择现有受众。

   在本例中，我们希望使用现有受众，确定属于银级和金级忠诚度积分的客户为目标。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >列表中可用的受众源自您的Campaign v8实例，或者如果您已在实例上配置了目标/源集成，则来自Adobe Experience Platform。
   >
   >目标/源集成允许您将Experience Platform区段发送到Adobe Campaign，并将Campaign投放和跟踪日志发送到Adobe Experience Platform。 [了解如何使用Campaign和Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. 选择受众后，您可以通过应用其他规则来进一步优化目标。

   您还可以设置控制组来分析电子邮件收件人与未定向收件人的行为。 [了解如何使用控制组](../audience/control-group.md)

   ![](assets/audience-selected.png)

## 计划发送 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="计划发送"
>abstract="定义发送日期和确切时间。 通过为营销消息选择最合适的时间，您可以最大限度地提高打开率。"

要计划电子邮件的发送，请打开您的电子邮件投放并浏览到 **计划** 部分。 使用 **[!UICONTROL 启用计划]** 切换以激活它，并设置所需的发送日期和时间。 发送投放后，实际发送将从您定义的联系日期开始。

默认情况下， **[!UICONTROL 发送前启用确认]** 选项。 此选项要求您在计划的日期和时间发送电子邮件之前确认发送。 如果您需要在计划的日期和时间自动发送电子邮件，则可以禁用此选项。

![](assets/schedule.png)

## 预览和测试电子邮件 {#preview-test}

在发送电子邮件之前，您可以预览和测试它以确保它符合您的预期。

在此使用案例中，您可以在模拟某些目标用户档案时预览电子邮件并将测试版本发送到特定电子邮件地址。

有关如何预览和测试电子邮件的其他信息，请参阅 [本节](../preview-test/preview-test.md).

1. 要查看您的电子邮件，请单击 **[!UICONTROL 查看并发送]**. 这会显示电子邮件的预览，以及所有配置的属性、受众和计划。 您可以通过单击“修改”按钮来编辑这些元素中的任意元素。

1. 要预览电子邮件并发送测试版本，请单击 **[!UICONTROL 模拟内容]** 按钮。

   ![](assets/review-email.png)

1. 在左侧，选择要用于预览电子邮件的用户档案。

   右侧窗格根据选定的用户档案显示电子邮件的预览。 如果添加了多个用户档案，则可以在它们之间切换以预览相应的电子邮件。

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. 要发送电子邮件的测试版本，请单击 **[!UICONTROL 测试]** 按钮，然后选择要使用的模式。

   在此示例中，使用 **[!UICONTROL 从主要目标替换]** 模式，将测试版本发送到特定的电子邮件地址，同时模拟电子邮件定向的某些用户档案。

   ![](assets/proof-mode.png)

1. 单击 **[!UICONTROL 添加地址]** 和指定接收测试版本的电子邮件地址。

   对于每个电子邮件地址，选择要模拟的用户档案。 您还可以让Adobe Campaign从目标中选择一个随机配置文件。

   ![](assets/proof-test-profile.png)

1. 单击 **[!UICONTROL 发送测试电子邮件]** 并确认发送。

   使用选定的配置文件将测试版本发送到指定的电子邮件地址，并具有 **[校对x]** 前缀。

   ![](assets/proof-sent.png)

   您可以检查发送的状态，并随时通过单击 **[!UICONTROL 查看测试电子邮件日志]** 按钮。

## 发送和监控电子邮件 {#prepare-send}

查看和测试您的电子邮件后，您可以启动其准备并发送它。

1. 要启动电子邮件的准备工作，请单击 **[!UICONTROL 准备]**. [了解如何准备电子邮件](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. 准备好发送电子邮件后，单击 **[!UICONTROL 发送]** 按钮(或 **[!UICONTROL 按计划发送]** （如果您已计划发送该邮件）并确认发送。

1. 在发送过程中，您可以直接在此屏幕中跟踪其进度并实时查看统计信息。

   ![](assets/sent-mail.png)

   您还可以通过单击 **[!UICONTROL 日志]** 按钮。 [了解如何监测投放日志](../monitor/delivery-logs.md)

1. 发送电子邮件后，您可以通过单击 **[!UICONTROL 报告]** 按钮。

![](assets/reports.png)
