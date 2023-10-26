---
audience: end-user
title: 监控和管理受众
description: 了解如何在Adobe Campaign Web中监控和管理受众
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 10%

---

# 监控和管理受众 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="受众出错"
>abstract="无受众数据可用。请等待工作流执行结束。"

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
