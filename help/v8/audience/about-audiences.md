---
audience: end-user
title: 开始使用受众
description: 了解如何在 Campaign Web UI 中使用受众
badge: label="Alpha"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '215'
ht-degree: 100%

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


受众是投放的主要目标：接收邮件的收件人。受众类型取决于投放模板中定义的目标映射。请参阅[此章节](../msg/delivery-template.md)以了解什么是投放模板。

要定义受众群体，您可以：

* 选择现有受众，并在客户端控制台中将其创建为列表。[了解详情](add-audience.md)
* 选择 Adobe Experience Platform 受众。[了解详情](aep-audience.md)
* 通过定义和组合过滤条件，使用规则生成器生成新受众。[了解详情](segment-builder.md)
* 使用外部文件中的受众：此选项仅适用于独立电子邮件投放，而不能用于营销活动投放。[了解详情](file-audience.md)

在营销活动工作流的上下文中发送消息时，受众是在特定的&#x200B;**读取受众**&#x200B;工作流活动中定义的。在此上下文中，您无法从文件加载受众以进行电子邮件投放，并且受众仅在此专用活动中定义。请参阅[此章节](../workflows/orchestrate-activities.md)以了解如何在营销活动工作流中定义投放的受众。

此外，您可以定义对照组来避免向部分受众发送消息，并衡量营销活动的影响。[了解详情](control-group.md)

![](assets/about-audience.png)

