---
audience: end-user
title: 使用更改数据源工作流活动
description: 了解如何使用更改数据源工作流活动
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---

# 更改数据源 {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="更改数据源"
>abstract="使用&#x200B;**更改数据源**&#x200B;活动，可为工作流的工作表选择不同的数据源。"

**更改数据源**&#x200B;活动是&#x200B;**定位**&#x200B;活动。 此活动允许您更改工作流工作表使用的数据源。 通过允许您跨不同数据库管理数据并提高性能，这提供了更大的灵活性。

在工作流中，通过过渡从一个活动传输到另一个活动的数据存储在临时&#x200B;**工作表**&#x200B;中。 默认情况下，工作表是在与处理数据的源相同的数据库中创建的。 例如，在查询存储在云数据库上的“用户档案”表时，会在同一云数据库上创建一个工作表。

在某些情况下，当前数据库中没有数据，或者数据不够有效，无法执行单一操作。 因此，您可能需要通过添加&#x200B;**[!UICONTROL 更改数据源]**&#x200B;活动，强制工作流使用其他数据库来执行此类操作。

有关Campaign架构的详细信息，请参阅[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)。

>[!IMPORTANT]
>
>请注意，不应将&#x200B;**[!UICONTROL 更改维度]**&#x200B;和&#x200B;**[!UICONTROL 更改数据源]**&#x200B;活动添加到一行中。 如果需要连续使用这两个活动，请在它们之间包含&#x200B;**[!UICONTROL 扩充]**&#x200B;活动。 这可以确保正确执行并防止潜在的冲突或错误。

>[!NOTE]
>
>**更改数据Source**&#x200B;活动每次执行最多可处理100万个记录。 如果您需要提高此限制，请联系您的Adobe代表。

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## 配置更改数据源活动 {#configure}

按照以下步骤配置&#x200B;**更改数据源**&#x200B;活动：

![显示如何将更改数据源活动添加到工作流的屏幕截图。](../assets/workflow-change-data-source-add.png)

1. 将&#x200B;**更改数据源**&#x200B;活动添加到您的工作流。

1. 定义要将工作表移动到的数据源：

   * **[!UICONTROL 默认Campaign数据库(PostgreSQL)]**：使用默认Campaign本地数据库。
   * **[!UICONTROL FDA外部帐户]**：使用通过联合数据访问功能连接到Adobe Campaign的外部云数据库。

     >[!AVAILABILITY]
     >
     >Campaign 配置以及与外部系统的连接仅限高级用户使用，并且只能从客户端控制台中使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hans){target="_blank"}

1. 配置工作流以使用新数据源执行所需的操作。

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->