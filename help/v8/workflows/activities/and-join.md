---
audience: end-user
title: 使用AND-join工作流活动
description: 了解如何使用“与”连接工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 4%

---


# AND-连接 {#join}

此 **And — 连接** 利用活动，可同步工作流的多个执行分支。

只有在所有集客过渡激活后（换言之，在所有先行活动完成后），合并联接活动才会触发其叫客过渡。

按照以下步骤配置 **AND — 连接** 活动：

1. 添加多个活动，例如 **合并** 活动，以至少形成两个不同的执行分支。
1. 添加 **AND — 连接** 活动到任何分支。
1. 在 **合并选项** 部分，检查您之前希望加入的所有活动。
1. 选择 **主集** 保留在叫客过渡中。
