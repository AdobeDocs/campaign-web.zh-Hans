---
audience: end-user
title: 使用 Adobe Experience Platform 受众
description: 了解如何从 Adobe Experience Platform 使用受众
badge: label="有限发布版"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 703196ad2bb504eb1d50008af110f952d8045eaa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 28%

---

# 使用 Adobe Experience Platform 受众{#aep-audience}

Adobe Campaign托管Cloud Service目标和源连接器允许Adobe Campaign与Adobe Experience Platform之间的无缝集成。

创建Adobe Experience Platform受众并在客户端控制台中可用后，您便可以像对Campaign受众使用一样使用该受众来个性化和发送消息。

>[!NOTE]
>
>要在Campaign中使用Adobe Experience Platform受众，您需要配置与Adobe源和目标的集成。 请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

要选择投放的受众，您还可以：

* 构建新受众。 [了解详情](../query/query-modeler-overview.md)
* 从外部文件加载受众。 [了解详情](file-audience.md)
* 使用现有的Campaign受众。 [了解详情](add-audience.md)。

要选择用于投放的Adobe Experience Platform受众，请执行以下步骤：

1. 从投放创建助手的&#x200B;**受众**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮。

   ![](assets/create-audience.png)

1. 选择&#x200B;**[!UICONTROL 选择受众]**&#x200B;以使用现有受众。要创建要在此电子邮件中使用的新受众，请选择&#x200B;**创建您自己的**。请参阅此[章节](../query/query-modeler-overview.md)。

   此屏幕显示当前文件夹在Adobe Campaign客户端控制台中定义的所有现有受众。 要从Adobe Experience Platform中选择受众，请浏览至 `AEP Audiences folder` 从屏幕的过滤器部分删除。

   ![](assets/select-audience-folder.png)

   您还可以定义规则以根据受众的来源进行过滤，如下所示：

   利用过滤器部分，可访问过滤选项以优化受众列表。 为此，请单击 **添加规则** 以访问查询建模器，从而您可以为受众列表创建高级过滤器。 [了解如何使用查询建模器](../query/query-modeler-overview.md)

   ![](assets/filter-on-aep-audience.png)

1. 选择一个受众，然后单击&#x200B;**选择**。

1. 如果要细化受众，请单击&#x200B;**编辑规则**。

   ![](assets/refine-audience.png)

1. 使用查询建模器，您可以通过附加过滤器或组合不同受众来扩充受众。 请参阅此[章节](../query/query-modeler-overview.md)。

1. 单击&#x200B;**保存**。
