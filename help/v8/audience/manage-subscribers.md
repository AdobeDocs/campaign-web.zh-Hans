---
audience: end-user
title: 管理订阅者
description: 了解如何在Adobe Campaign Web中管理服务并将其交付给订阅者
badge: label="有限发布版"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# 管理订阅者 {#manage-subscribers}

一旦您 [已创建服务](manage-services.md#create-service)，您可以添加订阅者、取消订阅收件人，并向该服务的订阅者发送消息。

此页面中详细介绍了订阅者管理。 要了解如何向订阅者发送消息，请参阅 [本节](../msg/send-to-subscribers.md).

## 将订阅者添加到您的服务 {#add-subscribers}

要手动添加订阅者，请执行以下步骤。

1. 从中选择现有服务 **[!UICONTROL 订阅服务]** 列表。

1. 转到 **[!UICONTROL 订阅者]** 选项卡，然后单击 **[!UICONTROL 添加订阅者]**.

   ![](assets/service-subscribers-tab.png)

1. 从列表中选择要添加的配置文件，然后单击 **[!UICONTROL 确认]**.

   ![](assets/service-subscribers-select-profiles.png)

1. 单击 **[!UICONTROL 发送]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> 以使所选收件人接收订阅 [确认消息](manage-services.md#create-confirmation-message) 您定义的时机 [创建服务](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

   >[!NOTE]
   >
   >如果您选择 **[!UICONTROL 取消]**，所选用户档案不会收到确认消息，但会订阅这些用户档案。

添加的用户档案将显示在 **[!UICONTROL 订阅者]** 选项卡。 他们现在已订阅您的服务。

## 从服务中删除订阅者 {#remove-subscribers}

### 手动取消订阅收件人 {#manual-unsubscription}

一旦您 [已添加订阅者](#add-subscribers) 手动取消订阅每一项服务。 请按照以下步骤操作。

1. 从中选择现有服务 **[!UICONTROL 订阅服务]** 列表。

1. 单击所需收件人名称旁边的三个圆点图标，然后选择 **[!UICONTROL 删除]**.

   ![](assets/service-subscribers-delete.png)

1. 确认删除。

1. 单击 **[!UICONTROL 发送]** 以使选定的收件人收到退订 [确认消息](manage-services.md#create-confirmation-message) 您定义的时机 [创建服务](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

收件人将从 **[!UICONTROL 订阅者]** 选项卡，且不再订阅您的服务。

### 自动取消订阅收件人 {#automatic-unsubscription}

订阅服务的持续时间有限。 有效期到期后，收件人会自动取消订阅。

此期限指定于 [创建服务](manage-services.md#create-service). 从 **[!UICONTROL 其他选项]**，禁用 **[!UICONTROL 有效期无限制]** 选项并定义服务的有效期。

![](assets/service-create-validity-period.png)

指定的持续时间过期后，所有订阅者将自动取消订阅该服务。
