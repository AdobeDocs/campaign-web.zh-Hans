---
audience: end-user
title: 使用重复数据删除工作流活动
description: 了解如何使用重复数据删除工作流活动
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 7%

---


# 重复数据删除 {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->

此 **删除重复项** 活动是 **定位** 活动。 利用此活动，可删除集客活动结果中的重复项。 此 **删除重复项** 活动通常用在定向活动之后、允许使用定向数据的活动之前。

## 配置

按照以下步骤配置 **计划程序** 活动：

1. 添加 **删除重复项** 活动添加到工作流。

   ![](../assets/workflow-deduplication.png)

1. 在 **用于标识重复项的字段** 部分，单击 **添加属性** 按钮来指定允许识别重复项的相同值的字段：电子邮件地址、名字、姓氏等。 利用字段的顺序，可指定要先处理的字段。

1. 选择唯一数量 **要保留的重复项**. 此字段的默认值为 1。使用 0 值，可保留所有重复项。

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. 选择 **去重方法** 要使用：

   * **随机选择**：随机选择要保留的重复项记录。
   * **使用表达式**：利用此选项可保留输入表达式的值最小或最大的记录。 ++表达式++排序
   * **遵循值列表**：用于为一个或多个字段定义值优先级。 要定义值，请单击 **属性** 以选择字段或创建表达式，然后将值添加到相应的表中。 要定义新字段，请单击位于值列表上方的“添加”按钮。 ++ 排序

1. 查看 **生成补码** 选项。 补充包含所有重复项。 然后，将向该活动添加其他过渡。

## 示例

