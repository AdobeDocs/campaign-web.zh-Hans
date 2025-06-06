---
audience: end-user
title: 使用更改维度工作流活动
description: 了解如何使用更改维度工作流活动
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 25%

---

# 更改维度 {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="生成补集"
>abstract="可使用剩余群体（已排除的重复项）生成额外的出站过渡。为此，请打开生成补集选项为此，请打开&#x200B;**生成补集**&#x200B;选项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="更改维度活动"
>abstract="通过此活动，可在生成受众时更改定位维度。它根据数据模板和输入维度移动轴。例如，您可以从“合同”维度切换到“客户”维度。"

**更改维度**&#x200B;活动是&#x200B;**定位**&#x200B;活动。 利用此活动，可在构建工作流时更改定向维度。 它根据数据模板和输入维度移动轴。[了解有关定向维度的更多信息](../../audience/about-recipients.md#targeting-dimensions)。

例如，您可以将工作流的定向维度从“收件人”切换为“订阅者应用程序”，以向定向收件人发送推送通知。

>[!IMPORTANT]
>
>请注意，不应将&#x200B;**[!UICONTROL 更改维度]**&#x200B;和&#x200B;**[!UICONTROL 更改数据源]**&#x200B;活动添加到一行中。 如果需要连续使用这两个活动，请在它们之间包含&#x200B;**[!UICONTROL 扩充]**&#x200B;活动。 这可以确保正确执行并防止潜在的冲突或错误。

## 配置更改维度活动 {#configure}

按照以下步骤配置&#x200B;**更改维度**&#x200B;活动：

1. 将&#x200B;**更改维度**&#x200B;活动添加到您的工作流。

   ![显示添加到工作流的“更改”维度活动的屏幕截图](../assets/workflow-change-dimension.png)

1. 定义&#x200B;**新目标维度**。 在维度更改期间，将保留所有记录。 其他选项尚不可用。

1. 执行工作流以查看结果。 比较变更维活动之前和之后的表中的数据，并比较工作流表的结构。

## 示例 {#example}

在本例中，向已购买的所有用户档案发送短信投放。 首先，使用链接到自定义“购买”定向维度的&#x200B;**[!UICONTROL 构建受众]**&#x200B;活动来定向发生的所有购买。

然后，使用&#x200B;**[!UICONTROL 更改维度]**&#x200B;活动将工作流定向维度切换为“收件人”。 这允许定向匹配查询的收件人。

![显示工作流中使用的“更改”维度活动示例的屏幕截图](../assets/workflow-change-dimension-example.png)