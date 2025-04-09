---
audience: end-user
title: 使用查询建模器
description: 了解如何使用Adobe Campaign Web查询建模器。
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: bf7ee45a0702b66af6962453893cf9c50c140d54
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 20%

---

# 使用查询建模器 {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="新的查询建模器"
>abstract="Adobe Campaign Web 具有一个查询建模器，它可简化过滤数据库的过程以根据各种条件选择特定目标。其中包括使用高级表达式和运算符。在每个需要定义规则以过滤数据的环境下都有查询建模器可用。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="查询建模器"
>abstract="为收件人或数据库中的任何其他目标选择维度定义过滤条件。利用 Adobe Experience Platform 受众进一步细化目标受众，并最大限度地提高营销活动的影响力。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="细化目标"
>abstract="这些规则只能在客户端控制台中进行更改。"

Adobe Campaign Web user interface features a query modeler that simplifies the process of filtering the database based on various criteria. 它确保与在客户端控制台中创建的查询完全兼容，从而促进到Web用户界面的无缝过渡。

此外，查询建模器可以高效地管理非常复杂和长的查询，提供增强的灵活性和精确度。 此外，它支持条件中的预定义过滤器，使您能够轻松优化查询，同时利用高级表达式和运算符实现全面的受众定位和分段策略。

## 访问查询建模器

在每个需要定义规则以过滤数据的环境下都有查询建模器可用。

| 使用情况 | 示例 |
|  ---  |  ---  |
| **Define audiences**: Specify the population you want to target in your messages or workflows, and effortlessly create new audiences tailored to your needs. [Learn how to build audiences](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Customize workflow activities**: apply rules within workflow activities, such as **Split** and **Reconciliation**, to align with your specific requirements. [Learn more on workflow activities](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Predefined filters**: Create predefined filters that serve as shortcuts during various filtering operations, whether you&#39;re working with data lists or forming the audience for a delivery. [Learn how to work with predefined filters](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **筛选报表数据**：添加规则以筛选报表中显示的数据。 [Learn how to work with reports](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **自定义列表**：创建自定义规则以筛选显示在列表中的数据，如收件人、投放列表等。 [了解如何筛选列表](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **生成条件内容**：通过创建条件来定义应该向不同收件人显示哪些内容，从而生成动态的电子邮件内容，确保发送个性化的相关消息。 [了解如何生成条件内容](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} |

>[!NOTE]
>
>When accessing an object created in the client console where rules have been applied such as an audience or a predefined filter, the **[!UICONTROL Refine target]** section may display. This means that additional parameters have been configured to refine the rule target. These parameters can be modified in the console only.
>
>![](assets/target-warning.png){zoomable="yes"}

## 查询建模器接口 {#interface}

>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="新用户体验"
>abstract="使用此切换开关可在经典查询建模器和新的规则生成器体验之间切换。"

查询建模器提供了一个中央画布，您可以在其中构建查询，以及一个右窗格，提供有关查询的信息。

![](assets/query-interface.png){zoomable="yes"}

### 中央画布 {#canvas}

在查询建模器中心画布上，您可以添加和组合构建查询的不同组件。 [了解如何生成查询](build-query.md)

位于画布右上角的工具栏提供了一些选项，用于轻松处理查询组件并在画布中导航：

* **多重选择模式**：选择多个筛选组件以将其复制并粘贴到您选择的位置。
* **旋转**：垂直切换画布。
* **适合屏幕**：根据屏幕调整画布缩放级别。
* **缩小** / **放大**：缩小或缩小画布。
* **显示映射**：打开显示您所在位置的画布快照。

### 规则属性窗格 {#rule-properties}

在右侧，**[!UICONTROL 规则属性]**&#x200B;窗格提供有关查询的信息。 它允许您执行各种操作来检查查询并确保查询符合您的需求。 构建查询以创建受众时，显示此窗格。 [了解如何检查和验证您的查询](build-query.md#check-and-validate-your-query)
