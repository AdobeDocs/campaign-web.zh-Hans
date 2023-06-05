---
audience: end-user
title: 开始使用受众
description: 了解如何在 Campaign Web UI 中使用受众
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 53%

---


# 开始使用受众 {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


受众是投放的主要目标：接收消息的收件人。 受众类型取决于投放模板中定义的目标映射。请参阅此[章节](../msg/delivery-template.md)。

了解如何使用Campaign规则生成器并定义筛选条件以选择消息的受众。 您可以轻松使用来自外部文件的数据或定位Adobe Experience Platform受众。


要定义受众，您可以：

* 选择在客户端控制台中创建的现有受众。 [了解详情](add-audience.md)
* 使用规则生成器构建新受众。 [了解详情](segment-builder.md)
* 使用来自外部文件的受众。 [了解详情](file-audience.md)
* 使用 Adobe Experience Platform 受众。[了解详情](aep-audience.md)

此外，您可以定义对照组来避免向部分受众发送消息，并衡量营销活动的影响。[了解详情](control-group.md)

![](assets/about-audience.png)

