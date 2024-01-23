---
audience: end-user
title: 为投放构建一次性受众
description: 了解如何为投放构建一次性受众。
badge: label="有限发布版"
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: a3476e46c29723af8246683a005543cfd605e7df
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 30%

---

# 生成一次性受众 {#one-time}

本节介绍如何在创建新投放时构建受众。 在本例中，使用查询建模器查询数据库来定位投放受众中要包含的收件人。

生成的受众仅用于此投放一次。 它不会保存在受众列表中。

定义投放的主要目标时，您还可以：

* [选择现有受众](add-audience.md) 从 **[!UICONTROL 受众]** 列表。
* [从外部文件加载受众](file-audience.md) （仅适用于电子邮件）。

要直接从投放构建新受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/segment-builder0.png)

1. 选择&#x200B;**创建您自己的**。此时将显示查询建模器。 利用该功能，可通过过滤数据库中包含的数据来定义投放所定向的群体。 [了解如何使用查询建模器](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png)

1. 查询准备就绪后，单击 **确认** 使用受众作为投放的主要目标。

   您还可以设置对照组来衡量营销活动的影响。对照组不会接收邮件。这使您能够将收到邮件的群体的行为与未收到邮件的联系人的行为进行比较。[了解详情](control-group.md)
