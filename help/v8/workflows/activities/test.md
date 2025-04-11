---
audience: end-user
title: 使用测试工作流活动
description: 了解如何使用测试工作流活动
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 35%

---


# 测试 {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="”测试“活动"
>abstract="**测试**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。它允许您根据指定条件启用过渡。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="条件"
>abstract="**测试**&#x200B;活动可以有多个输出过渡。在执行工作流期间，将会按顺序测试每个条件，直到满足其中一个条件。如果没有满足任何条件，工作流程会沿着&#x200B;**[!UICONTROL 默认条件]**&#x200B;路径继续。如果没有激活默认条件，工作流会在此时停止。"

**测试**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。它允许您根据指定条件启用过渡。

## 配置测试活动 {#test-configuration}

按照以下步骤配置&#x200B;**测试**&#x200B;活动：

1. 将&#x200B;**测试**&#x200B;活动添加到您的工作流。

1. 默认情况下，**[!UICONTROL Test]**&#x200B;活动提供简单的布尔测试。 如果满足“True”过渡中定义的条件，则会激活此过渡。 否则，将激活默认的“False”过渡。

1. 要配置与过渡关联的条件，请单击&#x200B;**[!UICONTROL 打开个性化对话框]**&#x200B;图标。 使用表达式编辑器定义激活此过渡所需的规则。 您还可以使用事件变量、条件和日期/时间函数。 [了解如何使用事件变量和表达式编辑器](../event-variables.md)。

   此外，请修改&#x200B;**[!UICONTROL 标签]**&#x200B;字段以个性化工作流画布上的过渡名称。

   ![测试活动的默认配置](../assets/workflow-test-default.png)

1. 向&#x200B;**[!UICONTROL Test]**&#x200B;活动添加多个输出转换。 为此，请单击&#x200B;**[!UICONTROL 添加条件]**&#x200B;按钮，并为每个过渡配置标签和相关条件。

1. 在执行工作流期间，将会按顺序测试每个条件，直到满足其中一个条件。如果没有满足任何条件，工作流程会沿着&#x200B;**[!UICONTROL 默认条件]**&#x200B;路径继续。如果没有激活默认条件，工作流会在此时停止。

## 示例 {#example}

在此示例中，根据&#x200B;**[!UICONTROL 构建受众]**&#x200B;活动定向的用户档案数激活不同的过渡：
* 如果定向的用户档案超过10,000个，则会发送电子邮件。
* 对于1,000到10,000个用户档案，将发送短信。
* 如果目标用户档案低于1,000，则会被定向到“请勿联系”过渡。

![测试活动过渡示例](../assets/workflow-test-example.png)

为实现此目的，`vars.recCount`事件变量用在“电子邮件”和“短信”条件中，以计算目标用户档案的数量并激活相应的过渡。

![测试活动示例的配置](../assets/workflow-test-example-config.png)
