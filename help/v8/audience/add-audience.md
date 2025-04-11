---
audience: end-user
title: 选择现有受众
description: 了解如何选择受众
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 12%

---

# 选择现有受众 {#add-audience}

>[!CONTEXTUALHELP]
>
本节介绍在定义投放的目标群体时，如何选择现有受众。 定义投放的主要目标时，您还可以：
* [使用查询建模器生成一次性受众](one-time-audience.md)。
* [从外部文件加载受众](file-audience.md)（仅适用于电子邮件）。

可从左侧菜单&#x200B;**受众**&#x200B;访问投放中可定位的受众。 它们源自多个来源，例如客户端控制台、Campaign Web受众工作流或Adobe Experience Platform。 [详细了解受众](manage-audience.md)。

要为邮件选择现有受众，请执行以下步骤：

1. 在投放创建助手的&#x200B;**受众**&#x200B;部分中，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 选择受众]**。

   [此屏幕截图显示了投放创建助手中的&#x200B;**选择受众**&#x200B;按钮。](assets/create-audience.png){zoomable="yes"}

1. 此屏幕显示当前文件夹的所有现有受众。

   [此屏幕快照显示当前文件夹中现有受众的列表。](assets/create-audience2.png){zoomable="yes"}

   要从Adobe Experience Platform中选择受众，请从屏幕的筛选器部分中浏览到`AEP Audiences folder`。 [了解有关Adobe Experience Platform受众的更多信息](manage-audience.md#monitor)

   [此屏幕截图显示了选中AEP Audiences文件夹的过滤器部分。](assets/select-audience-folder.png){zoomable="yes"}

1. 利用过滤器部分，可访问过滤选项以优化受众列表。 为此，请单击&#x200B;**添加规则**&#x200B;以访问查询建模器，该建模器允许您为受众列表创建高级过滤器。 [了解如何使用查询建模器](../query/query-modeler-overview.md)

   例如，您可以定义一个规则以根据受众的来源进行筛选，如下所示：

   [此屏幕截图显示基于受众来源应用于受众的过滤器。](assets/filter-on-aep-audience.png){zoomable="yes"}

1. 单击&#x200B;**确认**&#x200B;以将受众添加为投放主目标。 完成后，您可以通过单击&#x200B;**编辑规则**&#x200B;按钮，使用查询建模器优化受众。

   [此屏幕快照显示用于优化受众的&#x200B;**编辑规则**&#x200B;按钮。](assets/refine-audience.png){zoomable="yes"}

1. 您还可以设置对照组来衡量营销活动的影响。控制组未收到消息。 这样，您可以将收到消息的群体的行为与未收到消息的联系人的行为进行比较。 [了解详情](control-group.md)