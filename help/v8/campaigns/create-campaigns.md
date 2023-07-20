---
audience: end-user
title: 使用 Adobe Campaign Web 创建营销活动
description: 了解如何使用 Adobe Campaign Web 构建跨渠道营销活动
badge: label="Alpha"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: c9954ce69e50e1c8db2532be3292f71ff20f9f74
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 24%

---


# 创建您的第一个营销活动 {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="营销活动创建属性"
>abstract="定义营销活动的属性和元数据。"

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="营销活动属性"
>abstract="定义营销活动设置和元数据。"

要创建新营销活动，您需要定义其属性、计划并包含工作流和投放。

## 创建营销活动{#campaign-create}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="营销活动计划"
>abstract="在营销活动创建期间定义营销活动计划。"

要创建新营销活动，请执行以下步骤：

1. 单击 **[!UICONTROL 营销活动]** 菜单，然后单击 **[!UICONTROL 创建营销活动]** 按钮。
1. 选择 **模板** 为营销活动使用和提供标签。 营销活动模板已预配置，可重复使用它们来创建新营销活动。 它们是从客户端控制台创建的。
   [阅读更多](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=zh-Hans)。
1. 如果需要，可以更改以下内容 **其他选项**：内部名称、文件夹、被分派人、描述和性质。
1. 定义 **计划** 您的营销活动。 营销活动在到达开始日期时开始。 开始日期和结束日期显示在营销活动列表中，并可用作过滤器。 请参阅此[章节](manage-campaigns.md#access-campaigns)。

   ![定义营销活动属性](assets/campaign-properties.png)

   >[!NOTE]
   >
   >您以后始终可以从 **配置Campaign设置** 图标（在促销活动标签旁边）。 请参阅此[章节](gs-campaigns.md#campaign-dashboard)。

1. 单击&#x200B;**创建**。
1. 将工作流和投放添加到营销活动：

   * 从 **工作流** 选项卡，单击 **创建工作流**. 创建活动时，会自动添加默认工作流。 了解更多关于如何操作的信息 [创建工作流](../workflows/create-workflow.md).
   * 从 **投放** 选项卡，单击 **创建投放**. [了解详情](../msg/gs-messages.md)

1. 使用 **日志** 和 **报告** 用于分析营销活动性能的按钮。

## 监控和跟踪您的活动{#campaign-monitoring}

营销活动监测是分析营销活动效果的关键步骤。 打开您的营销策划，然后单击 **日志** 按钮。

您还可以通过单击 **报告** 按钮。 请参阅此[章节](../reporting/campaign-reports.md)。



<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
