---
audience: end-user
title: 为投放构建一次性受众
description: 了解如何为投放构建一次性受众。
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 29%

---

# 生成一次性受众 {#one-time}

本节介绍如何在创建新投放时构建受众。 在这种情况下，可通过查询建模器查询数据库，定向投放受众中要包含的用户档案。 生成的受众仅用于此投放一次。 它不会保存在受众列表中。

定义投放的主要目标时，您还可以：
* [选择现有受众](add-audience.md) 从 **[!UICONTROL 受众]** 列表。
* [从外部文件加载受众](file-audience.md) （仅适用于电子邮件）。

要为投放构建一次性新受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/segment-builder0.png){zoomable=&quot;yes&quot;}

1. 选择 **创建您自己的** 以打开查询建模器，该工具允许您通过筛选数据库中所包含的数据来定义目标群体。 [了解如何使用查询建模器](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable=&quot;yes&quot;}

1. 查询准备就绪后，单击 **确认** 将生成的受众用作投放的主要目标。

   您还可以设置对照组来衡量营销活动的影响。对照组不会接收邮件。这使您能够将收到邮件的群体的行为与未收到邮件的联系人的行为进行比较。[了解详情](control-group.md)
