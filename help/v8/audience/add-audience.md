---
audience: end-user
title: 选择受众
description: 了解如何选择受众
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 19%

---


# 选择受众 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="选择现有受众"
>abstract="在 Adobe Campaign v8 控制台中定义受众。如果您有可用的 Adobe Experience Platform 集成，也应能够看到 Platform 定义的受众。"

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

您还可以设置一个控制组来衡量营销活动的影响。 控制组未收到消息。 这样，您就可以比较收到消息的群体的行为与未收到消息的联系人的行为。 请参阅 [部分](control-group.md).