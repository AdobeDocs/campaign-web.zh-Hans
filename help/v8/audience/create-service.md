---
audience: end-user
title: 使用订阅服务
description: 了解如何在Adobe Campaign Web中创建服务
badge: label="Beta"
source-git-commit: dd8e8acb37cf9a68768c5da48335275c09d67cc8
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# 使用订阅服务 {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="创建和管理您的服务"
>abstract="使用Adobe Campaign创建和监控服务（如新闻稿），并检查这些服务的订阅/退订。 订阅仅适用于电子邮件和短信投放。"

使用Adobe Campaign Web管理和创建您的服务（如新闻稿），并检查这些服务的订阅/退订。

>[!NOTE]
>
>订阅仅适用于电子邮件和短信投放。

可以并行定义多种服务，例如：特定产品类别、网站主题或区域的新闻稿、各种类型警报消息的订阅以及实时通知。

要了解有关管理订阅和退订的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## 访问订阅服务 {#access-services}

要访问您的平台可用的订阅服务，请浏览 **[!UICONTROL 订阅服务]** 菜单的位置。

![](assets/service-list.png)

此时将显示所有现有订阅服务的列表。 您可以搜索服务和筛选渠道、文件夹，或者使用高级筛选器。

![](assets/service-filters.png)

要编辑现有服务，请单击其名称。

## 创建您的第一个订阅服务 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="订阅服务属性"
>abstract="输入订阅服务的标签，并定义其他选项。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="订阅服务确认消息"
>abstract="当用户订阅服务或取消订阅服务时，您可以发送确认消息。 选择要用于这些消息的模板。"


要创建订阅服务，请执行以下步骤：

1. 选择 **[!UICONTROL 创建订阅服务]** 按钮。

   ![](assets/service-create-button.png)

1. 选择渠道： **[!UICONTROL 电子邮件]** 或 **[!UICONTROL 短信]**.

1. 在服务属性中，输入标签并根据需要定义其他选项。

   ![](assets/service-create-properties.png)

1. 默认情况下，订阅无限制。 您可以禁用 **[!UICONTROL 有效期无限制]** 用于定义服务的有效期的选项。 <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. 当用户订阅或取消订阅服务时，您可以发送确认消息。 根据您的用例选择用于该消息的模板。

   ![](assets/service-create-confirmation-msg.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。新服务将添加到 **[!UICONTROL 订阅服务]** 列表。

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


