---
audience: end-user
title: 创建推送通知投放
description: 了解如何使用Adobe Campaign Web创建推送通知投放
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 933cfcdfb9ff9a176f4942e349b882c404c4e2a8
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 31%

---

# 创建推送通知投放 {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="推送通知模板"
>abstract="选择推送通知模板以开始投放推送。通过投放模板，可轻松地在营销活动和投放中重用自定义内容和设置。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=zh-Hans" text="使用投放模板"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="推送投放属性"
>abstract="定义您的推送投放属性。输入推送的标签并使用&#x200B;**其他选项**&#x200B;配置内部名称、投放文件夹和代码。您还可以输入自定义描述。"

您可以创建独立的推送通知投放，也可以在活动工作流的上下文中创建推送通知。 以下步骤详细介绍了独立（一次性）推送投放的过程。 如果您在活动工作流的上下文中工作，有关创建步骤的详细信息，请参阅 [本节](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## 创建推送投放 {#create-push-delivery}

要创建新的独立推送投放，请执行以下步骤：

1. 浏览至 **[!UICONTROL 投放]** 菜单，然后单击  **[!UICONTROL 创建投放]** 按钮。

1. 在 **[!UICONTROL 渠道]** 部分，选择 **推送通知** 作为渠道，并根据选择的设备操作系统(Android或iOS)选择模板。 [了解有关模板的更多信息](../msg/delivery-template.md)

1. 单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮以进行确认。

   ![](assets/push_create_1.png){zoomable=&quot;yes&quot;}

## 配置投放设置 {#configure-push-settings}

按如下所述配置您的投放设置：

1. 输入 **[!UICONTROL 标签]** 用于投放。 默认情况下，使用所选模板的标签设置标签。 它应进行更新。

1. 浏览 **[!UICONTROL 其他选项]** 下拉菜单以根据需要自定义选项。 如果您的投放基于扩展模式，请指定 **自定义选项** 字段可用。

   +++根据您的要求配置以下设置。
   * **[!UICONTROL 内部名称]**：为投放分配一个唯一标识符。
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中。
   * **[!UICONTROL 投放代码]**：使用您自己的命名惯例整理投放。
   * **[!UICONTROL 描述]**：提供投放的描述。
   * **[!UICONTROL 自然]**：指定投放的性质以进行分类。
+++


## 选择您的投放受众 {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="定义推送通知受众"
>abstract="要定义消息的受众，您必须首先选择与推送投放关联的应用程序。默认情况下，将您的推送通知发送到应用程序的所有订阅者。可通过单击&#x200B;**选择受众**&#x200B;按钮而细化到特定受众。如果需要，可添加对照组以衡量投放的影响力。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=zh-Hans" text="设置对照组"


您必须先选择应用程序，然后优化推送通知受众，如下所述：

1. 从 **[!UICONTROL 受众]** 部分，选择要用于此投放的应用程序。 默认情况下，将您的推送通知发送到应用程序的所有订阅者。您可以通过单击 **[!UICONTROL 选择受众]** 按钮。

   ![](assets/push_create_2.png){zoomable=&quot;yes&quot;}

1. 选择现有受众，或创建自己的受众，以优化推送投放的目标群体。 对于推送通知，默认为 [目标维度](../audience/about-recipients.md#targeting-dimensions) 是 **订阅者应用程序** (nms：appSubscriptionRcp)，链接到收件人表。

   了解如何在中选择现有受众 [此页面](../audience/add-audience.md)

   了解如何在中创建新受众 [此页面](../audience/one-time-audience.md)

1. 打开 **[!UICONTROL 启用对照组]** 用于设置控制组以测量投放影响的选项。 消息不会发送到该控制组，因此您可以将收到消息的群体的行为与未收到消息的联系人的行为进行比较。 [了解详情](../audience/control-group.md)

## 定义推送通知内容 {#create-content-push}

要定义通知的内容，请单击 **[!UICONTROL 编辑内容]**. [了解详情](content-push.md)

![](assets/push_create_5.png){zoomable=&quot;yes&quot;}

在此屏幕中，您还可以 [模拟您的内容](../preview-test/preview-test.md) 和 [设置优惠](../msg/offers.md).

## 计划投放发送 {#schedule-push}

在工作流上下文中发送投放时，您必须使用 **计划程序** 活动。 了解详情，请参阅 [此页面](../workflows/activities/scheduler.md). 以下步骤仅适用于独立投放。

要将独立推送投放计划为特定日期和时间，请执行以下步骤：

1. 浏览至 **[!UICONTROL 计划]** 投放属性的部分。

1. 使用 **[!UICONTROL 启用计划]** 切换以激活它。

1. 设置所需的发送日期和时间。

启动投放后，系统会在您为收件人定义的确切日期和时间自动发送消息。

![](assets/push_create_3.png){zoomable=&quot;yes&quot;}

在中了解有关投放计划的更多信息 [本节](../msg/gs-messages.md#gs-schedule)

## “交付”高级设置 {#adv-push}

单击 **[!UICONTROL 配置投放设置]** 访问与投放模板相关的高级选项。 [了解详情](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png){zoomable=&quot;yes&quot;}
