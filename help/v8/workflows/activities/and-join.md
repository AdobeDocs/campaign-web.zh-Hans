---
audience: end-user
title: 使用“AND-连接工作流”活动
description: 了解如何使用“AND-连接工作流”活动
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 50%

---

# AND-连接 {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="”AND-join“ 活动"
>abstract="利用 **And-join** 活动，可同步工作流的多个执行分支。一旦完成所有之前的活动，即会触发该活动。这可确保在继续执行工作流之前完成某些活动。"

**AND-连接**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。它同步工作流的多个执行分支。

只有在激活所有集客过渡后，此活动才会触发其集客过渡。 换句话说，一旦完成之前的所有活动，就会激活该活动。 这可确保在继续执行工作流之前已完成某些活动。

## 配置 AND-join 活动 {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="合并选项"
>abstract="选择您要参加的活动。在&#x200B;**主要集合**&#x200B;下拉列表中，选择要保留的集客过渡群体。"

请按照以下步骤操作，配置 **AND-连接**&#x200B;活动：

![显示AND-join活动的配置接口的屏幕截图。](../assets/workflow-andjoin.png)

1. 添加多个活动（如渠道活动）以形成至少两个不同的执行分支。
1. 向任何分支添加一个 **AND-连接**&#x200B;活动。
1. 在&#x200B;**合并选项**&#x200B;部分中，选中之前要加入的所有活动。
1. 在&#x200B;**主集**&#x200B;下拉列表中，选择要保留的集客过渡群体。 叫客过渡只能包含集客过渡群体之一。

## 示例 {#and-join-example}

以下示例显示了两个工作流分支，其中包含电子邮件和短信投放。在启用了两个集客过渡时，将触发AND-join。 推送通知仅在两个投放均完成后发送。

![具有两个分支的工作流示例，显示电子邮件和短信传递后跟推送通知。](../assets/workflow-andjoin-example.png){zoomable="yes"}