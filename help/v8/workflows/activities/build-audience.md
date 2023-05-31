---
audience: end-user
title: 使用构建受众工作流活动
description: 了解如何使用构建受众工作流活动
badge: label="Alpha" type="Positive"
source-git-commit: 4c0157c0457d1d6fa3194463adef8572017af8f0
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 16%

---


# 构建受众 {#build-audience}

此活动允许您定义受众。 您可以选择现有受众，也可以使用规则生成器定义您自己的查询。

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

按照以下步骤配置 **构建受众** 活动：

1. 添加构建受众活动。
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
