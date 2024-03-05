---
audience: end-user
title: 过滤器列表
description: 了解如何使用内置和自定义筛选器来筛选Adobe Campaign Web列表。
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 7%

---

# 过滤器列表 {#filter-lists}

Adobe Campaign Web在每个对象列表中提供过滤器，使您能够根据特定的上下文条件过滤信息。 例如，您可以按状态、渠道、联系日期或文件夹过滤投放。您还可以隐藏校样。

## 应用过滤器{#apply}

要将筛选器应用到列表，请单击 **[!UICONTROL 显示筛选器]** 按钮，位于列表的左上角，搜索栏旁边。

过滤器窗格随即打开，显示选定列表的可用过滤器。 例如，您可以根据营销活动的状态、开始和结束日期或存储文件夹筛选营销活动，而根据营销活动的渠道和存储文件夹筛选订阅服务列表。

![](assets/filters-pane.png){zoomable=&quot;yes&quot;}{width="70%" align="left" zoomable="yes"}

要根据您自己的条件筛选列表，请创建自定义筛选条件。 为此，请浏览到过滤器窗格的底部，然后单击 **添加规则** 按钮。 [了解如何创建自定义筛选条件](#custom)

筛选器应用于列表后，即可在搜索栏下方可见。 您可以随时删除单个过滤器，也可以通过单击 **全部清除** 按钮。

## 创建自定义筛选条件 {#custom}

自定义筛选条件允许您根据自己的特定条件优化列表。 它们使用Campaign查询建模器设计。 要创建自定义过滤器，请执行以下步骤：

1. 打开筛选器窗格，然后单击 **添加规则** 位于窗格底部的按钮。
1. 此时将打开查询建模器。 根据需要，定义并组合过滤器标准。 有关如何使用查询建模器的详细信息，请参阅 [本节](../query/query-modeler-overview.md).

   以下示例显示了一个自定义过滤器，该过滤器设计为在营销活动列表中显示由运行部门或瑜伽部门的操作员运行的短信营销活动。

   ![](assets/filters-sample.png){zoomable=&quot;yes&quot;}{width="70%" align="left" zoomable="yes"}

1. 配置自定义筛选条件后，单击 **[!UICONTROL 确认]** 以将其应用于列表。
