---
audience: end-user
title: 开始使用受众
description: 了解如何在Adobe Campaign Web中使用受众
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: b330230a031a366b674ebac37681274ee89ec6c8
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 25%

---

# 开始使用受众 {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="属性"
>abstract="您可以在此处找到受众属性的总结，例如其来源或其存储文件夹。单击&#x200B;**上一个工作流**&#x200B;部分中的链接以打开已用于创建该受众的工作流。"

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="受众规模"
>abstract="您可以在此处找到受众内轮廓的总数。单击&#x200B;**计算**&#x200B;按钮，可更新并重新计算受众结果。"

>[!CONTEXTUALHELP]
>id="acw_audiences_targeting"
>title="目标选择"
>abstract="目标选择"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="受众出错"
>abstract="无受众数据可用。请等待工作流执行结束。"

受众是投放的主要目标：接收消息的用户档案。 可从&#x200B;**[!UICONTROL 受众]**&#x200B;菜单访问Campaign Web中可用的受众列表。

![显示Campaign Web中可用受众列表的屏幕截图。](assets/audiences-list.png){zoomable="yes"}

受众可以源自多个源。 **[!UICONTROL Origin]**&#x200B;列指示创建给定受众的位置：

* **[!UICONTROL Adobe Campaign]**：这些受众已在[Adobe Campaign Web用户界面](create-audience.md)或[Adobe Campaign v8客户端控制台](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}中创建。

* **[!UICONTROL Adobe Experience Platform：]**&#x200B;这些受众已在Adobe Experience Platform内创建，并已通过Adobe Sources与Destinations集成集成到Campaign Web中。 请参阅[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}以了解如何设置此集成。

  ➡️ [通过观看视频了解此功能](#video)

要获取有关受众的其他信息，请从列表中将其打开。 此时将显示受众属性，以及受众中包含的用户档案数。 使用&#x200B;**[!UICONTROL 计算]**&#x200B;按钮随时刷新受众计数。

要预览受众的临时架构，请单击“属性”部分下的&#x200B;**[!UICONTROL 架构预览]**&#x200B;按钮。

**[!UICONTROL 数据]**&#x200B;选项卡允许您可视化属于受众的用户档案。 通过添加其他列自定义此视图，或使用高级筛选器优化显示的数据。

![显示受众详细信息（包括个人资料和自定义选项）的屏幕截图。](assets/audiences-details.png){zoomable="yes"}

要复制或删除受众，请单击受众名称旁边的受众列表中或受众详细信息屏幕内可用的&#x200B;**[!UICONTROL 更多操作]**&#x200B;按钮。

## 操作说明视频 {#video}

了解如何在Adobe Campaign Web用户界面中创建目标以使用Experience Platform受众。

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

有关如何设置Adobe Sources与Destinations集成的详细信息，请参阅[Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}。