---
audience: end-user
title: 选择现有受众
description: 了解如何选择受众
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="有限发布版"
source-git-commit: 2c002620fbfeba140b6f80a37116b06d2199c93c
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 30%

---


# 选择现有受众 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="选择现有受众"
>abstract="浏览列表以选择现有受众。使用“显示过滤器”图标筛选列表，或选择特定文件夹。"

本节介绍在定义投放的目标群体时，如何选择现有受众。 定义投放的主要目标时，您还可以：

* [构建一次性受众](one-time-audience.md) 使用查询建模器。
* [从外部文件加载受众](file-audience.md) （仅适用于电子邮件）。

可在投放中定位的受众可从 **受众** 左侧菜单。 它们源自多个源，例如客户端控制台、Campaign Web受众工作流或Adobe Experience Platform。 [了解如何监测和管理受众](manage-audience.md)

要为邮件选择现有受众，请执行以下步骤：

1. 从 **受众** 投放创建助理的部分，单击 **[!UICONTROL 选择受众]** 按钮，然后选择 **[!UICONTROL 选择受众]** 以使用现有受众。

   ![](assets/create-audience.png)

1. 此屏幕显示当前文件夹的所有现有受众。

   ![](assets/create-audience2.png)

   要从Adobe Experience Platform中选择受众，请浏览至 `AEP Audiences folder` 从屏幕的过滤器部分删除。

   ![](assets/select-audience-folder.png)

1. 利用过滤器部分，可访问过滤选项以优化受众列表。 为此，请单击 **添加规则** 以访问查询建模器，从而您可以为受众列表创建高级过滤器。 [了解如何使用查询建模器](../query/query-modeler-overview.md)

   例如，您可以定义一个规则以根据受众的来源进行筛选，如下所示：

   ![](assets/filter-on-aep-audience.png)

1. 单击 **确认** 以将受众添加为投放主要目标。 完成后，您仍然可以使用查询建模器优化受众，方法是单击 **编辑规则** 按钮。

   ![](assets/refine-audience.png)

   您还可以设置对照组来衡量营销活动的影响。对照组不会接收邮件。这使您能够将收到邮件的群体的行为与未收到邮件的联系人的行为进行比较。[了解详情](control-group.md)
