---
audience: end-user
title: 使用订阅服务活动
description: 了解如何使用订阅服务工作流活动
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 13%

---

# 订阅服务 {#subscriptipon-services}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="订阅服务活动"
>abstract="使用新的订阅服务工作流活动管理服务的订阅。 您可以订阅或取消订阅群体，还可以从外部文件更新多个订阅。 或者，也可以发送确认消息以通知订阅者。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hans" text="请参阅发行说明"


>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="订阅服务活动"
>abstract="订阅服务活动允许多个用户档案在单个操作中订阅或取消订阅服务。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="订阅服务常规参数"
>abstract="选择所需的服务并选择要执行的操作（订阅或退订）。 打开 **发送确认消息** 选项启用，通知用户已订阅或取消订阅所选服务。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="生成出站过渡"
>abstract="切换&#x200B;**“生成出站过渡”**&#x200B;选项，可在活动后添加过渡。"

此 **订阅服务** 活动是 **数据管理** 活动。 它允许您为过渡中指定的群体创建或删除对信息服务的订阅。

## 配置订阅服务活动 {#subscription-services-configuration}

按照以下步骤配置 **订阅服务** 活动：

1. 添加 **订阅服务** 活动添加到工作流中。 定向用户档案或导入包含已识别数据的文件后，即可使用此活动。

1. 使用以下选项之一选择要为其管理订阅的服务：

   * **[!UICONTROL 选择特定服务]**：使用手动选择服务 **[!UICONTROL 服务]** 字段。

   * **[!UICONTROL 从集客过渡]**：使用集客过渡中指定的服务。 例如，可以导入一个文件，在该文件中指定用于管理各行的服务。然后，会为每个配置文件动态选择要对其执行操作的服务。

   ![](../assets/workflow-subscription-service.png)

1. 选择要执行的操作： **订阅** 或 **取消订阅**.

   如果在集客过渡中定义了服务，则可以选择如何检索此操作：

   * **选择特定操作类型**：手动选择要执行的操作(**订阅** 或 **取消订阅**)

   * **从集客过渡路径中选择操作类型**：选择集客数据的列，在该列中指定要对每个记录执行的操作。 例如，可以导入一个文件，该文件指定对“operation”列中的每行执行的操作。

     >[!NOTE]
     >
     >此处只能选择boolean或integer字段。 确保包含要执行的操作的数据与此格式匹配。 例如，如果从加载文件活动加载数据，请检查您是否正确设置了中包含操作的列的格式 **[!UICONTROL 加载文件]** 活动。 有关示例，请参见 [本节](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. 要通知收件人他们已订阅或取消订阅所选服务，请切换 **[!UICONTROL 发送确认消息]** 选项启用。 该通知的内容在与信息服务相关联的投放模板中定义。

1. 如果您使用的是来自集客过渡的数据，则 **[!UICONTROL 其他信息]** 部分显示，允许您指定每个记录的数据和订阅来源。 您可以将此部分留空，这样在运行工作流时就不会设置日期或来源。

   * 如果集客数据包含一列，指示用户档案订阅服务的日期，则可以在以下位置选择它： **[!UICONTROL 日期]** 字段。

   * 在 **[!UICONTROL 源路径]** 字段，定义订阅的来源。 您可以将其设置为集客数据的一个字段，也可以通过检查 **[!UICONTROL 将常量设置为原点]** 选项。

   ![](../assets/workflow-subscription-service-additional.png)

1. 要在活动后添加叫客过渡，请切换 **[!UICONTROL 生成叫客过渡]** 选项启用。

## 示例 {#example}

### 将受众订阅到特定服务 {#uc1}

此工作流显示如何让受众订阅现有服务。

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL 构建受众]** 活动面向现有受众。

* A **[!UICONTROL 订阅服务]** 通过活动，选择用户档案必须订阅的服务。

### 从文件更新多个订阅状态 {#uc2}

以下工作流显示如何导入包含用户档案的文件，并将其订阅更新为文件中指定的多项服务。

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL 加载文件]** 活动会加载一个包含数据的CSV文件，并定义导入列的结构。 “服务”和“操作”列指定要更新的服务和要执行的操作（订阅或退订）。

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  如您所见，文件中的操作为“订阅”或“退订”。系统需要 **Boolean** 或 **Integer** 值以识别要执行的操作：“0”代表退订，“1”代表订阅。为满足此要求，必须在示例文件配置屏幕的“operation”列的详细信息中执行值的重新映射。

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  如果文件已使用“0”和“1”来标识操作，则无需重映射这些值。仅确保将列作为 **布尔型** 或 **整数** 在示例文件列中。

* A **[!UICONTROL 调解]** 活动标识来自文件的数据，使其归属至Adobe Campaign数据库的用户档案维度。 此 **电子邮件** 字段的匹配项 **电子邮件** 用户档案资源的字段。

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* An **[!UICONTROL 扩充]** 活动会创建指向“服务(nms)”表的链接，并在上传文件的“服务”列与数据库中的“服务”内部名称”字段之间创建一个简单联接。

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL 删除重复项]** 基于 **电子邮件** 字段标识重复项。 消除重复项很重要，因为如果存在重复项，则所有数据的服务订阅都将失败。

  ![](../assets/workflow-subscription-service-uc2-dedup.png)

* A **[!UICONTROL 订阅服务]** 标识要更新的服务来自过渡，通过在中创建的链接 **[!UICONTROL 调解]** 活动。

  此 **[!UICONTROL 操作类型]** 被标识为来自 **操作** 字段输入。 此处只能选择 Boolean 或 Integer 字段。如果列表中未显示包含要执行操作的文件列，请确保已正确设置了中的列格式 **[!UICONTROL 加载文件]** 活动，如本示例前面所述。

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
