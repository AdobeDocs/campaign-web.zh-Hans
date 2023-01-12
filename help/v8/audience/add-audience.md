---
audience: end-user
title: 添加受众
description: Campaign v8 Web文档
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: d5fa13813a22b21fdedd90475ee9258f5003e22d
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 4%

---

# 选择受众 {#add-audience}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="选择现有受众"
>abstract="受众在Adobe Campaign v8控制台中定义。 如果您有可用的Adobe Experience Platform集成，则还应该能够查看平台定义的受众。"

本节将介绍在定义电子邮件投放的目标群体时如何选择现有受众。 如果要创建新受众，请参阅 [部分](segment-builder.md).

1. 从 **受众** 投放创建助手的部分，单击 **[!UICONTROL 选择受众]** 按钮。

   ![](assets/create-audience.png)

1. 选择 **[!UICONTROL 选择受众]** 以使用现有受众。 要创建要在此电子邮件中使用的新受众，请选择 **创建您自己的**. 请参阅 [部分](segment-builder.md).

   此屏幕显示在Adobe Campaign控制台中或从Adobe Experience Platform定义的所有现有受众。

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >要利用Adobe Experience Platform受众，您需要配置与目标的集成。 请参阅 [目标文档](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=zh-Hans){target="_blank"}.

1. 选择受众并单击 **选择**.

1. 单击 **编辑规则** 要优化受众。

   ![](assets/create-audience3.png)

1. 使用规则生成器，您可以使用其他过滤器或通过组合不同的受众来扩充您的受众。 请参阅 [部分](segment-builder.md).

   ![](assets/create-audience4.png)

1. 单击&#x200B;**保存**。

您还可以设置一个控制组来衡量营销活动的影响。 控制组将不会收到消息。 这样，您就可以比较收到消息的群体的行为与未收到消息的联系人的行为。 请参阅 [部分](control-group.md).