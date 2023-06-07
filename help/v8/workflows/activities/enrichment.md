---
audience: end-user
title: 使用扩充工作流活动
description: 了解如何使用扩充工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 28%

---


# 扩充 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="扩充活动"
>abstract="扩充活动可让您使用数据库中的其他信息来增强目标数据。它通常用在定向活动后的工作流中。<br/>在将扩充数据添加到工作流中后，可以在扩充活动后添加的活动中使用它，以根据客户的行为、偏好和需求来将客户分成不同的组，或者创建更可能让目标受众产生共鸣的个性化营销邮件和营销活动。"

此 **扩充** 活动是 **定位** 活动。 它允许您使用数据库中的其他信息增强目标数据。 它通常用在分段活动之后的工作流中。

扩充数据可来自：

* **同一个工作表**，此工作表与工作流中的目标工作表相同：

   *定位一组客户，并将“出生日期”字段添加到当前工作表*

* **另一个工作表**：

   *定位一组客户，并添加“采购”表中的“金额”和“产品类型”字段*。

将扩充数据添加到工作流后，便可在之后添加的活动中使用它 **扩充** 根据客户的行为、偏好和需求将客户划分为不同的群组的活动，或者创建更可能引起目标受众共鸣的个性化营销消息和促销活动。

例如，可以将与客户购买相关的信息添加到工作流工作表中，并使用此数据来个性化包含客户最近一次购买或在这些购买中花费的金额的电子邮件。

## 常规配置

按照以下步骤配置 **扩充** 活动：

1. 添加活动，例如 **构建受众** 和 **合并** 活动。
1. 添加 **扩充** 活动。
1. 单击 **添加扩充数据**.

![](../assets/workflow-enrichment1.png)

您可以选择两种类型的数据：目标维中的单个属性或集合链接。

## 单个属性

这里，我们只是添加一个扩充属性，例如，出生日期。 执行以下步骤：

1. 在 **属性** 字段。
1. 从定向维度中选择一个简单字段，在我们的示例中是出生日期。
1. 单击&#x200B;**确认**。

![](../assets/workflow-enrichment2.png)

## 收藏集链接

在这个更复杂的用例中，我们将选择一个收藏集链接，该链接是表之间具有1-N基数的链接。 让我们检索三个小于100美元的最新购买数据。 为此，您需要定义：

* 属性： **总金额** 字段
* 要检索的行数：3
* 过滤器：过滤掉大于100$的项
* a sorting： descendant sorting on **订单日期** 字段。

执行以下步骤：

### 添加属性

您可以在此处选择收集链接以用作扩充数据。

1. 在 **属性** 字段。
1. 单击 **显示高级属性**.
1. 选择 **总金额** 中的字段 **购买** 表格。

![](../assets/workflow-enrichment3.png)

### 定义收藏集设置

然后，定义如何收集数据以及要检索的记录数。

1. 选择 **收集数据** 在 **选择收集数据的方式** 下拉菜单。
1. 在“ ”中键入“3” **要检索的行（要创建的列）** 字段。

![](../assets/workflow-enrichment4.png)

例如，如果要获取客户的平均购买量，请选择 **聚合数据** 相反，并选择 **Average** 在 **聚合函数** 下拉菜单。

![](../assets/workflow-enrichment5.png)

### 定义过滤器

在本例中，我们定义了属性的最大值。 我们筛选掉大于100$的项目。

1. 单击 **编辑筛选器**.
1. 添加以下两个过滤器： **总金额** 存在和 **总金额** 小于100。 第一个筛选器筛选NULL值，因为它们显示为最大值。
1. 单击&#x200B;**确认**。

![](../assets/workflow-enrichment6.png)

### 定义排序

现在，我们需要应用排序以检索这三个 **最新** 购买。

1. 激活 **启用排序** 选项。
1. 在 **属性** 字段。
1. 选择 **订单日期** 字段。
1. 单击&#x200B;**确认**。
1. 选择 **降序** 从 **排序** 下拉菜单。

![](../assets/workflow-enrichment7.png)

<!--
cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->