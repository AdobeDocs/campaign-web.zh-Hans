---
audience: end-user
title: 使用“生成受众”工作流活动
description: 了解如何使用“生成受众”工作流活动
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 100%

---


# 生成受众 {#build-audience}

**生成受众**&#x200B;活动是一个&#x200B;**定位**&#x200B;活动。此活动允许您定义将输入工作流的受众。在营销活动工作流的上下文中发送消息时，消息受众不是在渠道活动中定义的，而是在&#x200B;**生成受众**&#x200B;活动中定义的。

要定义受众群体，您可以：

* 选择现有受众，并在客户端控制台中将其创建为列表。
* 选择 Adobe Experience Platform 受众。
* 通过定义和组合筛选条件，使用规则生成器生成新受众。

>[!NOTE]
>
>在此上下文中，您无法从文件加载受众。为此，需要创建独立投放。[了解详情](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 配置

请按照以下步骤配置&#x200B;**生成受众**&#x200B;活动：

1. 添加一个&#x200B;**生成受众**&#x200B;活动。
1. 定义一个标签。
1. 定义受众类型：**创建您自己的**&#x200B;或&#x200B;**读取受众**。

要创建您自己的查询，请额外执行以下步骤：

1. 选择&#x200B;**创建您自己的（查询）**。
1. 选择&#x200B;**定位维度**。定位维度可让您定义操作的目标人群：收件人、合同受益人、操作人员、订阅者等。默认情况下，目标是从收件人中选择的。请参阅 [v8 文档](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}。
1. 单击&#x200B;**继续**。
1. 使用规则生成器定义您的查询，就像设计新电子邮件时创建受众的方式一样。请参阅此[章节](../../audience/segment-builder.md)。

要选择现有受众，请执行以下步骤：

1. 选择&#x200B;**读取受众**。
1. 单击&#x200B;**继续**。
1. 选择您的受众，就像设计新电子邮件时使用受众一样。请参阅此[章节](../../audience/add-audience.md)。

## 示例

此工作流程示例包含两个&#x200B;**生成受众**&#x200B;活动。第一个示例针对扑克玩家受众，然后是电子邮件投放。第二个示例针对 VIP 客户受众，然后是短信投放。

![](../assets/workflow-audience-example.png)