---
audience: end-user
title: 选择受众
description: 了解如何选择受众
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positive"
source-git-commit: cf94ea6f5bbb287c5cd56f5af023a40d1f8538d6
workflow-type: ht
source-wordcount: '272'
ht-degree: 100%

---


# 选择现有受众 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="选择现有受众"
>abstract="在 Adobe Campaign v8 控制台中定义受众。如果您有可用的 Adobe Experience Platform 集成，也应能够看到 Platform 定义的受众。"

此章节说明如何在定义电子邮件投放的目标人群时选择现有受众。

您还可以：

* 创建新受众。[了解详情](segment-builder.md)
* 从文件导入受众。[了解详情](import-audience.md)
* 使用 Adobe Experience Platform 受众。[了解详情](aep-audience.md)。


要为邮件选择现有受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/create-audience.png)

1. 选择&#x200B;**[!UICONTROL 选择受众]**&#x200B;以使用现有受众。要创建要在此电子邮件中使用的新受众，请选择&#x200B;**创建您自己的**。请参阅此[章节](segment-builder.md)。

   此屏幕将显示在 Adobe Campaign 控制台中定义的或 Adobe Experience Platform 中的所有现有受众。

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >要利用 Adobe Experience Platform 受众，您需要配置与 Destinations 的集成。请参阅 [Destinations 文档](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hans){target="_blank"}。

1. 选择一个受众，然后单击&#x200B;**选择**。

1. 如果要细化受众，请单击&#x200B;**编辑规则**。

   ![](assets/create-audience3.png)

1. 利用规则生成器，可以使用附加筛选器或通过组合不同的受众来扩充您的受众。请参阅此[章节](segment-builder.md)。

   ![](assets/create-audience4.png)

1. 单击&#x200B;**保存**。

您还可以设置对照组来衡量营销活动的影响。对照组不会接收邮件。这使您能够将收到邮件的群体的行为与未收到邮件的联系人的行为进行比较。请参阅[章节](control-group.md)。