---
audience: end-user
title: 使用规则生成器定义受众
description: 了解如何使用区段生成器
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: ht
source-wordcount: '549'
ht-degree: 100%

---

# 使用规则生成器定义受众 {#segment-builder}

此章节介绍如何在设计新电子邮件时创建受众。创建的受众只能在当前电子邮件中使用。

利用规则生成器，可以通过筛选数据库中包含的数据来定义邮件的目标人群。如果要选择现有受众，请参阅此[章节](add-audience.md)。

有关规则生成器的更多信息，请参阅[分段服务文档](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html)。

要在设计电子邮件时创建新的受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/segment-builder0.png)

1. 选择&#x200B;**创建您自己的**。这将显示规则生成器。

   ![](assets/segment-builder.png)

## 面板

左侧的面板包含可筛选以创建受众的所有元素。面板中包含的磁贴必须移入中心画布才能进行配置和使用。面板分为两个选项卡：

* **属性**：此选项卡可让您访问架构中的所有可用字段。字段列表取决于电子邮件模板中定义的定位架构。

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **受众**：此选项卡可让您使用在 Campaign Classic 控制台中定义的或 Adobe Experience Platform 中的某个现有受众进行筛选。

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >要利用 Adobe Experience Platform 受众，您需要配置与 Destinations 的集成。请参阅 [Destinations 文档](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hans){target="_blank"}。

您可以使用搜索栏快速查找元素。

## 画布

画布是指位于中央的区域，您可以在其中根据从面板添加的元素来配置和组合规则。要添加新规则，请从面板中拖动一个磁贴并将其放到画布上。之后，将根据要添加的数据类型为您提供特定于上下文的选项。

![](assets/segment-builder4.png){width="70%" align="left"}

## “规则属性”窗格

利用右侧的&#x200B;**规则属性**&#x200B;窗格，您可以执行以下操作：

![](assets/segment-builder5.png){width="70%" align="left"}

* **查看结果**：显示按受众定位的收件人的列表。
* **代码视图**：在 SQL 中显示基于代码的受众版本。
* **显示高级属性**：如果您要在左侧面板中查看完整属性列表，请选中此选项：节点、分组、1-1 链接、1-N 链接。
* **属性**：显示已创建受众的描述。

## 示例

在此示例中，我们生成了一个受众来定位所有居住在亚特兰大或西雅图的 1980 年之后出生的客户。

1. 在面板的&#x200B;**属性**&#x200B;选项卡中，搜索&#x200B;**出生日期**&#x200B;字段。拖动磁贴并将其放到画布上。

   ![](assets/segment-builder6.png)

1. 在画布中，选择 **After** 运算符并输入所需日期。

   ![](assets/segment-builder7.png)

1. 在面板中，搜索&#x200B;**城市**&#x200B;字段，并将其添加到画布中第一条规则的下方。

   ![](assets/segment-builder8.png)

1. 在文本字段中，输入第一个城市名称，然后按 Enter。

   ![](assets/segment-builder9.png)

1. 对第二个城市名称重复此操作。

   ![](assets/segment-builder10.png)

1. 单击&#x200B;**查看结果**&#x200B;以显示与查询匹配的收件人的列表和数量。还可以添加列以可视化和检查数据。在我们的示例中，添加&#x200B;**城市**&#x200B;列，应看到亚特兰大和西雅图。

   ![](assets/segment-builder11.png)

1. 单击&#x200B;**确认**。

您的受众已定义并可在电子邮件中使用。