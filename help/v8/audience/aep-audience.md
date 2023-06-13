---
audience: end-user
title: 使用 Adobe Experience Platform 受众
description: 了解如何从 Adobe Experience Platform 使用受众
badge: label="Alpha" type="Positive"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: f7d59309979a063f4491f24c4a9e6deab83a4351
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 50%

---

# 使用 Adobe Experience Platform 受众{#aep-audience}

Adobe Campaign托管Cloud Service目标和源连接器允许Adobe Campaign与Adobe Experience Platform之间的无缝集成。

创建Adobe Experience Platform受众并在客户端控制台中可用后，您可以像对Campaign受众进行个性化和发送消息一样使用该受众。

>[!NOTE]
>
>要在Campaign中使用Adobe Experience Platform受众，您需要配置与Adobe源和目标的集成。 请参阅 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.


您还可以：

* 构建新受众。 [了解详情](segment-builder.md)
* 从外部文件加载受众。 [了解详情](file-audience.md)
* 使用现有的Campaign受众。 [了解详情](add-audience.md)。

要为消息选择Adobe Experience Platform受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/create-audience.png)

1. 选择&#x200B;**[!UICONTROL 选择受众]**&#x200B;以使用现有受众。要创建要在此电子邮件中使用的新受众，请选择&#x200B;**创建您自己的**。请参阅此[章节](segment-builder.md)。

   此屏幕显示当前文件夹在Adobe Campaign客户端控制台中定义的所有现有受众。 要从Adobe Experience Platform中选择受众，请浏览至 `AEP Audiences folder` 从屏幕的过滤器部分。

   ![](assets/select-audience-folder.png)

   您还可以定义根据受众的来源进行筛选的规则，如下所示：

   ![](assets/filter-on-aep-audience.png)

1. 选择一个受众，然后单击&#x200B;**选择**。

1. 如果要细化受众，请单击&#x200B;**编辑规则**。

   ![](assets/refine-audience.png)

1. 利用规则生成器，可以使用附加筛选器或通过组合不同的受众来扩充您的受众。请参阅此[章节](segment-builder.md)。

1. 单击&#x200B;**保存**。

您还可以设置对照组来衡量营销活动的影响。对照组不会接收邮件。这使您能够将收到邮件的群体的行为与未收到邮件的联系人的行为进行比较。请参阅[章节](control-group.md)。

