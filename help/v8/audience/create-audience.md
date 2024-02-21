---
audience: end-user
title: 创建受众
description: 了解如何在Adobe Campaign Web中创建受众
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: cdb33c46e849a16272869913044358d344e0d6ba
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 21%

---

# 创建受众 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="受众组合"
>abstract="在可视化工作流程画布中创建新受众。除了从头开始创建简单受众之外，还可利用工作流活动细化受众。将多个受众合并为单个受众、用外部属性充实受众或根据所选择的规则将其划分为多个受众。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=zh-Hans" text="请参阅发行说明"

<!--TO REMOVE BELOW-->

>[!CONTEXTUALHELP]
>id="acw_homepage_rn1"
>title="受众组合"
>abstract="在可视化工作流程画布中创建新受众。除了从头开始创建简单受众之外，还可利用工作流活动细化受众。将多个受众合并为单个受众、用外部属性充实受众或根据所选择的规则将其划分为多个受众。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=zh-Hans" text="请参阅发行说明"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="受众"
>abstract="可从此屏幕访问可在投放中定位的所有受众的列表。单击&#x200B;**创建**&#x200B;以使用&#x200B;**拆分**&#x200B;或&#x200B;**排除**&#x200B;等各种工作流活动将新受众创建到视觉画布中。"

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="受众设置"
>abstract="输入受众姓名和其他选项，然后单击&#x200B;**创建受众**&#x200B;按钮。"

Campaign Web允许您在可视工作流画布中创建新受众。 除了从头开始创建简单受众之外，还可利用工作流活动细化受众。例如，您可以将多个受众合并为单个受众，使用外部属性丰富受众，或根据您选择的规则将受众划分为多个受众。

创建工作流后，生成的受众将自动与现有受众一起存储在Campaign数据库中。 然后，可以在工作流或独立投放中定位这些受众。

➡️ [在视频中发现此功能](#video)

## 创建您的第一个受众 {#create}

要创建受众，请执行以下步骤：

1. 导航至 **[!UICONTROL 受众]** 菜单，然后单击 **[!UICONTROL 创建受众]** 按钮进行标记。

1. 系统会自动创建一个新工作流，允许您合并活动以生成受众。 默认情况下，画布包含两个主要活动：

   * “查询” **[!UICONTROL 构建受众]** 活动是工作流的起点，允许您创建受众，并将其用作工作流的基础。

   * “新受众” **[!UICONTROL 保存受众]** 活动表示工作流中的最后一步，使您能够将结果另存为新受众。

   ![](assets/create-audience-blank.png){zoomable=&quot;yes&quot;}

   >[!IMPORTANT]
   >
   >受众工作流存储在中 **工作流** 菜单，以及您的其他营销活动工作流。 它们专门为构建受众而设计，可通过其垂直画布进行识别。

1. 为了提高可读性，我们建议在工作流设置中更改工作流的名称。 **标签** 字段。 [了解如何配置工作流设置](../workflows/workflow-settings.md)

1. 打开 **[!UICONTROL 构建受众]** 活动并使用查询建模器，通过筛选数据库中包含的数据来定义要包含在受众中的群体。 [了解如何配置构建受众活动](../workflows/activities/build-audience.md)

1. 如果想要对工作流中的定向群体执行其他操作，请根据需要添加尽可能多的活动，并将它们连接在一起。 有关如何配置工作流活动的更多信息，请参阅 [工作流文档](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >渠道活动不可用于受众工作流。

   ![](assets/audience-creation-canvas.png){zoomable=&quot;yes&quot;}

1. 配置 **[!UICONTROL 保存受众]** 活动，指定您希望如何保存工作流上游计算的群体。 [了解如何配置保存受众活动](../workflows/activities/save-audience.md)

1. 工作流准备就绪后，单击 **[!UICONTROL 开始]** 执行它。

工作流将保存在中 **[!UICONTROL 工作流]** 列表，而生成的受众可在中访问 **[!UICONTROL 受众]** 列表中定义了标签 **保存受众** 活动。 了解如何在中监控和管理受众 [本节](manage-audience.md)

您现在可以使用此受众作为投放的主要目标。 [了解详情](add-audience.md)

## 受众工作流示例 {#example}

下方的示例显示了一个受众工作流，该工作流配置为定向居住在纽约的女客户，并根据他们最近购买过的物品（瑜伽或跑步装备）创建两个新受众。

![](assets/audiences-example.png){zoomable=&quot;yes&quot;}

1. 此 **[!UICONTROL 构建受众]** 活动针对居住在纽约的所有女性用户档案。
1. 此 **[!UICONTROL 扩充]** 活动通过“购买”表中的信息丰富了受众，以确定客户购买的产品类型。
1. 此 **[!UICONTROL Split]** 活动根据客户的最新购买情况将工作流分为两个路径。
1. 此 **[!UICONTROL 保存受众]** 每个路径末尾的活动会在数据库中创建两个新受众，其中包括每个路径中计算的群体。

## 编辑受众 {#edit}

您可以根据需要通过重新执行相应的工作流来修改从工作流生成的受众。 这样，您就可以轻松地刷新受众数据，或通过调整查询来满足您的需求来优化受众。

1. 导航至 **受众** 菜单并打开要编辑的受众。
1. 在 **概述** 选项卡， **上一个工作流** 部分提供用于生成受众的工作流的链接。 单击以访问工作流。
1. 进行所需的更改，然后单击 **开始** 按钮以再次重新运行工作流。 完成后，工作流产生的受众将自动更新为最新工作流结果。

默认情况下，重新运行受众工作流会使用新数据替换受众的整个内容，从而导致以前的数据丢失。

如果您不希望替换现有的受众结果，请配置 **保存受众** 活动以符合您的要求。 例如，您可以更改 **受众标签** 用于将新结果存储到新受众中的字段，或将新结果添加到现有受众内容而不擦除以前的数据。 [了解如何配置保存受众活动](../workflows/activities/save-audience.md)

![](assets/edit-audience-save.png){zoomable=&quot;yes&quot;}

## 操作方法视频 {#video}

了解如何构建和管理受众、如何为投放选择受众以及定义控制组。

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)
