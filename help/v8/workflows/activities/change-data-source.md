---
audience: end-user
title: 使用更改数据源工作流活动
description: 了解如何使用更改数据源工作流活动
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 27%

---

# 更改数据源 {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="更改数据源"
>abstract="使用新的更改数据源工作流定位活动来更改工作流工作表使用的数据源。这项活动提供了更大的灵活性，使您可以跨不同的数据库管理数据并提高性能。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="请参阅发行说明"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="更改数据源"
>abstract="使用&#x200B;**更改数据源**&#x200B;活动，可为工作流的工作表选择不同的数据源。"

此 **更改数据源** 活动是 **定位** 活动。 此活动允许您更改工作流工作表使用的数据源。 这允许您跨不同的数据库管理数据并提高性能，从而提供了更大的灵活性。

在工作流中，通过过渡从一个活动传输到另一个活动的数据存储在临时中 **工作台**. 默认情况下，工作表是在与处理数据的源相同的数据库中创建的。 例如，在查询存储在云数据库上的“用户档案”表时，会在同一云数据库上创建一个工作表。

在某些情况下，当前数据库中没有数据，或者数据不够有效，无法执行单一操作。 因此，您可能需要通过添加 **[!UICONTROL 更改数据源]** 活动。

有关Campaign架构的详细信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## 配置更改数据源活动 {#configure}

按照以下步骤配置 **更改维度** 活动：

![](../assets/workflow-change-data-source-add.png)

1. 添加 **更改数据源** 活动添加到工作流。

1. 定义要将工作表移动到的数据源：

   * **[!UICONTROL 默认Campaign数据库(PostgreSQL)]**：使用默认的Campaign本地数据库。
   * **[!UICONTROL FDA外部帐户]**：使用通过联合数据访问功能连接到Adobe Campaign的外部云数据库。

     >[!AVAILABILITY]
     >
     >Campaign 配置以及与外部系统的连接仅限高级用户使用，并且只能从客户端控制台中使用。[了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=zh-Hans){target="_blank"}

1. 配置工作流以使用新数据源执行所需的操作。

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
