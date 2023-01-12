---
audience: end-user
title: 使用区段生成器
description: Campaign v8 Web文档
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: d5fa13813a22b21fdedd90475ee9258f5003e22d
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 1%

---

# 使用规则生成器定义受众 {#segment-builder}

![](../assets/do-not-localize/badge.png)

本节介绍如何在设计新电子邮件时创建受众。 创建的受众只能在此电子邮件中使用。

规则生成器允许您通过过滤数据库中包含的数据来定义消息定向的群体。 如果要选择现有受众，请参阅 [部分](add-audience.md).

有关规则生成器的更多信息，请参阅 [Segmentation Service文档](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

要在设计电子邮件时创建新受众，请执行以下步骤：

1. 从 **受众** 投放创建助手的部分，单击 **[!UICONTROL 选择受众]** 按钮。

   ![](assets/segment-builder0.png)

1. 选择 **创建您自己的**. 将显示规则生成器。

   ![](assets/segment-builder.png)

## 面板

位于左侧的面板包含可筛选以创建受众的所有元素。 调色板中包含的图块必须移入中心画布中才能进行配置和考虑。 面板分为两个选项卡：

* **属性**:利用此选项卡，可访问架构中的所有可用字段。 字段列表取决于电子邮件模板中定义的定位架构。

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **受众**:利用此选项卡，可使用在“Campaign Classic”控制台中或从Adobe Experience Platform中定义的现有受众之一进行过滤。

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >要利用Adobe Experience Platform受众，您需要配置与目标的集成。 请参阅 [目标文档](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hans){target="_blank"}.

您可以使用搜索栏快速查找元素。

## 画布

画布是中心区域，您可以在其中根据从面板添加的元素配置和组合规则。 要添加新规则，请将拼贴从面板拖放到画布上。 然后，将根据要添加的数据类型向您显示特定于上下文的选项。

![](assets/segment-builder4.png){width="70%" align="left"}

## 规则属性窗格

在右侧， **规则属性** 窗格允许您执行以下操作：

![](assets/segment-builder5.png){width="70%" align="left"}

* **查看结果：** 显示受众定向的收件人列表
* **代码视图**:在SQL中显示基于代码的受众版本。
* **显示高级属性**:如果要查看左侧面板中的完整属性列表，请勾选此选项：节点、分组、1-1链接、1-N链接。
* **属性**:显示已创建受众的描述。

## 示例

在此示例中，我们将构建一个受众，以定位居住在亚特兰大或西雅图的1980年以后出生的所有客户。

1. 在 **属性** ，搜索 **出生日期** 字段。 将图块拖放到画布上。

   ![](assets/segment-builder6.png)

1. 在画布中，选择 **之后** 运算符并输入所需的日期。

   ![](assets/segment-builder7.png)

1. 在面板中，搜索 **城市** 字段，并将其添加到第一个规则下方的画布中。

   ![](assets/segment-builder8.png)

1. 在文本字段中，输入城市名称，然后按Enter。

   ![](assets/segment-builder9.png)

1. 对第二个城市名称重复此操作。

   ![](assets/segment-builder10.png)

1. 单击 **查看结果** 以显示与查询匹配的收件人列表和数量。 您还可以添加列以可视化和检查数据。 在本例中，将 **城市** 列中，应该可以看到亚特兰大和西雅图。

   ![](assets/segment-builder11.png)

1. 单击 **确认**.

您的受众已定义并准备在电子邮件中使用。