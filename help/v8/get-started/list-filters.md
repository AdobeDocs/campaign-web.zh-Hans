---
audience: end-user
title: 浏览、搜索和过滤列表
description: 探索如何浏览和过滤列表 Campaign Web v8
badge: label="Beta"
source-git-commit: 8612e29aa16bce609a822e42d15e2f92a6874383
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 86%

---


# 浏览、搜索和过滤列表 {#list-screens}

左侧导航菜单中的大多数链接显示对象列表，例如&#x200B;**投放**&#x200B;或&#x200B;**营销活动**&#x200B;的列表。其中一些列表屏幕为只读状态。您可以自定义列表显示，并过滤这些列表，如下详述。

要删除过滤器，请单击&#x200B;**全部清除**&#x200B;按钮。

## 自定义列表屏幕 {#custom-lists}

列表将以列的形式显示。可以更改列配置来显示其他信息。为此，请单击列表右上角的&#x200B;**为自定义版面配置列**&#x200B;图标。

![](assets/config-columns.png){width="70%" align="left" zoomable="yes"}

在&#x200B;**配置列**&#x200B;屏幕中，添加或删除列，并更改它们的显示顺序。

例如，对于这些设置：

![](assets/columns.png){width="70%" align="left" zoomable="yes"}

该列表显示以下列：

![](assets/column-sample.png){width="70%" align="left" zoomable="yes"}

使用&#x200B;**显示高级属性**&#x200B;开关以查看当前列表的所有属性。[了解详情](#adv-attributes)

## 对数据排序 {#sort-lists}

您也可以单击任意列标题来对列表中的项目进行排序。将显示一个箭头（向上或向下），指示列表已按该列排序。

对于数字或日期列，**向上**&#x200B;箭头表示列表按升序排序，**向下**&#x200B;箭头表示列表按降序排序。对于字符串或字母数字列，值将按字母顺序列出。

## 内置过滤器 {#list-built-in-filters}

要更快地找到项目，您可以使用搜索栏或按上下文条件过滤列表。

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

例如，您可以按状态、渠道、联系日期或文件夹过滤投放。您也可以隐藏测试。

## 自定义过滤器{#list-custom-filters}

要针对数据创建自定义过滤器，请浏览到过滤器底部，然后单击 **添加规则** 按钮以访问规则生成器。

拖放属性可在&#x200B;**高级过滤器**&#x200B;屏幕中生成筛选条件。

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

使用&#x200B;**显示高级属性**&#x200B;开关以查看当前列表的所有属性。[了解详情](#adv-attributes)

自定义筛选器的规则生成器的工作原理与创建受众所用的规则生成器类似。 有关如何使用该功能的详细信息，请参阅 [受众文档](../audience/segment-builder.md).

## 使用高级属性 {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="显示高级属性"
>abstract="默认情况下，属性列表中仅显示最常见属性。使用此切换可以查看高级属性。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="规则生成器高级字段"
>abstract="为高级过滤器配置高级字段。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="规则生成器高级属性"
>abstract="使用高级属性定义您的规则。"


默认情况下，属性列表和过滤器配置屏幕中仅显示最常见属性。配置屏幕中将隐藏设置为数据架构中的 `advanced` 属性的属性。

激活&#x200B;**显示高级属性**&#x200B;开关可查看当前列表的所有可用属性：将立即更新属性列表。


![](assets/adv-toggle.png){width="70%" align="left" zoomable="yes"}
