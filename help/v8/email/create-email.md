---
audience: end-user
title: 发送您的第一封电子邮件
description: 了解如何使用Campaign Web UI发送您的第一封电子邮件
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# 发送您的第一封电子邮件 {#first-email}

![](../assets/do-not-localize/badge.png)

了解如何创建您的第一封定向电子邮件。 在此用例中，您计划在特定日期向银牌和金牌忠诚会员发送电子邮件。

该电子邮件还基于预定义的设计模板，根据客户用户档案属性提供个性化内容。

![](assets/delivery-list.png)

## 创建电子邮件 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="选择电子邮件模板"
>abstract="电子邮件模板是特定的投放配置，其中包含预定义的设置，例如分类规则、个性化或路由参数。 模板在Campaign客户端控制台中定义。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="电子邮件属性"
>abstract="属性是常用的投放参数，可帮助您命名投放并对其进行分类。 如果您的投放基于在Adobe Campaign v8控制台中定义的扩展架构，则某些特定 **自定义选项** 字段。"

1. 要创建新投放，请转到 **[!UICONTROL 投放]** 菜单和选择 **[!UICONTROL 电子邮件]** 作为渠道。

1. 选择要使用的模板，然后单击 **[!UICONTROL 创建投放]**.

   >[!NOTE]
   >
   >模板是预配置的投放设置，可保存以供将来使用。 管理员用户可以在Adobe Campaign控制台中创建这些配置文件。 [了解如何使用投放模板](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. 为电子邮件提供标签，并根据您的需求配置其他选项：

   * **[!UICONTROL 内部名称]**:为投放分配唯一标识符，
   * **[!UICONTROL 文件夹]**:将投放存储在特定文件夹中，
   * **[!UICONTROL 提交代码]**:使用此字段根据您自己的命名约定组织投放，
   * **[!UICONTROL 描述]**:为投放指定描述，
   * **[!UICONTROL 自然]**:为分类目的指定电子邮件的性质。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >如果您已使用特定自定义字段扩展了架构，则可以在 **[!UICONTROL 自定义选项]** 中。

   ![](assets/email-properties.png)

   此外，通过单击投放名称旁边的按钮，还可以访问高级设置，如分类规则和目标映射。 这些设置在选定的模板中进行了预配置，但可以根据需要编辑此特定电子邮件。

## 创建电子邮件内容 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="了解如何设计电子邮件内容"
>abstract="了解如何使用Email Designer。"

在此用例中，您可以使用预定义的模板来设计我们的电子邮件。

有关如何配置电子邮件内容的详细说明，请参阅 [此部分](../content/edit-content.md).

1. 要开始创建电子邮件内容，请单击 **[!UICONTROL 编辑内容]** 按钮。

   这会为您提供一个专用界面，您可以在该界面中配置电子邮件内容并使用Email Designer进行设计。

   ![](assets/edit-content.png)

1. 输入电子邮件的主题行，然后使用表达式编辑器对其进行个性化。 [了解如何个性化您的内容](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. 要设计电子邮件的正文，请单击 **[!UICONTROL 编辑电子邮件正文]** 按钮。

   选择用于创建电子邮件内容的方法。 在本例中，使用预定义的设计模板。

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. 选择模板后，该模板会显示在Email Designer中，您可以在其中进行任何必要的编辑和添加个性化。

   例如，要将个性化添加到电子邮件标题，请选择组件块并单击 **[!UICONTROL 添加个性化]**.

   ![](assets/add-perso.png)

1. 对内容满意后，保存并关闭您的设计。 单击 **[!UICONTROL 保存]** ，以返回到电子邮件创建屏幕。

   ![](assets/save-content.png)

## 定义受众 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="定义受众"
>abstract="为您的营销消息选择最佳受众。 您可以选择已在Campaign v8实例中定义的现有受众，也可以从Adobe Experience Platform中选择，也可以使用规则生成器创建新受众。"

在此用例中，您会向现有受众发送电子邮件。 有关如何使用受众的其他说明，请参阅 [此部分](../audience/about-audiences.md).

1. 要选择电子邮件的受众，请单击 **[!UICONTROL 选择受众]** 按钮，然后从列表中选择现有受众。

   在此示例中，我们希望使用现有受众来定位属于银牌和金牌忠诚度积分级别的客户。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >列表中可用的受众源自您的Campaign v8实例，或者来自Adobe Experience Platform（如果已在您的实例中配置目标/源集成）。
   >
   >通过目标/源集成，您可以将Experience Platform区段发送到Adobe Campaign，并将Campaign投放和跟踪日志发送到Adobe Experience Platform。 [了解如何使用Campaign和Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. 选择受众后，您可以通过应用其他规则进一步优化目标。

   您还可以设置一个控制组来分析与未定向收件人相比电子邮件收件人的行为。 [了解如何与控制组合作](../audience/control-group.md)

   ![](assets/audience-selected.png)

## 计划发送 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="计划发送"
>abstract="定义发送的日期和确切时间。 通过为您的营销消息选择最合适的时间，您可以最大限度地提高打开率。"

要计划发送电子邮件，请单击 **[!UICONTROL 启用]** 并设置发送所需的日期和时间。

默认情况下， **[!UICONTROL 发送前确认]** 选项，要求您在计划的日期和时间发送电子邮件之前确认发送。 如果您希望在计划的日期和时间自动发送电子邮件，则可以禁用此选项。

![](assets/schedule.png)

## 预览和测试电子邮件 {#preview-test}

在发送电子邮件之前，您可以预览并测试该电子邮件，以确保其符合您的预期。

在此用例中，您可以预览电子邮件，并将测试版本发送到特定的电子邮件地址，同时模拟某些目标用户档案。

有关如何预览和测试电子邮件的其他信息，请参阅 [此部分](../preview-test/preview-test.md).

1. 要查看和发送电子邮件，请单击 **[!UICONTROL 审阅并发送]**. 此时会显示电子邮件的预览，以及所有已配置的属性、受众和计划。 您可以通过单击修改按钮来编辑其中的任何元素。

1. 要预览电子邮件并发送测试版本，请单击 **[!UICONTROL 模拟内容]** 按钮。

   ![](assets/review-email.png)

1. 在左侧，选择要用于预览电子邮件的用户档案。

   右侧窗格显示基于所选用户档案的电子邮件预览。 如果已添加多个用户档案，则可以在它们之间切换以预览相应的电子邮件。

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. 要发送电子邮件的测试版本，请单击 **[!UICONTROL 测试]** 按钮，然后选择要使用的模式。

   在本例中，使用 **[!UICONTROL 从主目标替换]** 模式，在模拟电子邮件所定向的某些用户档案时，将测试版本发送到特定电子邮件地址。

   ![](assets/proof-mode.png)

1. 单击 **[!UICONTROL 添加地址]** 和指定接收测试版本的电子邮件地址。

   对于每个电子邮件地址，选择要模拟的用户档案。 您还可以让Adobe Campaign从目标中选择一个随机配置文件。

   ![](assets/proof-test-profile.png)

1. 单击 **[!UICONTROL 发送测试电子邮件]** 确认发送。

   测试版本将使用包含 **[校样x]** 前缀。

   ![](assets/proof-sent.png)

   您可以随时检查发送状态，并通过单击 **[!UICONTROL 查看测试电子邮件日志]** 按钮。

## 发送并监视电子邮件 {#prepare-send}

审核和测试电子邮件后，您可以启动准备并发送它。

1. 要开始准备电子邮件，请单击 **[!UICONTROL 准备]**. [了解如何准备电子邮件](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. 准备好发送电子邮件后，单击 **[!UICONTROL 发送]** 按钮（或） **[!UICONTROL 按计划发送]** （如果已计划其发送）并确认发送。

1. 在发送过程中，您可以直接在此屏幕中跟踪其进度并实时查看统计信息。

   ![](assets/sent-mail.png)

   您还可以通过单击 **[!UICONTROL 日志]** 按钮。 [了解如何监控投放日志](../monitor/delivery-logs.md)

1. 发送电子邮件后，您可以通过单击 **[!UICONTROL 报表]** 按钮。

![](assets/reports.png)
