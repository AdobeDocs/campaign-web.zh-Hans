---
audience: end-user
title: 使用“等待工作流”活动
description: 了解如何使用“等待工作流”活动
badge: label="有限发布版"
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: 023777b88fa5c80e110fcf334517f7cef1c7f1ee
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 92%

---

# 等待 {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="等待活动"
>abstract="**等待**&#x200B;活动用于将过渡从一个活动推迟另一个活动。"

**等待**&#x200B;活动是&#x200B;**流量控制**&#x200B;活动。它可为两个执行的活动之间添加一段等待的时间。例如，在执行电子邮件投放活动后，等待几天，再分析这期间产生的打开次数和点击次数，然后再执行所有后续操作（提醒电子邮件、创建受众等）。

## 配置{#wait-configuration}

请按照以下步骤操作，配置&#x200B;**等待**&#x200B;活动：

1. 向您的工作流添加一个&#x200B;**等待**&#x200B;活动。

1. 指定集客过渡和叫客过渡之间等待的&#x200B;**持续时间**。

1. 选择时间单位 **期间** 字段：秒、分钟、小时、天。

## 示例{#wait-example}

下面的示例展示了典型用例中的&#x200B;**等待**&#x200B;活动。发送某个活动的电子邮件邀请。发送邀请 24 小时后，短信投放会发送给同一群体。

![](../assets/workflow-wait-example.png)
