---
audience: end-user
title: 使用构建受众工作流活动
description: 了解如何使用构建受众工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 11%

---


# 构建受众 {#build-audience}

此 **构建受众** 活动是 **定位** 活动。 此活动允许您定义将进入工作流的受众。 在营销活动工作流的上下文中发送消息时，未在渠道活动中定义消息受众，但在渠道活动中 **构建受众** 活动。

要定义受众群体，您可以：

* 选择在客户端控制台中作为列表创建的现有受众。
* 选择Adobe Experience Platform受众。
* 通过定义和组合筛选条件，使用规则生成器构建新受众。

>[!NOTE]
>
>在此上下文中，您无法从文件加载受众。 为此，您需要创建一个独立的投放。 [了解详情](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 配置

按照以下步骤配置 **构建受众** 活动：

1. 添加 **构建受众** 活动。
1. 定义标签。
1. 定义受众类型： **创建您自己的** 或 **读取受众**.

要创建自己的查询，请按照以下额外步骤操作：

1. 选择 **创建您自己的（查询）**.
1. 选择 **定位维度**. 定位维度可让您定义操作的目标人群：收件人、合同受益人、操作人员、订阅者等。默认情况下，将从收件人中选择目标。 请参阅 [v8文档](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. 单击 **继续**.
1. 使用规则生成器定义查询，与设计新电子邮件时创建受众的方式相同。 请参阅此[章节](../../audience/segment-builder.md)。

要选择现有受众，请执行以下步骤：

1. 选择 **读取受众**.
1. 单击 **继续**.
1. 选择受众，与设计新电子邮件时使用受众的方式相同。 请参阅此[章节](../../audience/add-audience.md)。

## 示例

以下是包含两个工作流的工作流示例 **构建受众** 活动。 第一个目标是扑克玩家受众，然后是电子邮件投放。 第二个目标是VIP客户端受众，随后是短信投放。

![](../assets/workflow-audience-example.png)