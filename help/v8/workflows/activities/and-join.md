---
audience: end-user
title: 使用“AND-连接工作流”活动
description: 了解如何使用“AND-连接工作流”活动
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 94%

---


# AND-连接 {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND — 加入活动"
>abstract="**AND-连接**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。利用此活动，可同步工作流的多个执行分支。"



**AND-连接**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。利用此活动，可同步工作流的多个执行分支。

一旦激活所有集客过渡，换言之，一旦完成所有先行工作，此活动就会触发其所有叫客过渡。这使您可以在继续执行工作流之前确保某些活动已完成。

## 配置

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="配置AND — 连接活动"
>abstract="选择要加入的活动。 在&#x200B;**主集**&#x200B;下拉列表中，选择您要保留的集客过渡群体。"

请按照以下步骤操作，配置 **AND-连接**&#x200B;活动：

1. 添加多项活动（例如渠道活动），来构成至少两个不同的执行分支。
1. 向任何分支添加一个 **AND-连接**&#x200B;活动。
1. 在&#x200B;**合并选项**&#x200B;部分中，选中您之前希望加入的所有活动。
1. 在&#x200B;**主集**&#x200B;下拉列表中，选择您要保留的集客过渡群体。叫客过渡只能包含集客过渡群体之一。

## 示例

以下示例显示了两个工作流分支，其中包含电子邮件和短信投放。当两个集客过渡均启用时，将触发 AND-连接。只有在两次投放完成后才会发送推送通知。

![](../assets/workflow-andjoin-example.png)