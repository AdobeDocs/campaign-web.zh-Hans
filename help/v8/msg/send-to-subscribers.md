---
audience: end-user
title: 向服务的订阅者发送消息
description: 了解如何向服务的订阅者发送消息
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 向服务的订阅者发送消息 {#send-to-subscribers}

您可以在Adobe Campaign中创建订阅服务，并向订阅者发送消息。 了解如何在[此页面](../audience//manage-services.md#create-service)上创建订阅服务。

要向订阅者发送消息，请创建特定受众以识别订阅者，然后创建投放，如下所述。

1. 创建受众。 系统会自动创建新工作流。 [了解有关受众的详细信息](../audience/create-audience.md)

1. 为了提高可读性，请在工作流设置&#x200B;**标签**&#x200B;字段中更改工作流的名称。 [了解如何配置工作流设置](../workflows/workflow-settings.md)

1. 打开&#x200B;**[!UICONTROL 生成受众]**&#x200B;活动，然后选择&#x200B;**[!UICONTROL 创建受众]**。 [了解如何配置生成受众活动](../workflows/activities/build-audience.md)

   ![](assets/service-create-audience.png){zoomable="yes"}

1. 在受众创建流程中，选择以下自定义条件：存在&#x200B;**[!UICONTROL 订阅]**，例如&#x200B;**[!UICONTROL 服务]**&#x200B;等于您定义的服务。 在此示例中，选择您的&#x200B;**Luma瑜伽新闻稿**。

   ![](assets/service-audience-subscribers.png){zoomable="yes"}

1. 选择&#x200B;**[!UICONTROL 确认]**&#x200B;并单击&#x200B;**[!UICONTROL 开始]**&#x200B;以执行工作流。

1. 创建投放。 创建投放的步骤详见[此页面](../msg/gs-messages.md#create-delivery)。
1. 浏览到您的投放设置，将默认目标映射更改为&#x200B;**订阅(nms：subscriptions)**。

   ![](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. 在投放的主目标部分中，选择您在上面创建的受众。

   ![](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. 创建邮件内容，测试并发送投放，如[此部分](../preview-test/preview-test.md)中所述。

   ![](assets/service-delivery-ready.png){zoomable="yes"}

您的投放仅发送给该服务的订阅者。
