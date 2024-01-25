---
audience: end-user
title: 使用订阅服务
description: 了解如何在Adobe Campaign Web中访问、创建和管理订阅服务
badge: label="有限发布版"
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: cbfd821173466c51e9073f01e8792cbdc069c6a2
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 23%

---

# 创建和管理订阅服务 {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="创建和管理服务"
>abstract="使用 Adobe Campaign 创建和监测您的服务（如新闻稿）以及检查这些服务的订阅或取消订阅情况。订阅仅适用于电子邮件和短信投放。"

使用Adobe Campaign Web管理和创建服务（如新闻稿），并检查这些服务的订阅或退订。

>[!NOTE]
>
>订阅仅适用于电子邮件和短信投放。

可以并行定义多种服务，例如：特定产品类别、网站主题或区域的新闻稿、各种类型警报消息的订阅以及实时通知。

要了解有关管理订阅和退订的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## 访问订阅服务 {#access-services}

要访问适用于您的平台的订阅服务，请执行以下步骤。

1. 浏览至 **[!UICONTROL 订阅服务]** 菜单的位置。

   ![](assets/service-list.png)

1. 此时将显示所有现有订阅服务的列表。 您可以搜索服务，并在渠道、文件夹上使用添加规则 [查询建模器](../query/query-modeler-overview.md).

   ![](assets/service-filters.png)

1. 要编辑现有服务，请单击其名称。

1. 您可以使用服务名称旁边的三个圆点图标来删除或复制任何服务。<!--so all subscribers are unsubscribed - need to mention?-->

## 创建您的第一个订阅服务 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="定义服务属性"
>abstract="输入订阅服务的标签并定义其他选项，如服务的有效期。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="选择确认消息"
>abstract="当用户订阅服务或从服务取消订阅时，您可发送确认消息。选择用于该消息的模板。"

要创建订阅服务，请执行以下步骤。

1. 选择 **[!UICONTROL 创建订阅服务]** 按钮。

   ![](assets/service-create-button.png)

1. 选择渠道： **[!UICONTROL 电子邮件]** 或 **[!UICONTROL 短信]**.

1. 在服务属性中，输入标签并定义 **[!UICONTROL 其他选项]** 如所愿。

   ![](assets/service-create-properties.png)

1. 默认情况下，服务存储在 **[!UICONTROL 服务和订阅]** 文件夹。 您可以通过浏览到所需的位置来更改它。 [了解如何使用文件夹](../get-started/permissions.md#folders)

1. 默认情况下，订阅无限制。 您可以禁用 **[!UICONTROL 有效期无限制]** 用于定义服务的有效期的选项。

   在下面的示例中，20天后：
   * 收件人将无法再订阅此服务。
   * 此服务的所有订阅者将在20天后自动取消订阅。 [了解详情](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. 当用户订阅服务或从服务取消订阅时，您可发送确认消息。根据您的用例选择用于该消息的模板。 这些模板必须配置 **[!UICONTROL 订阅]** 目标映射。 [了解详情](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. 单击 **[!UICONTROL 保存并审阅]**. 新服务将添加到 **[!UICONTROL 订阅服务]** 列表。

您现在可以：

* 将订阅者添加到此服务，并取消订阅收件人。 [了解详情](../msg/send-to-subscribers.md)

* 向此服务的订阅者发送消息。 [了解如何操作](../msg/send-to-subscribers.md)

## 创建确认消息 {#create-confirmation-message}

要向订阅或取消订阅服务的用户发送确认消息，您必须使用创建投放模板 **[!UICONTROL 订阅]** 目标映射，无已定义目标。 为此，请执行以下步骤。

1. 为订阅确认创建投放模板。 [了解如何创建模板](../msg/delivery-template.md)

1. 请勿为此投放选择受众。 相反，请访问投放 **[!UICONTROL 设置]**，转到 [受众](../advanced-settings/delivery-settings.md#audience) 选项卡，然后选择 **[!UICONTROL 订阅]** 列表中的目标映射。

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >如果您不选择  **[!UICONTROL 订阅]** 目标映射，您的订阅者将不会收到确认消息。 目标映射在Campaign v8控制台中定义。 在中了解详情 [Adobe Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

1. 编辑投放模板的内容，保存并关闭它。

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >了解有关投放渠道以及如何在中定义投放内容的更多信息 [电子邮件渠道](../email/create-email.md) 和 [短信渠道](../sms/create-sms.md) 部分。

1. 重复上述步骤以创建用于取消订阅确认的投放模板。

现在，您可以在以下情况下选择这些消息 [创建订阅服务](#create-service). 订阅或取消订阅该服务的用户将收到所选的确认消息。

## 监测订阅服务 {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="订阅者总数"
>abstract="单击&#x200B;**计算**&#x200B;获取此服务的订阅者总数。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="相关时段的订阅数"
>abstract="使用下拉列表更改时间范围并查看所选时段内的订阅数和取消订阅数。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="订阅整体演变"
>abstract="此图显示按时段划分的细分情况，包括订阅数、取消订阅数、数量演变和忠诚度百分比。"

要衡量订阅服务对短信和电子邮件渠道的有效性，您可以访问给定服务的日志和报告。

1. 从中选择现有服务 **[!UICONTROL 订阅服务]** 列表。 单击 **[!UICONTROL 计算]** 将获取订阅者的总数。

   ![](assets/service-logs-subscribers-count.png)

1. 从服务仪表板中，选择 **[!UICONTROL 日志]** 查看此服务的订阅者列表。

   您可以检查订阅者总数、每个收件人的姓名和地址以及他们订阅或取消订阅的时间。 您还可以对其进行过滤。

   ![](assets/service-logs.png)

1. 从服务仪表板中，选择 **[!UICONTROL 报表]**. 检查以下指示器：

   * 此 **[!UICONTROL 订阅者总数]** 将显示。

   * 您可以查看选定时段内的订阅和退订数量。 使用下拉列表更改时间范围。

     ![](assets/service-reports.png)

   * 此 **[!UICONTROL 订阅的总体演变]** 图表按期间显示细分，包括订阅、取消订阅、数量演变和忠诚度百分比。<!--what is Registered?-->

1. 使用 **[!UICONTROL 重新加载]** 按钮以检索跟踪工作流执行和计划的最后一个值。
