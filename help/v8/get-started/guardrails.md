---
title: Campaign Web UI 中的护栏和限制
description: Campaign Web UI 中的护栏和限制
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: ht
source-wordcount: '588'
ht-degree: 100%

---

# 护栏和限制 {#guardrails-limitations}

在 Campaign Web UI 中使用在 Campaign 客户端控制台中创建或修改的组件时，适用以下列出的护栏和限制。

## 工作流 {#wf-guardrails-limitations}

### 活动

Web UI 中尚不支持的工作流活动为只读活动，并显示为不兼容的活动。仍可执行工作流、发送消息、检查日志等。可编辑在 Web UI 和客户端控制台中都能找到的工作流活动。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

不显示 Web UI 中尚不支持的工作流活动设置。但是，在执行工作流时适用这些设置。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

在控制台中，**扩充**&#x200B;活动可执行协调和扩充。在 Web UI 中尚无协调功能可用。如果已在控制台中定义&#x200B;**扩充**&#x200B;活动中的协调设置，则该活动将在 Web UI 中显示为不兼容的只读活动。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### 画布

在 Web UI 中创建新工作流时，画布仅支持一个入口点。但是，如果在控制台中创建具有多个入口点的工作流，则可在 Web UI 中打开并编辑该工作流。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

在 Web UI 中尚无循环可用。如果使用控制台创建了包括循环的工作流，则无法从 Web UI 访问该工作流。并显示一条错误消息。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

每次添加或删除活动时都会刷新节点的定位。如果在控制台中创建工作流，使用 Web UI 修改它，然后在控制台中重新打开它，则可能会发现一些细微的定位瑕疵。这种情况不影响工作流的过程和任务。

| 初始工作流 | 定位更改 |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## 预定义过滤器 {#filters-guardrails-limitations}

在产品的该版本中，当选择投放的受众或在工作流中生成受众时，在用户界面中找不到某些预定义过滤器。

并显示一条具体的错误消息。

![](assets/filter-unavailable.png){width="70%" align="left"}

即使无法在规则生成器中查看查询的图形表示形式，也无法编辑过滤器，您仍可使用它，并在屏幕的&#x200B;**属性**&#x200B;部分中查看过滤条件。

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
