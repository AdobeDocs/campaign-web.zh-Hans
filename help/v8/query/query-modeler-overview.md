---
audience: end-user
title: 使用查询建模器
description: 了解如何使用Adobe Campaign Web查询建模器。
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 14%

---

# 使用查询建模器 {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="新建规则生成器"
>abstract="现在提供了新的规则生成器，帮助您在改进的用户界面中定义复杂的条件。 您可以根据需要从旧规则生成器切换到新规则生成器。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

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

Adobe Campaign Web用户界面提供了一个查询建模器，可简化根据各种标准筛选数据库的过程。 它确保与在客户端控制台中创建的查询完全兼容，从而促进到Web用户界面的无缝过渡。

此外，查询建模器还可以高效地管理非常复杂和冗长的查询，从而提高灵活性和精确度。 它还支持条件中的预定义过滤器，使用户能够轻松优化查询，同时利用高级表达式和运算符实现全面的受众定位和分段策略。

## 访问查询建模器

在每个需要定义规则以过滤数据的环境下都有查询建模器可用。

| 使用情况 | 示例 |
|  ---  |  ---  |
| **定义受众**：指定要在消息或工作流中定位的群体，并轻松创建根据您的需求定制的新受众。 [了解如何构建受众](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [显示如何访问受众创建界面的图像] |
| **自定义工作流活动**：在工作流活动中应用规则（如&#x200B;**拆分**&#x200B;和&#x200B;**协调**）以符合您的特定要求。 [了解有关工作流活动的更多信息](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [显示如何访问工作流自定义选项的图像] |
| **预定义筛选器**：创建预定义筛选器，这些筛选器可在各种筛选操作期间用作快捷键，无论您是使用数据列表还是组成投放的受众。 [了解如何使用预定义过滤器](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [显示如何访问预定义过滤器的图像] |
| **筛选报表数据**：添加规则以筛选报表中显示的数据。 [了解如何使用报表](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [显示如何过滤报表中数据的图像] |
| **自定义列表**：创建自定义规则以筛选显示在列表（如收件人列表或投放列表）中的数据。 [了解如何筛选列表](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [显示如何自定义列表筛选器的图像] |
| **生成条件内容**：通过创建条件来定义应该向不同收件人显示哪些内容，从而动态生成电子邮件内容，确保发送个性化的相关消息。 [了解如何生成条件内容](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [显示如何创建条件内容的图像] |

>[!NOTE]
>
>访问在应用规则的客户端控制台中创建的对象（如受众或预定义过滤器）时，可能会显示&#x200B;**[!UICONTROL 优化目标]**&#x200B;部分。 这意味着已配置其他参数来优化规则目标。 这些参数只能在控制台中修改。
>
>![显示有关优化目标的警告的图像](assets/target-warning.png){zoomable="yes"}

## 查询建模器界面 {#interface}

查询建模器提供了一个中央画布（可在其中构建查询）和一个右窗格（提供有关查询的信息）。

>[!IMPORTANT]
>
>提供了全新的查询建模器界面。 新的规则生成器简化了界面，让您能够更轻松地构建查询。 要切换到此体验，请按右上角的切换按钮。 您可以随时返回经典查询建模器，只需返回切换开关以禁用新界面即可。 您可以应用与这个新界面中的查询建模器相同的原则。
>![显示新规则生成器界面](assets/query-modeler-toggle.png){zoomable="yes"}切换的图像


>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="新的规则生成器体验"
>abstract="使用此切换开关可在经典查询建模器和新规则生成器体验之间切换。 新的规则生成器具有简单直观的界面，可让您更轻松地构建查询。"

![显示查询建模器接口的图像](assets/query-interface.png){zoomable="yes"}

### 中央画布 {#canvas}

在查询建模器中心画布上，您可以添加和组合不同的组件来构建查询。 [了解如何生成查询](build-query.md)

>[!BEGINTABS]

>[!TAB 经典查询建模器]

位于画布右下角的工具栏提供了一些选项，用于轻松处理查询组件和导航画布：

* **多重选择模式**：选择多个筛选组件以将其复制并粘贴到您选择的位置。
* **旋转**：垂直切换画布。
* **适合屏幕**：根据屏幕调整画布缩放级别。
* **缩小** / **放大**：缩小或放大画布。
* **显示映射**：打开显示当前位置的画布快照。

>[!TAB 新规则生成器体验]

位于画布右上角的工具栏提供了一些选项，用于轻松处理查询组件和导航画布：

* **上移选定内容**：将组件上移一行。
* **下移选定内容**：将组件下移一行。
* **组选择**：将两个组件放入组中。
* **取消分组选择**：将单个组的组件分开。
* **全部展开**：展开所有组。
* **全部折叠**：折叠所有组。
* **删除所有**：删除所有组和组件。

>[!ENDTABS]

### 规则属性窗格 {#rule-properties}

在右侧，**[!UICONTROL 规则属性]**&#x200B;窗格提供有关查询的信息。 它允许您执行各种操作来检查查询并确保查询符合您的需求。 构建查询以创建受众时，显示此窗格。 [了解如何检查和验证您的查询](build-query.md#check-and-validate-your-query)
