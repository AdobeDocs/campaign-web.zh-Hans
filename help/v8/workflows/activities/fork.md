---
audience: end-user
title: 使用“分叉工作流”活动
description: 了解如何使用“分叉工作流”活动
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 100%

---


# 分叉 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分叉活动"
>abstract="利用分叉活动，可创建叫客过渡以同时开始多个活动。"

利用分叉活动，可创建叫客过渡以同时开始多个活动。

## 配置

请按照以下步骤操作，配置&#x200B;**分叉**&#x200B;活动：

1. 向您的工作流添加一个&#x200B;**分叉**&#x200B;活动。
1. 单击&#x200B;**添加过渡**&#x200B;以添加新的叫客过渡。默认情况下会定义两个过渡。
1. 请为每个过渡添加标签。

## 示例

在下面的示例中，我们使用两个&#x200B;**分叉**&#x200B;活动：

* 在两个查询之前使用一个分叉活动，同时执行这两个查询。
* 在交集之后使用一个分叉活动，同时向目标群体发送一封电子邮件和一条短信。

![](../assets/workflow-fork-example.png)

