---
title: Campaign Web UI中的护栏和限制
description: Campaign Web UI中的护栏和限制
badge: label="Beta"
source-git-commit: 9ab03458bbd9606537c0b42d72643cf1efefcc81
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 4%

---


# 护栏和限制 {#guardrails-limitations}

在Campaign Web UI中使用在Campaign客户端控制台中创建或修改的组件时，以下列出的护栏和限制适用。

## 工作流 {#wf-guardrails-limitations}

**活动版本**

* Web UI中尚不支持的工作流活动是只读的。 您仍然可以执行工作流、发送消息、检查日志等。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-activities-console.png) | ![](assets/limitations-activities-web.png) |

**画布版本**

* 如果控制台工作流具有多个启动节点/分支或浮动活动，则需要添加启动活动和分支，以将启动节点连接到主节点。 您还需要删除浮动活动。

**活动定位**

* 仅当添加或删除了活动时（并非始终如此），才会重新计算节点的位置（因此将修改活动的初始位置）。

**未公开选项**

* 不兼容的选项不会显示在Web UI中。

**循环**

* 在Web UI中，循环尚不可用。 如果您使用控制台创建了包含循环的工作流，则无法在Web UI中访问该工作流。 将显示一条错误消息。

| 控制台 | Web UI |
| --- | --- |
| ![](assets/limitations-loops-console.png) | ![](assets/limitations-loops-web.png) |

**协调与扩充**

在Campaign客户端控制台中， **扩充** 活动可以执行协调和扩充。 在Campaign Web UI中，协调功能尚不可用。 如果您在控制台活动中设置了协调，则在Web UI中，它将显示为不兼容的活动。

* 如果 **扩充** 控制台中的活动仅执行扩充，即 **扩充** 活动会显示在Web中。
* 如果 **扩充** 控制台中的活动仅执行协调，会显示不兼容的活动。

## 预定义过滤器 {#filters-guardrails-limitations}

在选择投放的受众或在工作流中构建受众时，某些预定义过滤器在该版本产品的用户界面中不可用。

此时会显示特定的错误消息。 即使无法在规则生成器中查看查询的图形表示形式，也无法编辑筛选器，您仍可以使用它，并查看筛选条件和结果。 您还可以访问SQL查询以检查确切的设置。

![](assets/filter-unavailable.png){width="70%" align="left"}


请注意，如果在Web界面中构建过滤器，并在控制台中使用不支持的属性对其进行修改，则在Web界面中无法再使用该图形表示。 无论如何，您仍可以使用过滤器。

下面列出了不支持的属性。

### 不支持的数据类型 {#unsupported-data-type}

在Web界面中显示过滤器或规则时，不支持客户端控制台中可用的以下数据类型：

* 日期时间
* 时间
* 时间跨度
* 多次
* 浮点数

### 不支持的筛选功能 {#unsupported-filtering-capabilities}

在客户端控制台中使用复杂的表达式和函数构建过滤器时，无法在Web界面中对其进行编辑。

此外，不支持以下运算符：

* 数值类型
   * 包含在
   * no in

* 字符串类型
   * 大于
   * 小于
   * 大于或等于
   * 小于或等于
   * 点赞
   * 不相似

* 日期类型
   * 在或晚于
   * 在或早于
   * 不等于
   * 为空
   * 不为空
   * 包含在
   * 不在
   * 最近

* 1-N链接
   * COUNT， SUM， AVG， MIN， MAX