---
audience: end-user
title: 使用“AND-连接工作流”活动
description: 了解如何使用“AND-连接工作流”活动
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 100%

---

# AND-连接 {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join 活动"
>abstract="利用 **And-join** 活动，可同步工作流的多个执行分支。一旦完成所有之前的活动，即触发该活动。这使您能够在继续执行工作流之前确保某些活动已完成。"

**AND-连接**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。利用此活动，可同步工作流的多个执行分支。

一旦激活所有集客过渡，换言之，一旦完成所有先行工作，此活动就会触发其所有叫客过渡。这使您可以在继续执行工作流之前确保某些活动已完成。

## 配置 AND-join 活动{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="配置 AND-join 活动"
>abstract="选择您要参加的活动。在&#x200B;**主要集合**&#x200B;下拉列表中，选择要保留的集客过渡群体。"

请按照以下步骤操作，配置 **AND-连接**&#x200B;活动：

![](../assets/workflow-andjoin.png)

1. 添加多项活动（例如渠道活动），来构成至少两个不同的执行分支。
1. 向任何分支添加一个 **AND-连接**&#x200B;活动。
1. 在&#x200B;**合并选项**&#x200B;部分中，选中您之前希望加入的所有活动。
1. 在&#x200B;**主集**&#x200B;下拉列表中，选择您要保留的集客过渡群体。叫客过渡只能包含集客过渡群体之一。

## 示例{#and-join-example}

以下示例显示了两个工作流分支，其中包含电子邮件和短信投放。当两个集客过渡均启用时，将触发 AND-连接。只有在两次投放完成后才会发送推送通知。

![](../assets/workflow-andjoin-example.png){zoomable=&quot;yes&quot;}
