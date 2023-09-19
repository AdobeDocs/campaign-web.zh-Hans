---
audience: end-user
title: 使用更改维度工作流活动
description: 了解如何使用更改维度工作流活动
badge: label="Beta"
source-git-commit: 8139ec2f1e94bebacd89ea64af88d0b0babb8781
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---


# 更改维度 {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="生成补码"
>abstract="您可以使用已作为重复项排除的剩余群体生成额外的叫客过渡。 为此，请打开 **生成补码** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="更改维度活动"
>abstract="利用此活动，可在构建受众时更改定向维度。 它根据数据模板和输入维度移动轴。 例如，您可以从“合同”维度切换到“客户”维度。"

此 **更改维度** 活动是 **定位** 活动。 利用此活动，可在构建受众时更改定向维度。 此活动根据数据模板和输入维度移动轴。 例如，您可以从“合同”维度切换到“客户”维度。

## 配置更改维度活动 {#configure}

按照以下步骤配置 **更改维度** 活动：

1. 添加 **更改维度** 活动添加到工作流。

   ![](../assets/workflow-change-dimension.png)

1. 定义 **新建目标维度**. 在维度更改期间，将保留所有记录。 其他选项尚不可用。

1. 执行工作流以查看结果。 比较变更维活动之前和之后的表中的数据，并比较工作流表的结构。

## 示例 {#example}


