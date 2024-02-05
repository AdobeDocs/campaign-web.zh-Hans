---
title: Campaign Web用户界面的护栏和限制
description: Campaign Web用户界面的护栏和限制
badge: label="Beta 版"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: db06e0f54984991e1d6b1056932a9974e340546e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 65%

---

# 护栏和限制 {#guardrails-limitations}

在Campaign Web用户界面中使用在Campaign客户端控制台中创建或修改的组件时，以下列出的护栏和限制适用。

## 工作流 {#wf-guardrails-limitations}

### 活动

Campaign Web用户界面中尚不支持的工作流活动是只读的，并且显示为不兼容的活动。 仍可执行工作流、发送消息、检查日志等。在Campaign Web用户界面和Campaign客户端控制台中可用的工作流活动均可编辑。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

不会显示Web用户界面中尚不受支持的工作流活动设置。 但是，在执行工作流时适用这些设置。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

在控制台中，**扩充**&#x200B;活动可执行协调和扩充。在Campaign Web用户界面中，协调功能尚不可用。 如果您在客户端控制台中定义了 **扩充** 活动，在Campaign Web用户界面中显示为不兼容的只读活动。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### 画布

在Campaign Web用户界面中创建新工作流时，画布仅支持一个入口点。 但是，如果您在控制台中创建了一个具有多个入口点的工作流，则可以在Campaign Web用户界面中打开并编辑该工作流。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

循环在Campaign Web用户界面中尚不可用。 如果您使用控制台创建了包含循环的工作流，则无法从Campaign Web用户界面访问该工作流。 并显示一条错误消息。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

每次添加或删除活动时都会刷新节点的定位。如果在控制台中创建工作流，并使用Campaign Web用户界面修改它，然后在控制台中重新打开它，您可能会注意到一些细微的定位缺陷。 这种情况不影响工作流的过程和任务。

| 初始工作流 | 定位更改 |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## 预定义过滤器 {#filters-guardrails-limitations}

>[!CONTEXTUALHELP]
>id="acw_predefined_filter_read_only"
>title="此过滤器为只读"
>abstract="在该产品版本的用户界面中没有某些预定义过滤器可用。这些过滤器被标为只读。即使无法在查询建模器中查看查询的图形表示形式，也无法编辑过滤器，您仍可使用它，并在屏幕的&#x200B;**属性**&#x200B;部分中查看过滤条件。"

在产品的该版本中，当选择投放的受众或在工作流中生成受众时，在用户界面中找不到某些预定义过滤器。这些过滤器被标为只读。

并显示一条具体的错误消息。

![](assets/filter-unavailable.png){width="70%" align="left"}

即使无法在查询建模器中查看查询的图形表示形式，也无法编辑过滤器，您仍可使用它，并在屏幕的&#x200B;**属性**&#x200B;部分中查看过滤条件。

![](assets/rule-edit.png){width="70%" align="left"}

还可访问 SQL 查询以检查确切的设置。为此，请单击&#x200B;**代码视图**&#x200B;按钮。

![](assets/rule-code-view.png){width="70%" align="left"}

单击&#x200B;**计算**&#x200B;按钮以检查有多少个项目符合过滤器的标准。

![](assets/rule-calculate.png){width="70%" align="left"}

使用&#x200B;**查看结果**&#x200B;按钮显示这些项目。

![](assets/rule-view-results.png){width="70%" align="left"}

请注意，如果在 Web 界面中生成一个过滤器，然后在控制台中用不支持的属性修改它，则在 Web 界面中无法再找到图形表示形式。在任何情况下都仍可使用该过滤器。

下面列出了不支持的属性。

### 不支持的数据类型 {#unsupported-data-type}

在 Web 界面中显示过滤器或规则时，不支持可在客户端控制台中找到的以下数据类型：

* datetime
* time
* timespan
* double
* float

### 不支持的过滤功能 {#unsupported-filtering-capabilities}

在客户端控制台中用复杂的表达式和函数生成过滤器时，无法在 Web 界面中编辑该过滤器。

此外，不支持以下运算符：

* 数值型
   * is included in
   * no in

* 字符串类型
   * greater than
   * less than
   * greater than or equals to
   * less than or equals to
   * like
   * not like

* 日期类型
   * on or after
   * on or before
   * not equals to
   * is empty
   * is not empty
   * is included in
   * not in
   * in last

* 1 对多链接
   * COUNT、SUM、AVG、MIN、MAX
