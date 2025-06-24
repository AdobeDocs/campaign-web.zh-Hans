---
audience: end-user
title: 投放警报
description: 了解如何使用投放警报。
badge: label="有限发布版"
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: a28bc98d1735232d8aa0b0daaeca3969913e548c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 26%

---

# 投放警报条件 {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="投放提醒标准仪表板"
>abstract="Campaign Web 用户界面提供了预定义的提醒条件（吞吐量低的投放、准备失败的投放......），你可以将其添加到你的仪表板。您还可以创建自己的条件来满足您的需要。"

Campaign Web用户界面提供了预定义的警报标准，例如可添加到功能板的低吞吐量投放或准备失败的投放。 您还可以创建自己的条件来满足您的需要。

可从左侧导航窗格的&#x200B;**传递警报**&#x200B;菜单（**条件**&#x200B;选项卡下）访问警报条件。

![投放警报菜单中显示的警报条件列表](assets/alerting-criteria-list.png)

>[!AVAILABILITY]
>
>此功能位于有限可用性(LA)中。 仅供&#x200B;**从 Adobe Campaign Standard 迁移到 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境上。

## 预定义的警报条件 {#ootb-criteria}

Campaign Web用户界面中提供了预定义的警报标准。 这些标准涵盖一系列场景，如下所示：

* **投放失败**：在定义的范围内计划的任何投放，状态错误。
* **准备的投放失败**：在定义的范围内修改的任何投放，其准备步骤（目标计算和内容生成）失败。
* **软退回的错误率很低的投放**：在定义的范围内计划的任何投放，其状态至少为“进行中”，且软退回错误率大于定义的百分比。
* **硬退回的错误率为错误的投放**：在定义的范围内计划的任何投放，其状态至少为“进行中”，且硬退回错误率大于定义的百分比。
* **等待长时间开始的投放**：任何在定义的范围内计划的投放，其“等待开始”状态超过定义的持续时间。 “开始挂起”状态表示系统尚未考虑这些消息。
* **低吞吐量的投放**：任何开始传递的时间均超过定义的持续时间，并且已处理消息的百分比小于定义的百分比，吞吐量低于定义的值。
* **正在进行的投放**：在定义的范围内计划的任何投放，状态为“正在进行”。

>[!NOTE]
>
>默认值将应用于上述标准的所有参数。 可以在投放警报仪表板的&#x200B;**标准参数**&#x200B;部分中自定义这些值，正在使用它们。 [了解如何使用仪表板](../msg/delivery-alerting-dashboards.md)

## 创建提醒条件 {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="创建投放提醒条件"
>abstract="除了 Adobe Campaign 提供的预定义警报标准外，您还可以创建自己的标准来满足您的需求。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="添加到提醒中的指标"
>abstract="选择要在电子邮件提醒的“详细信息”部分中显示为列的指标。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="提醒类型"
>abstract="指定条件的&#x200B;**提醒类型**，即在提醒的“摘要”部分中投放条件旁边显示的标签和颜色。"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="条件频率"
>abstract="控制符合条件的每次投放的每日提醒频率。"

要创建新标准，请执行以下步骤：

1. 导航到左侧导航窗格中的&#x200B;**投放警报**&#x200B;菜单，然后选择&#x200B;**标准**&#x200B;选项卡。
1. 单击&#x200B;**创建投放警报条件**&#x200B;按钮。
1. 提供条件的标签。 内部名称会自动填充为只读。
1. 使用此标准应用的&#x200B;**投放过滤器**&#x200B;通过对其应用预定义过滤器来细化该标准的范围。

   在以下示例中，已选择&#x200B;**正在进行的投放(critInProgressDeliveries)**&#x200B;过滤器，这意味着该条件只考虑具有“正在进行”状态的投放。

   ![带有选定筛选器的警报条件属性示例](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >如果任何预定义过滤器都不适合您的需要，您可以从&#x200B;**客户管理** > **预定义过滤器**&#x200B;菜单创建您自己的过滤器。 [了解更多信息](../get-started/predefined-filters.md)
   >
   >此操作只能由高级用户执行。

1. 在要添加到警报的&#x200B;**指示符**&#x200B;部分中，选择要作为列显示在电子邮件警报的“详细信息”部分中的指示符。

1. 指定条件的&#x200B;**提醒类型**，即在提醒的“摘要”部分中投放条件旁边显示的标签和颜色。

1. 使用&#x200B;**标准频率**&#x200B;部分控制每个符合条件的投放每天的警报频率：

   * **将在每个通知中重复此传递条件**：在当天的所有电子邮件警报中显示符合该条件的传递。
   * **此传递标准仅在一天的第一次发生时发送**：仅在当天的第一次报告中显示符合该标准的传递，而不会在后续电子邮件警报中重复该传递。