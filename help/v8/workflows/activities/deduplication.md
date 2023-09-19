---
audience: end-user
title: 使用重复数据删除工作流活动
description: 了解如何使用重复数据删除工作流活动
badge: label="Beta"
source-git-commit: 1f23eafc80e21b63485a774fd9052c8d03051685
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 4%

---


# 重复数据删除 {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="重复数据删除属性"
>abstract="这允许您指定允许识别重复项的相同值的字段：电子邮件地址、名字、姓氏等。 利用字段的顺序，可指定要先处理的字段。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="重复数据删除活动"
>abstract="此 **删除重复项** 利用活动，可删除集客活动结果中的重复项。 它主要用于定向活动之后，以及允许使用定向数据的活动之前。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="生成补码"
>abstract="您可以使用已作为重复项排除的剩余群体生成额外的叫客过渡。 为此，请打开 **生成补码** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="删除重复项设置"
>abstract="要删除传入数据中的重复项，请在以下字段中定义重复数据删除方法。 默认情况下，只保留一个记录。 您还应根据表达式或属性选择重复数据删除模式。 默认情况下，将随机选择要排除在重复项之外的记录。"

此 **删除重复项** 活动是 **定位** 活动。 利用此活动，可删除集客活动结果中的重复项。 此 **删除重复项** 活动通常用在定向活动之后、允许使用定向数据的活动之前。

## 配置重复数据删除活动{#deduplication-configuration}

按照以下步骤配置 **删除重复项** 活动：

![](../assets/workflow-deduplication.png)

1. 添加 **删除重复项** 活动添加到工作流。

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
   * **使用表达式**：利用此选项可保留输入表达式的值最小或最大的记录。
   * **遵循值列表**：用于为一个或多个字段定义值优先级。 要定义值，请单击 **属性** 以选择字段或创建表达式，然后将值添加到相应的表中。 要定义新字段，请单击位于值列表上方的“添加”按钮。

1. 查看 **生成补码** 选项。 补充包含所有重复项。 然后，将向该活动添加其他过渡。

## 示例{#example}

在以下示例中，我们使用重复数据删除活动，在发送投放之前从目标中排除重复项。 标识的重复项会添加到专用的重复项受众中，如有必要，可以重复使用。 我们使用 **电子邮件** 用于标识重复项的字段。 我们选择保留1个条目，然后选择 **Random** 删除重复项方法。

![](../assets/workflow-deduplication-example.png)
