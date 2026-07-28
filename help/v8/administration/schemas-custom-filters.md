---
title: 添加自定义筛选条件
description: 了解如何在列表视图的筛选器窗格中将自定义筛选器添加为快速访问字段。
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# 添加自定义筛选条件 {#custom-filters}

**[!UICONTROL 清单列表配置]** > **[!UICONTROL 自定义筛选器]**&#x200B;部分允许您选择在架构列表视图的[筛选器窗格](../query/filter.md)中，在&#x200B;**[!UICONTROL 高级筛选器]**&#x200B;规则生成器上方将哪些属性显示为快速访问字段。

有关屏幕定义屏幕以及如何对其进行访问的更多信息，请参阅[访问屏幕定义](schemas-browse-access.md#screen-def)部分。

## 添加自定义筛选条件 {#add}

1. 浏览到&#x200B;**[!UICONTROL 架构]**&#x200B;菜单，并使用筛选器找到可编辑的架构。

1. 选择列表中的架构名称以将其打开，然后单击架构详细信息视图中的&#x200B;**[!UICONTROL 屏幕版本]**&#x200B;按钮以访问屏幕定义。

1. 转到&#x200B;**[!UICONTROL 清单列表配置]**&#x200B;部分，单击&#x200B;**[!UICONTROL 自定义筛选器]**&#x200B;表上方的省略号图标，然后选择&#x200B;**[!UICONTROL 选择属性]**。

   ![自定义筛选器选择](assets/schemas-custom-filters1.png)

1. 选择一个或多个属性并进行确认。

   您可以选择：

   * 模式的直接属性，例如代码或类别。
   * 链接属性，例如链接到产品的品牌。 在这种情况下，过滤器使用仅限于链接架构的搜索选取器。
   * 链接的子属性，例如链接文件夹的全名或链接收件人的电子邮件。

   ![属性选取器显示直接属性和链接子属性](assets/schemas-custom-filters2.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。 您可以使用上下箭头或拖动自定过滤器来重新排序它们，并使用行上的垃圾桶图标删除过滤器。

1. 浏览到此架构的记录列表，并打开筛选器窗格。 在&#x200B;**[!UICONTROL 高级筛选器]**&#x200B;规则生成器的上方，您选择的属性显示为&#x200B;**[!UICONTROL 自定义筛选器]**。

   ![自定义筛选器显示在筛选器窗格中](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >基于日期或日期和时间属性的自定义筛选器将显示为日期范围选取器。

1. 在其中一个自定义筛选器中输入或选择一个值以优化列表。

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->