---
audience: end-user
title: 选择现有受众
description: 了解如何选择受众
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 57%

---


# 选择现有受众 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="选择现有受众"
>abstract="浏览列表以选择现有受众。 使用“显示过滤器”图标筛选列表，或选择特定文件夹。"

此章节说明如何在定义电子邮件投放的目标人群时选择现有受众。

您还可以：

* 构建新受众。 [了解详情](segment-builder.md)
* 从外部文件加载受众（仅适用于电子邮件）。 [了解详情](file-audience.md)
* 使用 Adobe Experience Platform 受众。[了解详情](aep-audience.md)。


要为邮件选择现有受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/create-audience.png)

1. 选择&#x200B;**[!UICONTROL 选择受众]**&#x200B;以使用现有受众。要创建要在此电子邮件中使用的新受众，请选择&#x200B;**创建您自己的**。请参阅此[章节](segment-builder.md)。

   此屏幕显示当前文件夹的所有现有受众。

   ![](assets/create-audience2.png)

   受众创建自 **受众** 左侧菜单。 还可以在客户端控制台中创建它们。

   要使用Adobe Experience Platform受众，您需要配置与目标集成。 请参阅 [Adobe Experience Platform目标文档](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hans){target="_blank"}.

1. 选择一个受众，然后单击&#x200B;**选择**。
1. 使用 **显示筛选器** 图标以显示筛选选项。 单击 **添加规则** 要访问规则生成器：使用规则生成器，您可以为受众列表创建高级过滤器。 请参阅以了解如何使用规则生成器 [部分](segment-builder.md).

   ![](assets/create-audience4.png)

1. 单击&#x200B;**保存**。

您还可以设置对照组来衡量营销活动的影响。对照组不会接收邮件。这使您能够将收到邮件的群体的行为与未收到邮件的联系人的行为进行比较。在[此章节](control-group.md)中了解更多信息。