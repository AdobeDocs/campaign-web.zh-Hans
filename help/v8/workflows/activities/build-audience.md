---
audience: end-user
title: 使用“生成受众”工作流活动
description: 了解如何使用“生成受众”工作流活动
badge: label="有限发布版"
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: fb72b943b324990f6dd82a4a05bfd28e5452480a
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 61%

---

# 生成受众 {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="“构建受众”活动"
>abstract="通过&#x200B;**构建受众**&#x200B;活动，可定义将进入工作流的受众。在工作流的上下文中发送消息时，不在渠道活动中，而是在&#x200B;**构建受众**&#x200B;活动中定义消息受众。"

**生成受众**&#x200B;活动是一个&#x200B;**定位**&#x200B;活动。此活动允许您定义将输入工作流的受众。在工作流的上下文中发送消息时，不在渠道活动中，而是在&#x200B;**构建受众**&#x200B;活动中定义消息受众。

要定义受众群体，您可以：

* 选择现有受众，并在客户端控制台中将其创建为列表。
* 选择 Adobe Experience Platform 受众。
* 通过定义和组合筛选条件，使用查询建模器生成器构建新受众。

>[!NOTE]
>
>在此上下文中，您无法从文件加载受众。为此，您需要创建一个独立的电子邮件投放。 [了解详情](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 配置“构建受众”活动{#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="选择定位维度"
>abstract="定位维度可让您定义操作的目标人群：收件人、合同受益人、操作人员、订阅者等。默认情况下从收件人中选择目标。"

请按照以下步骤配置&#x200B;**生成受众**&#x200B;活动：

![](../assets/workflow-audience.png)

1. 添加一个&#x200B;**生成受众**&#x200B;活动。
1. 定义一个标签。
1. 定义受众类型：**创建您自己的**&#x200B;或&#x200B;**读取受众**。
1. 按照以下选项卡中详述的步骤配置受众。

>[!BEGINTABS]

>[!TAB 创建您自己的（查询）]

要创建自己的查询，请执行以下步骤：

1. 选择&#x200B;**创建您自己的（查询）**。
1. 选择&#x200B;**定位维度**。定位维度可让您定义操作的目标人群：收件人、合同受益人、操作人员、订阅者等。默认情况下，目标是从收件人中选择的。[了解有关定位维度的更多信息](../../audience/about-recipients.md#targeting-dimensions)
1. 单击&#x200B;**继续**。
1. 使用查询建模器定义查询，与设计新电子邮件时创建受众的方式相同。 [了解如何使用查询建模器](../../audience/../query/query-modeler-overview.md)

>[!TAB 读取受众]

要选择现有受众，请执行以下步骤：

1. 选择&#x200B;**读取受众**。
1. 单击&#x200B;**继续**。
1. 选择受众，与设计新投放时使用受众的方式相同。 请参阅此[章节](../../audience/add-audience.md)。

>[!IMPORTANT]
>
>如果您要使用 **[!UICONTROL 构建受众]** 针对Experience Platform受众的活动，您需要添加 **[!UICONTROL 更改维度]** 活动之后，用于确保受众的定向维度设置为“收件人”。 此页面底部提供了工作流示例。

>[!ENDTABS]

## 示例{#build-audience-examples}

此工作流程示例包含两个&#x200B;**生成受众**&#x200B;活动。第一个示例针对扑克玩家受众，然后是电子邮件投放。第二个示例针对 VIP 客户受众，然后是短信投放。

![](../assets/workflow-audience-example.png)

这是将Adobe Experience Platform受众与Adobe Campaign受众结合在一起的另一个工作流示例。 要允许组合这些受众，请执行以下操作 **[!UICONTROL 更改维度]** 在Adobe Experience Platform受众之后添加了具有“收件人”定向维度的活动。 [了解如何配置更改维度活动](change-dimension.md)

![](../assets/workflow-audience-aep.png)
