---
audience: end-user
title: 创建您的第一封电子邮件
description: Campaign v8 Web文档
source-git-commit: cdddef89cda4fa39cee38e9d0171a6ea395537c7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 1%

---

# 发送您的第一封电子邮件 {#first-email}

>[!NOTE]
>
>此文档正在构建中并且经常更新。 此内容的最终版本将于2023年1月准备就绪。

此用例介绍如何创建您的第一封电子邮件

在本例中，我们将安排在特定日期向银牌和金牌忠诚客户发送电子邮件。 此电子邮件将使用ZIP文件中的预定义HTML模板进行设计，并将包含使用用户档案属性进行个性化的功能。

![](assets/delivery-list.png)

## 创建电子邮件 {#create-email}

1. 从 **[!UICONTROL 投放]** 菜单。
1. 选择 **[!UICONTROL 电子邮件]** 渠道和模板，然后单击 **[!UICONTROL 创建]**.

   >[!NOTE]
   >
   >模板信息。 在V7文档中查看信息

   ![](assets/channel-template.png)

1. 为投放提供标签，并根据需要配置其他选项：

   * 内部名称:
   * 文件夹:
   * 投放代码:
   * 说明:
   * 自然:

   检查模板中定义的设置并提及它们(描述？ 文件夹？，自然？)

   ![](assets/email-properties.png)

   >[!NOTE]
   >
   >“投放设置”按钮的信息+文档链接

## 创建电子邮件内容 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="使用Email Designer创建您的第一个电子邮件内容。"
>abstract="创建您的第一个电子邮件内容"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="创建电子邮件内容"
>abstract="热障涂层"

1. 单击 **[!UICONTROL 编辑内容]** 按钮以开始创建电子邮件的内容。

   利用此屏幕，可配置电子邮件内容并使用Email Designer进行设计。

   ![](assets/edit-content.png)

   >[!NOTE]
   >
   >在选定的电子邮件模板中，将预定义“发件人”名称和“发件人”电子邮件信息。
   >
   >默认情况下，会为打开数和点击数启用电子邮件跟踪。 要禁用这些选项，请从“可选功能”部分中取消选择它们。

1. 使用表达式编辑器指定电子邮件的主题。 [了解如何个性化您的内容](../personalization/personalize.md)

   在本例中，我们希望使用用户档案的名字个性化主题行。

   ![](assets/subject-line.png)

1. 根据需要，向电子邮件中添加附加文件。 了解如何编辑电子邮件内容

1. 单击 **[!UICONTROL 编辑电子邮件正文]** 按钮以创建和设计电子邮件的内容。

   选择用于创建电子邮件内容的方法。 在本例中，我们要导入现有HTML内容。

   ![](assets/import-html.png)

1. 选择要导入的HTML或ZIP文件，然后单击 **[!UICONTROL 下一个]**.

   如果您的文件夹包含资产，请选择应将资产存储到的实例和文件夹，然后单击 **[!UICONTROL 导入]**. （+链接到资产上的文档？）

   ![](assets/import-folder.png)

1. 导入内容后，该内容会显示在Email Designer中，以便您根据需要对其进行编辑并添加个性化。

   在此示例中，我们要在电子邮件标题中添加个性化。 要执行此操作，请选择组件块，然后单击 **[!UICONTROL 添加个性化]**.

   ![](assets/add-perso.png)

1. 准备好内容后，保存该内容，然后单击箭头以返回到电子邮件创建屏幕。

   ![](assets/save-content.png)

## 定义受众 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="定义受众"
>abstract="热障涂层"

1. 单击 **[!UICONTROL 选择受众]** 按钮，然后选择现有受众或创建新受众。

   在此示例中，我们希望使用现有受众来定位属于银牌和金牌忠诚度积分级别的客户。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >列表中可用的受众源自您的Campaign V8实例，或来自Adobe Experience Platform（如果已在您的实例上实施目标/源集成）。 了解如何选择电子邮件受众

1. 选择受众后，您可以根据需要编辑规则。 您还可以设置一个控制组，以将电子邮件收件人的行为与未定向用户档案的行为进行比较。 了解如何与控制组合作

## 计划发送 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="计划发送"
>abstract="热障涂层"

要计划电子邮件的发送，请单击启用，然后指定所需的日期和时间。

=发送前确认选项：计划日期会发生什么情况：确认消息发送的通知？

![](assets/schedule.png)

## 预览和测试电子邮件 {#preview-test}

电子邮件准备就绪后，您可以先预览并测试该电子邮件，然后再启动其发送。

1. 单击 **[!UICONTROL 审阅以发送]**. 此时会显示电子邮件的预览，以及所有已配置的属性、受众和计划。 您可以使用修改按钮编辑其中的任何元素。

   ![](assets/review-email.png)

1. 单击 **[!UICONTROL 模拟内容]** 按钮以预览电子邮件并发送校样。

1. 在左侧区域中，选择要用于预览电子邮件的用户档案。 您可以使用目标用户档案或专用测试用户档案。

1. 基于所选用户档案的右侧区域将显示电子邮件的预览。 如果已添加多个用户档案，则可以在其中每个用户档案之间切换，以预览相应的电子邮件。

   ![](assets/preview.png)

   >[!NOTE]
   >
   >此外， **[!UICONTROL 呈现电子邮件]** 按钮，您可以使用多个设备或邮件提供商预览电子邮件。 了解如何预览电子邮件渲染

1. 要发送电子邮件的校样，请单击 **[!UICONTROL 测试]** 按钮，然后选择将接收校样的用户档案。 在本例中，我们希望将校样发送到特定的测试用户档案。

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >您还可以通过模拟某些定向的用户档案并将校样消息发送到所选的电子邮件地址来测试消息。 了解如何使用“从目标中替换”模式

1. 单击 **[!UICONTROL 发送测试电子邮件]** 然后确认发送。

   发送校样后，您可以单击 **[!UICONTROL 查看测试电子邮件日志]** 按钮。

## 发送并监视电子邮件 {#prepare-send}

审核并测试电子邮件后，即可启动其准备并发送。

1. 单击 **[!UICONTROL 准备]** 以启动消息的准备工作。

   您可以实时跟踪准备进度和统计信息。 准备完成后，您可以访问详细的日志以进一步分析。 了解如何监控投放

   ![](assets/preparation.png)

1. 准备好发送电子邮件后，单击 **[!UICONTROL 发送]** 然后确认发送。

   您可以实时跟踪发送情况以及统计信息。 此外， **[!UICONTROL 日志]** 按钮，可访问有关电子邮件发送的详细信息。 了解如何监控投放

   ![](assets/logs.png)

1. 发送电子邮件后，您可以访问专用报告以进行进一步分析。

   ![](assets/reports.png)
