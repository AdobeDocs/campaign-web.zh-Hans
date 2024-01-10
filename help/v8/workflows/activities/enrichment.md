---
audience: end-user
title: 使用“扩充工作流”活动
description: 了解如何使用“扩充工作流”活动
badge: label="有限发布版"
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: fb72b943b324990f6dd82a4a05bfd28e5452480a
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 81%

---

# 扩充 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="扩充活动"
>abstract="通过&#x200B;**扩充**&#x200B;活动，可利用来自数据库的其他信息增强目标数据。它通常用于分段活动之后的工作流中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="扩充活动"
>abstract="将扩充数据添加到工作流后，即可在扩充活动后添加的活动中使用它，以根据客户的行为、偏好和需求将客户分成不同的组，或创建更有可能让目标受众产生共鸣的个性化营销邮件和营销活动。"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="扩充数据"
>abstract="选择用于扩充您的工作流的数据。可选择两种类型的扩充数据：目标维度中的单个扩充属性或收藏集链接（即在各表之间具有 1-N 基数的链接）。"

**扩充**&#x200B;活动是一个&#x200B;**定位**&#x200B;活动。它可让您使用数据库中的其他信息来增强目标数据。它通常用于分段活动之后的工作流中。

扩充数据可来自：

* **同一个工作表**，此工作表与工作流中的目标工作表相同：

  *定位一组客户并将“出生日期”字段添加到当前工作表*.

* **另一个工作表**：

  *定位一组客户，并添加“采购”表中的“金额”和“产品类型”字段*。

将扩充数据添加到工作流后，便可用于在之后添加的活动 **扩充** 活动，根据客户的行为、偏好和需求将客户划分为不同的群组，或者创建更可能引起目标受众共鸣的个性化营销消息和营销活动。

例如，可以将与客户购买相关的信息添加到工作流工作表中，并使用此数据来个性化包含客户最近一次购买或在这些购买中花费的金额的电子邮件。

## 配置扩充活动 {#enrichment-configuration}

请按照以下步骤操作，配置&#x200B;**扩充**&#x200B;活动：

1. 添加活动，例如&#x200B;**生成受众**&#x200B;和&#x200B;**合并**&#x200B;活动。
1. 添加&#x200B;**扩充**&#x200B;活动。
1. 单击 **添加扩充数据** 并选择要用于扩充数据的属性。

   您可以选择两种类型的扩充数据：目标维度中的[单个扩充属性](#single-attribute)，或[收藏集链接](#collection-link)。

   >[!NOTE]
   >
   >此 **“编辑表达式”按钮** 在属性选择屏幕中，您可以构建高级表达式以选择属性。 [了解如何使用表达式编辑器](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## 单个扩充属性 {#single-attribute}

我们在此处只添加单个扩充属性，例如出生日期。执行以下步骤：

1. 在&#x200B;**属性**&#x200B;字段内单击。
1. 从定位维度中选择一个简单的字段，在我们的示例中是出生日期。
1. 单击&#x200B;**确认**。

![](../assets/workflow-enrichment2.png)

## 收藏集链接 {#collection-link}

在这个更复杂的用例中，我们将选择一个收藏集链接，它是表之间具有 1 对多基数的链接。让我们检索最近三笔低于 100 美元的购买。为此，您需要定义：

* 扩充属性：**总金额**&#x200B;字段
* 要检索的行数：3
* 筛选条件：筛选掉大于 100 美元的项目
* 排序：**订购日期**&#x200B;字段的降序排序。

### 添加属性 {#add-attribute}

您可以在此处选择用作扩充数据的收藏集链接。

1. 在&#x200B;**属性**&#x200B;字段内单击。
1. 单击&#x200B;**显示高级属性**。
1. 从&#x200B;**购买**&#x200B;表中选择&#x200B;**总金额**&#x200B;字段。

![](../assets/workflow-enrichment3.png)

### 定义收藏集设置{#collection-settings}

然后，定义数据的收集方式以及要检索的记录数。

1. 在&#x200B;**选择数据收集方式**&#x200B;下拉列表中选择&#x200B;**收集数据**。
1. 在&#x200B;**要检索的行（要创建的列）**&#x200B;字段中键入“3”。

![](../assets/workflow-enrichment4.png)

例如，如果您想要获取客户的平均购买金额，请改选&#x200B;**汇总数据**，然后从&#x200B;**汇总函数**&#x200B;中选择&#x200B;**平均**。

![](../assets/workflow-enrichment5.png)

### 定义筛选条件{#collection-filters}

我们在此处定义扩充属性的最大值。我们将筛选掉大于100$的项目。 [了解如何使用查询建模器](../../query/query-modeler-overview.md)

1. 单击&#x200B;**编辑筛选条件**。
1. 添加以下两个筛选条件：**总金额**&#x200B;存在且&#x200B;**总金额**&#x200B;小于 100。第一个筛选条件筛选掉 NULL 值，因为它们将显示为最大值。
1. 单击&#x200B;**确认**。

![](../assets/workflow-enrichment6.png)

### 定义排序{#collection-sorting}

我们现在需要应用排序来检索这三个&#x200B;**最新**&#x200B;的购买。

1. 激活&#x200B;**启用排序**&#x200B;选项。
1. 在&#x200B;**属性**&#x200B;字段内单击。
1. 选择&#x200B;**订购日期**&#x200B;字段。
1. 单击&#x200B;**确认**。
1. 从&#x200B;**排序**&#x200B;下拉列表中选择&#x200B;**降序**。

![](../assets/workflow-enrichment7.png)

<!--

Add other fields
use it in delivery


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
