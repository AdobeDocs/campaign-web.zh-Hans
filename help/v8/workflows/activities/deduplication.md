---
audience: end-user
title: 使用重复数据删除工作流活动
description: 了解如何使用重复数据删除工作流活动
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 50%

---

# 重复数据删除 {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="用于识别重复项的字段"
>abstract="在&#x200B;**用于识别重复项的字段**&#x200B;部分中，单击&#x200B;**添加属性&#x200B;**&#x200B;按钮以指定允许将相同值视为重复的字段，如电子邮件地址、名字、姓氏等。栏位的顺序可让您指定首要处理的条件。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="删除重复项活动"
>abstract="删除&#x200B;**重复项活动可让您删除**&#x200B;入站活动结果中的重复项。主要在目标市场选择活动之后且在允许使用目标数据的活动之前使用。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="生成补集"
>abstract="可使用剩余群体（已排除的重复项）生成额外的出站过渡。为此，请打开生成补集选项为此，请打开&#x200B;**生成补集**&#x200B;选项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="重复数据删除设置"
>abstract="要删除传入数据中的重复项，请在以下字段中定义删除重复项方法。默认情况下，只会保留一条记录。您还应该根据表达式或属性选择删除重复项模式。默认情况下，要避免重复的记录是随机选择的。"

**重复数据删除**&#x200B;活动是&#x200B;**定位**&#x200B;活动。 利用此活动，可删除集客活动结果中的重复项，例如收件人列表中重复的用户档案。 **重复数据删除**&#x200B;活动通常用在定向活动之后，以及允许使用定向数据的活动之前。

## 配置重复数据删除活动{#deduplication-configuration}

按照以下步骤配置&#x200B;**重复数据删除**&#x200B;活动：

![](../assets/workflow-deduplication.png)

1. 向工作流添加&#x200B;**重复数据删除**&#x200B;活动。

1. 在&#x200B;**用于识别重复项的字段**&#x200B;部分中，单击&#x200B;**添加属性&#x200B;**&#x200B;按钮以指定允许将相同值视为重复的字段，如电子邮件地址、名字、姓氏等。利用字段的顺序，可指定要先处理的字段。 [了解如何选择属性并将其添加到收藏夹](../../get-started/attributes.md)

1. 在&#x200B;**重复数据删除设置**&#x200B;部分中，选择要保留的唯一&#x200B;**重复项数**。 此字段的默认值为 1。使用 0 值，可保留所有重复项。

   例如，如果记录 A 和 B 被视为记录 Y 的重复项，而记录 C 被视为记录 Z 的重复项：

   * 如果字段的值为 1：只保留 Y 和 Z 记录。
   * 如果字段的值为 0：保留所有记录。
   * 如果字段的值为 2：保留 C 和 Z 记录，并保留 A、B 和 Y 中的两个记录，具体情况取决于此后选择的重复数据删除方法。

1. 选择要使用的&#x200B;**重复数据删除方法**：

   * **随机选择**：随机选择要保留的重复项记录。
   * **使用表达式**：保留输入表达式的值最小或最大的记录。
   * **非空值**：保留表达式不为空的记录。
   * **遵循值列表**：为一个或多个字段定义值优先级。 若要定义值，请单击&#x200B;**属性**&#x200B;以选择一个字段或创建表达式，然后将值添加到相应的表中。 要定义新字段，请单击位于值列表上方的&#x200B;**添加按钮**。

1. 如果要利用剩余群体，请选中&#x200B;**生成补码**&#x200B;选项。 补充包含所有重复项。 然后，将向该活动添加其他过渡。

## 示例{#deduplication-example}

在以下示例中，使用重复数据删除活动，在发送投放之前从目标中排除重复项。 识别的重复用户档案将添加到专用受众，如有必要，可以重复使用。 选择&#x200B;**电子邮件**&#x200B;地址以标识重复项。 保留1个条目并选择&#x200B;**随机**&#x200B;重复数据删除方法。

![](../assets/workflow-deduplication-example.png)
