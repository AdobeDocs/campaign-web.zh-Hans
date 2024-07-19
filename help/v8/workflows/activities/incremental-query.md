---
audience: end-user
title: 使用增量查询工作流活动
description: 了解如何使用增量查询工作流活动
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 19%

---

# 增量查询 {#incremental-query}



>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="增量查询"
>abstract=" **增量查询**&#x200B;活动是一个&#x200B;**定位**&#x200B;活动，它允许您使用查询建模器查询数据库。每次执行此活动时，都会排除先前执行得出的结果。这样可让您仅定向新元素。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="增量查询历史记录"
>abstract="增量查询历史记录"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="增量查询处理后的数据"
>abstract="增量查询处理后的数据"

**增量查询**&#x200B;活动是&#x200B;**定位**&#x200B;活动，允许您按计划查询数据库。 每次执行此活动时，都会排除先前执行得出的结果。这样可让您仅定向新元素。

>[!NOTE]
>
>虽然Campaign客户端控制台将&#x200B;**[!UICONTROL 增量查询]**&#x200B;活动与内置调度程序集成，但Campaign Web用户界面会单独处理此功能。 要计划增量查询执行，您必须先在工作流中添加一个&#x200B;**[!UICONTROL 调度程序]**&#x200B;活动，然后再添加&#x200B;**[!UICONTROL 增量查询]**&#x200B;活动。 [了解如何配置调度程序活动](scheduler.md)

**[!UICONTROL 增量查询]**&#x200B;活动可用于各种类型的使用：

* 对个体进行分段以定义消息的目标、受众等。
* 导出数据。 例如，您可以使用活动以文件格式定期导出新日志。 如果要在外部报表或BI工具中使用日志数据，则此功能非常有用。

之前执行已定向的群体将存储在工作流中。 这意味着从同一模板启动的两个工作流不共享同一日志。 但是，同一工作流中基于同一增量查询的两个任务使用相同的日志。

如果增量查询在其执行之一期间的结果等于0，则工作流将暂停，直到查询下一次程序化执行。 因此，在后续执行之前，不会处理增量查询之后的过渡和活动。

## 配置增量查询活动 {#incremental-query-configuration}

按照以下步骤配置&#x200B;**增量查询**&#x200B;活动：

![](../assets/incremental-query.png)

1. 将&#x200B;**增量查询**&#x200B;活动添加到您的工作流中。

1. 在&#x200B;**[!UICONTROL 受众]**&#x200B;部分中，选择&#x200B;**定向维度**，然后单击&#x200B;**[!UICONTROL 继续]**。

   定位维度可让您定义操作的目标人群：收件人、合同受益人、操作人员、订阅者等。默认情况下，目标是从收件人中选择的。[了解有关定向维度的更多信息](../../audience/about-recipients.md#targeting-dimensions)

1. 使用查询建模器定义查询，与设计新电子邮件时创建受众的方式相同。 [了解如何使用查询建模器](../../query/query-modeler-overview.md)

1. 在&#x200B;**[!UICONTROL 已处理数据]**&#x200B;部分中，选择要使用的增量模式：

   * **[!UICONTROL 排除先前执行的结果]**：每次执行活动时，都会排除先前执行的结果。

     以前执行中已定向的记录最多可记录从被定向之日起的天数。 为此，请使用&#x200B;**[!UICONTROL History in days]**&#x200B;字段。 如果此值为零，则不会从日志中清除收件人。

   * **[!UICONTROL 使用日期字段]**：此选项允许您根据特定日期字段从先前执行中排除结果。 要实现此目的，请从可用于所选定向维度的属性列表中选择所需的日期字段。 在下次执行工作流时，将仅检索在上次执行日期之后修改或创建的数据。

     在第一次执行工作流后，**[!UICONTROL 上次执行日期]**&#x200B;字段变为可用。 它指定将用于下一次执行的日期，并在每次执行工作流时自动更新。 您仍然可以手动输入新值来覆盖此值，以使其符合您的需求。

   >[!NOTE]
   >
   >根据所选的日期字段，**[!UICONTROL 使用日期字段]**&#x200B;模式允许更大的灵活性。 例如，如果指定字段对应于修改日期，则可利用日期字段模式，检索最近更新的数据，而其他模式将仅排除在先前执行中已定向的记录，即使上次执行工作流后已修改这些记录也是如此。

## 示例 {#incremental-query-example}

以下示例显示了一个工作流的配置，该工作流每周都会筛选Adobe Campaign数据库中订阅Yoga新闻稿服务的用户档案，以向他们发送欢迎电子邮件。

![](../assets/incremental-query-example.png)

工作流由以下元素组成：

* **[!UICONTROL 调度程序]**&#x200B;活动，用于在每周一早上6:00执行工作流。
* **[!UICONTROL 增量查询]**&#x200B;活动，用于在第一次执行期间定向所有当前订阅者，然后在后续执行期间只定向该周的新订阅者。
* **[!UICONTROL 电子邮件投放]**&#x200B;活动。
