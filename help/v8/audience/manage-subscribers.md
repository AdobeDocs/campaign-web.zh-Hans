---
audience: end-user
title: 管理订阅者
description: 了解如何在Adobe Campaign Web中管理服务并将其交付给订阅者
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 管理订阅者 {#manage-subscribers}

创建服务[后](manage-services.md#create-service)，您可以添加订阅者、取消订阅收件人并向该服务的订阅者发送消息。

此页面中详细介绍了订阅者管理。 若要了解如何向订阅者发送消息，请参阅[此部分](../msg/send-to-subscribers.md)。

## 将订阅者添加到您的服务 {#add-subscribers}

要手动添加订阅者，请执行以下步骤。

1. 从&#x200B;**[!UICONTROL 订阅服务]**&#x200B;列表中选择现有服务。

1. 转到&#x200B;**[!UICONTROL 订阅者]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 添加订阅者]**。

   ![](assets/service-subscribers-tab.png){zoomable="yes"}

1. 从列表中选择要添加的配置文件，然后单击&#x200B;**[!UICONTROL 确认]**。

   ![](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 发送]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->，使所选收件人接收您在[创建服务](manage-services.md#create-service)时定义的订阅[确认消息](manage-services.md#create-confirmation-message)。

   ![](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >如果选择&#x200B;**[!UICONTROL 取消]**，将不会向选定的用户档案发送确认消息，但是这些用户档案已订阅。

添加的用户档案显示在&#x200B;**[!UICONTROL 订阅者]**&#x200B;选项卡中。 他们现在已订阅您的服务。

## 从服务中删除订阅者 {#remove-subscribers}

### 手动取消订阅用户档案 {#manual-unsubscription}

向服务[添加订阅者](#add-subscribers)后，您可以手动取消订阅每个订阅者。 请按照以下步骤操作。

1. 从&#x200B;**[!UICONTROL 订阅服务]**&#x200B;列表中选择现有服务。

1. 单击所需收件人名称旁边的三个圆点图标，然后选择&#x200B;**[!UICONTROL 删除]**。

   ![](assets/service-subscribers-delete.png){zoomable="yes"}

1. 确认删除。

1. 单击&#x200B;**[!UICONTROL 发送]**，使选定的收件人接收您在[创建服务](manage-services.md#create-service)时定义的取消订阅[确认消息](manage-services.md#create-confirmation-message)。

   ![](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

收件人已从&#x200B;**[!UICONTROL 订阅者]**&#x200B;选项卡中删除，且不再订阅您的服务。

### 自动取消订阅收件人 {#automatic-unsubscription}

订阅服务的持续时间有限。 当有效期过期时，用户档案会自动取消订阅。

此期限在[创建服务](manage-services.md#create-service)时指定。 在&#x200B;**[!UICONTROL 其他选项]**&#x200B;中，禁用&#x200B;**[!UICONTROL 无限有效期]**&#x200B;选项并定义服务的有效期。

![](assets/service-create-validity-period.png){zoomable="yes"}

指定的持续时间过期后，所有订阅者将自动取消订阅该服务。
