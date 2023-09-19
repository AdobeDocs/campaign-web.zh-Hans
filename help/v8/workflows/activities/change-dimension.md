---
audience: end-user
title: 使用更改维度工作流活动
description: 了解如何使用更改维度工作流活动
badge: label="Beta"
source-git-commit: fb144e4b7186717dd0c4049d8ce884998a1adefe
workflow-type: tm+mt
source-wordcount: '296'
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

此 **更改维度** 活动是 **定位** 活动。 利用此活动，可在构建工作流时更改定向维度。 它根据数据模板和输入维度移动轴。 [了解有关定位维度的更多信息](../../audience/about-recipients.md#targeting-dimensions)

例如，您可以将工作流的定向维度从“收件人”切换为“订阅者应用程序”，以便向定向收件人发送推送通知。

## 配置更改维度活动 {#configure}

按照以下步骤配置 **更改维度** 活动：

1. 添加 **更改维度** 活动添加到工作流。

   ![](../assets/workflow-change-dimension.png)

1. 定义 **新建目标维度**. 在维度更改期间，将保留所有记录。 其他选项尚不可用。

1. 执行工作流以查看结果。 比较变更维活动之前和之后的表中的数据，并比较工作流表的结构。

## 示例 {#example}

在本例中，我们希望向所有已购买的用户档案发送短信投放。 为此，我们首先使用 **[!UICONTROL 构建受众]** 链接到自定义“购买”定向维度的活动，以定向发生的所有购买。

然后使用 **[!UICONTROL 更改维度]** 活动以将工作流定向维度切换到“收件人”。 这样，我们便能够定位匹配查询的收件人。

![](../assets/workflow-change-dimension-example.png)
