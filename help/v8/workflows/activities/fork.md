---
audience: end-user
title: 使用“分叉工作流”活动
description: 了解如何使用“分叉工作流”活动
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 55%

---


# 分叉 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="分叉活动"
>abstract="利用&#x200B;**分叉**&#x200B;活动，可创建叫客过渡以同时开始多个活动。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分叉活动过渡"
>abstract="默认情况下，使用&#x200B;**分叉**&#x200B;活动创建两个过渡。单击&#x200B;**添加过渡**&#x200B;按钮以定义其他叫客过渡并输入其标签。"

**分叉**&#x200B;活动是一种&#x200B;**流量控制**&#x200B;活动。通过使用该功能，可创建叫客过渡以同时启动多个活动。

## 配置分支活动 {#fork-configuration}

请按照以下步骤操作，配置&#x200B;**分叉**&#x200B;活动：

![工作流分支活动配置屏幕截图](../assets/workflow-fork.png)

1. 向您的工作流添加一个&#x200B;**分叉**&#x200B;活动。
1. 单击&#x200B;**添加过渡**&#x200B;以添加新的叫客过渡。缺省情况下，定义了两个过渡。
1. 为每个过渡添加标签。

## 示例 {#fork-example}

在以下示例中，使用了两个&#x200B;**Fork**&#x200B;活动：

* 放在两个查询之前一个，以同时执行它们。
* 在交叉点后一个，同时向目标群体发送电子邮件和短信。

![工作流分支示例屏幕截图](../assets/workflow-fork-example.png)
