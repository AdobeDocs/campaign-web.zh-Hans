---
audience: end-user
title: 使用 Adobe Campaign Web 创建营销活动
description: 了解如何使用 Adobe Campaign Web 构建跨渠道营销活动
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 35%

---

# 创建您的第一个营销活动 {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="营销活动创建属性"
>abstract="在此屏幕中，定义营销活动设置：选择模板，然后输入营销活动的标签。浏览找到其他设置以更改默认内部名称和文件夹，添加描述并选择被分派人。"

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="营销活动属性"
>abstract="在此屏幕中，您可以检查和更新营销活动设置：其标签、内部名称、文件夹和描述。您还可以查看将营销活动分配给的用户。"

要创建新营销活动，请定义其设置、计划并包含工作流和投放。

## 创建营销活动 {#campaign-create}

要创建新营销活动，请执行以下步骤：

1. 单击&#x200B;**[!UICONTROL 营销活动]**&#x200B;菜单，然后单击&#x200B;**[!UICONTROL 创建营销活动]**&#x200B;按钮。

   ![显示“营销活动”菜单中“创建营销活动”按钮的屏幕截图](assets/create-campaign-button.png)

1. 选择要使用的&#x200B;**模板**，并提供营销活动的标签。 [了解更多信息](manage-campaigns.md#manage-campaign-templates)。
1. 如果需要，请更改以下&#x200B;**其他选项**：内部名称、文件夹、代理人、说明和性质。
1. 定义营销活动的&#x200B;**计划**。 在[本节](#campaign-schedule)中了解如何设置营销活动计划。
1. 单击&#x200B;**创建**。

   ![显示促销活动属性屏幕的屏幕截图，包括内部名称、文件夹、代理人、描述和性质的字段。](assets/create-a-campaign-properties.png)

1. 将工作流和投放添加到营销活动：

   * 在&#x200B;**工作流**&#x200B;选项卡中，单击&#x200B;**创建工作流**。 创建营销策划时，会自动添加默认工作流。 详细了解如何[创建工作流](../workflows/create-workflow.md)。

   * 在&#x200B;**投放**&#x200B;选项卡中，单击&#x200B;**创建投放**。 [了解详情](../msg/gs-messages.md)

## 监控和跟踪您的活动 {#campaign-monitoring}

营销活动监测是分析营销活动效果的关键步骤。 打开您的营销活动，然后单击&#x200B;**日志**&#x200B;按钮。

您还可以通过单击&#x200B;**报告**&#x200B;按钮查看专用报告。 请参阅此[章节](../reporting/campaign-reports.md)。

## 定义营销活动计划 {#campaign-schedule}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="营销活动计划"
>abstract="选择营销活动计划。您可以创建营销活动，在到达开始日期时，此营销活动将开始。默认情况下，营销活动开始日期为创建日期，持续 5 天。开始日期和结束日期显示在营销活动列表中，并可用作筛选条件。"

达到开始日期时，营销活动即会开始。 只要未到达开始日期，营销活动就会处于&#x200B;**[!UICONTROL 草稿]**&#x200B;状态。 当达到开始日期时，它将变为&#x200B;**[!UICONTROL 正在进行]**。 到达结束日期后，营销活动将设置为&#x200B;**[!UICONTROL 已完成]**。

开始和结束日期显示在营销活动列表中，并可用作过滤器。 请参阅此[章节](manage-campaigns.md#access-campaigns)。

>[!NOTE]
>
>您稍后可以从营销活动标签旁边的&#x200B;**配置营销活动设置**&#x200B;图标修改这些属性。 请参阅此[章节](gs-campaigns.md#campaign-dashboard)。

到达日期后，将实际发送在工作流上下文中该营销活动中创建的已准备好发送的投放。 为此，必须已启动工作流。

<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.
-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header

About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and helps you organize your marketing activities: you can separate them by country, by brand, by unit, and similar criteria.

A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.

To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

* Timeline
* About dynamic reports
* Creating a campaign

In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card, and access a program or sub-program.

Click on the Create button, and select Campaign.

In the Creation mode screen, select a campaign type.

The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date for your campaign. These dates only apply to the campaign itself.

Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

>[!NOTE]
>
>Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.

Programs and campaigns icons and statuses:

Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

* Gray: the program/campaign has not yet started - Editing status.
* Blue: the program/campaign is in progress - In progress status.
* Green: the program/campaign has finished - Finished status.

By default, the current date is automatically shown as the validity start date, and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.

Business.Adobe.com resources
-->