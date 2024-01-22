---
audience: end-user
title: 监测和管理受众
description: 了解如何在Adobe Campaign Web中监控和管理受众
badge: label="Beta 版"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 523a43bef4f179740a96039ac2fc5f4f858aa1dc
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 15%

---

# 监测和管理受众 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="属性"
>abstract="您可以在此处找到受众属性的摘要，例如其来源、存储文件夹或其状态。 单击以下位置中的链接： **上一个工作流** 部分，用于打开用于创建受众的工作流。"

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="受众规模"
>abstract="您可以在此处找到受众中的配置文件总数。 单击“计算”按钮以更新并重新计算受众结果。"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="受众出错"
>abstract="无受众数据可用。请等待工作流执行结束。"

受众是投放的主要目标：接收邮件的收件人。受众类型取决于投放模板中定义的目标映射。要了解有关投放模板的更多信息，请参阅 [此页面](../msg/delivery-template.md).

要定义受众群体，您可以：

* [创建新受众](create-audience.md) 从 **[!UICONTROL 受众]** 菜单，
* [选择现有受众](add-audience.md) 在客户端控制台中创建为列表或来自Adobe Experience Platform，
* [构建新受众](../query/query-modeler-overview.md) 通过定义和组合筛选条件来使用查询建模器，
* [使用外部文件中的受众](file-audience.md). 此选项仅适用于独立电子邮件投放，不能用于营销活动投放。

定位受众时，您还可以定义 **对照组** 可避免向部分受众发送消息，并衡量活动的影响。 [了解如何设置对照组](control-group.md)

>[!NOTE]
>
>在营销活动工作流的上下文中发送消息时，会在特定中定义受众 **构建受众** 工作流活动。 在此上下文中，您无法从文件加载受众以进行电子邮件投放，并且受众仅在此专用活动中定义。了解如何在的营销活动工作流中定义投放的受众 [本节](../workflows/activities/build-audience.md)

可在Campaign Web中使用的受众列表，可从以下位置访问： **[!UICONTROL 受众]** 菜单。

![](assets/audiences-list.png)

受众可以源自多个源。 此 **[!UICONTROL Origin]** 列指示创建给定受众的位置：

* **[!UICONTROL Adobe Campaign]**：这些受众是在Adobe Campaign V8控制台中创建的。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform：]** 这些受众是在Adobe Experience Platform中创建的，并使用Adobe源和目标集成集成集成到了Campaign Web中。 了解如何在中设置此集成 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>要在Campaign中使用Adobe Experience Platform受众，您需要配置与Adobe源和目标的集成。 请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL Adobe Campaign WebUI]**：这些受众是使用Campaign Web受众工作流创建的。 [了解如何创建受众](create-audience.md)

要获取有关受众的更多信息，请从列表中将其打开。 此时将显示受众属性以及受众中包含的用户档案数。 您可以随时使用刷新受众计数 **[!UICONTROL 计算]** 按钮。

此 **[!UICONTROL 数据]** 选项卡允许您可视化属于受众的用户档案。 您可以通过添加更多列或利用高级筛选器来优化显示的数据来自定义此视图。

![](assets/audiences-details.png)

要复制或删除受众，请单击 **[!UICONTROL 更多操作]** 按钮在受众名称或受众详细信息屏幕中的受众列表中可用。
