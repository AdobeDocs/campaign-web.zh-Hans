---
audience: end-user
title: 使用Campaign规则生成器构建受众
description: 了解如何使用规则生成器
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 24%

---

# 使用规则生成器 {#segment-builder}

通过规则生成器，您可以通过筛选数据库中包含的数据，定义投放所定向的群体。 使用它可通过&#x200B;**[!UICONTROL 构建受众]**&#x200B;活动从工作流构建受众，或在创建投放以创建一次性受众时直接构建受众。

* [了解如何创建和保存受众](create-audience.md)
* [了解如何为投放创建一次性受众](one-time-audience.md)

## 面板

位于左侧的面板包含可筛选以创建受众的所有元素。 使用搜索栏快速查找元素。 将调色板中包含的拼贴移动到中心画布以进行配置并考虑这些拼贴。

![显示筛选选项和选项卡的调色板界面](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

面板分为两个选项卡：

* **属性**：此选项卡提供对架构中所有可用字段的访问权限。 字段列表取决于电子邮件模板中定义的定位架构。

* **受众**：通过此选项卡，可使用在Campaign Classic控制台中或从Adobe Experience Platform中定义的某个现有受众进行筛选。 在[本节](manage-audience.md)中了解如何监视和管理受众。

  >[!NOTE]
  >
  >要使用Adobe Experience Platform受众，请配置与目标集成。 请参阅[Adobe Experience Platform目标文档](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hans){target="_blank"}。

## 画布

画布是中心区域，您可以在其中根据从面板添加的元素配置和组合规则。 要添加新规则，请从面板中拖动一个磁贴并将其放到画布上。上下文特定的选项是基于要添加的数据类型而显示的。

![显示规则配置选项的画布界面](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## “规则属性”窗格

在右侧，**规则属性**&#x200B;窗格允许您执行下面列出的操作。

![显示可用操作的规则属性窗格](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **查看结果：**&#x200B;显示受众定向的用户档案列表。
* **代码视图**：显示SQL中受众的基于代码的版本。
* **显示高级属性**：选中此选项可查看左侧面板中属性的完整列表，包括节点、分组、1-1链接和1-N链接。
* **计算**：更新并显示查询所定向的用户档案数。
* **选择或保存筛选器**：使用预定义筛选器筛选查询，或将查询另存为新的筛选器以供将来重用。 [了解如何使用预定义过滤器](../get-started/predefined-filters.md)。

  >[!IMPORTANT]
  >
  >在此版本的产品中，用户界面中没有某些预定义过滤器。 但仍可使用这些它们。[了解详情](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)。

* **属性**：显示已创建受众的说明。

## 示例

在此示例中，构建受众的目标是居住亚特兰大或西雅图且出生于1980年之后的所有客户。

1. 在面板的&#x200B;**属性**&#x200B;选项卡中，搜索&#x200B;**出生日期**&#x200B;字段。拖动磁贴并将其放到画布上。

   ![正在将出生日期字段添加到画布](assets/segment-builder6.png){zoomable="yes"}

1. 在画布中，选择 **After** 运算符并输入所需日期。

   ![为“出生日期”字段配置After运算符](assets/segment-builder7.png){zoomable="yes"}

1. 在面板中，搜索&#x200B;**城市**&#x200B;字段，并将其添加到画布中第一条规则的下方。

   ![将“城市”字段添加到画布](assets/segment-builder8.png){zoomable="yes"}

1. 在文本字段中，输入第一个城市名称，然后按 Enter。

   ![在“城市”字段中输入第一个城市名称](assets/segment-builder9.png){zoomable="yes"}

1. 对第二个城市名称重复此操作。

   ![在“城市”字段中输入第二个城市名称](assets/segment-builder10.png){zoomable="yes"}

1. 单击&#x200B;**查看结果**&#x200B;以显示与查询匹配的收件人的列表和数量。添加列以可视化并检查数据。 在此示例中，添加&#x200B;**City**&#x200B;列以查看亚特兰大和西雅图。

   ![正在查看添加了“城市”列的结果](assets/segment-builder11.png){zoomable="yes"}

1. 单击&#x200B;**确认**。