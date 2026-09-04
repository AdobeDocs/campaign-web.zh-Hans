---
audience: end-user
title: 计划和项目
description: 了解如何在Adobe Campaign中创建和配置计划和程序
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
TQID: https://experienceleague.adobe.com/FSiHCjupRlS0zoI9HPdcU--Y2PZot5fQOzWICwmV-oQ
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 640
ht-degree: 5%

---

# 计划和项目 {#plan-and-programs}

使用 Adobe Campaign 可以为营销计划和项目配置文件夹层次结构。

为了更好地组织这些组件，Adobe建议采用以下层次结构：计划`>`项目`>`营销活动。

* **计划**&#x200B;可能包含多个计划。 它定义了特定期间的战略目标。
* **项目**&#x200B;可能包含其他项目以及营销策划、工作流和登陆页面。
* **营销活动**&#x200B;可能包含投放、工作流和登陆页面。

## 创建和配置计划 {#create-plan}

要创建计划，请创建文件夹类型为&#x200B;**[!UICONTROL 计划]**&#x200B;的文件夹。 [了解有关创建文件夹的更多信息](../get-started/work-with-folders.md)

![显示计划文件夹创建的屏幕截图](assets/plan_create.png){zoomable="yes"}

转到计划的&#x200B;**[!UICONTROL 文件夹设置]**&#x200B;对其进行管理。

![显示计划](assets/plan_settings.png){zoomable="yes"}的文件夹设置的屏幕截图

定义&#x200B;**[!UICONTROL 自定义选项]**，并设置计划的计划日期。

![显示计划的自定义选项的屏幕截图](assets/plan_options.png){zoomable="yes"}

要管理&#x200B;**[!UICONTROL 自定义选项]**：

1. 浏览到&#x200B;**[!UICONTROL 架构]**。
1. 在筛选器中选择&#x200B;**[!UICONTROL 可编辑的]**&#x200B;架构。
1. 单击架构。

![显示计划自定义详细信息的编辑屏幕截图](assets/plan_edit.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 屏幕版本]**&#x200B;按钮。

   ![](assets/plan_edit2.png){zoomable="yes"}

配置自定义选项：

![显示计划自定义字段配置的屏幕截图](assets/plan_customfields.png){zoomable="yes"}

## 创建和配置程序 {#create-program}

项目可从左侧导航菜单中获得，类似于营销策划、投放和工作流的列表视图。 **[!UICONTROL 项目群]**&#x200B;条目允许您在现有项目群内创建项目群，而不是在计划下。

要在计划中创建第一个顶级计划，请在资源管理器中导航到您的计划（请参阅此[部分](#create-plan)），然后创建文件夹类型为&#x200B;**[!UICONTROL 计划]**&#x200B;的文件夹。 [了解有关创建文件夹的更多信息](../get-started/work-with-folders.md)。

要在现有项目中创建项目，请执行以下步骤：

1. 在左侧导航菜单中浏览到&#x200B;**[!UICONTROL 程序]**&#x200B;条目。 此视图列出您的所有项目并允许您搜索和过滤。 单击某个程序会在“资源管理器”视图中打开它。

   ![显示节目列表视图的屏幕截图](assets/program_view.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 创建程序]**&#x200B;并配置以下选项：

   ![显示“创建程序”屏幕的屏幕快照](assets/program_create.png){zoomable="yes"}

   * 输入&#x200B;**[!UICONTROL 标签]**。
   * 选择要用作&#x200B;**[!UICONTROL 父文件夹]**&#x200B;的现有程序。
   * （可选）在&#x200B;**[!UICONTROL 计划]**&#x200B;部分中设置&#x200B;**[!UICONTROL 日期范围]**。

   >[!TIP]
   >
   >如果从“资源管理器”视图创建程序，则父文件夹会自动设置为当前程序。

1. 再次单击&#x200B;**[!UICONTROL 创建程序]**&#x200B;以保存更改并创建程序。 然后，程序将显示在“资源管理器”视图中。 您可以像任何其他文件夹一样重命名和删除它，以及访问其设置。 您还可以在此程序中创建子程序。

   ![在资源管理器视图中显示程序的屏幕截图](assets/program_explorer.png){zoomable="yes"}

项目的自定义选项的配置方式与计划的配置方式相同。 请参阅[创建和配置计划](#create-plan)。

## 如何将营销活动链接到项目

您可以通过两种方式将营销活动链接到项目：

### 方#1：您已经有一个项目，并想要创建与其关联的营销策划

要将新营销策划链接到项目，请直接在项目中创建营销策划。

![显示在项目中创建营销活动的屏幕截图](assets/program_campaign_create.png){zoomable="yes"}

**[!UICONTROL 文件夹]**&#x200B;设置将自动填充程序路径。

![显示链接到项目的营销活动文件夹设置的屏幕截图](assets/program_campaign_folder.png){zoomable="yes"}

### 方式#2：您已经有一个现有营销策划，并想要将其链接到现有项目

转到要链接到项目的营销活动的&#x200B;**[!UICONTROL 设置]**&#x200B;按钮。

![显示促销活动设置按钮的屏幕截图](assets/campaign_settings.png){zoomable="yes"}

在其&#x200B;**[!UICONTROL 属性]**&#x200B;中，单击&#x200B;**[!UICONTROL 文件夹]**&#x200B;设置中的&#x200B;**[!UICONTROL 文件夹]**&#x200B;图标以选择您的&#x200B;**[!UICONTROL 程序]**&#x200B;文件夹。

![显示用于将营销活动链接到项目的文件夹选择的屏幕截图](assets/campaign_folder.png){zoomable="yes"}

选择您的&#x200B;**[!UICONTROL 程序]**&#x200B;文件夹，单击&#x200B;**[!UICONTROL 确认]**&#x200B;按钮，然后单击&#x200B;**[!UICONTROL 保存并关闭]**&#x200B;按钮。

![显示链接到项目的营销活动的屏幕截图](assets/campaign_linked.png){zoomable="yes"}

您的营销策划现已列于您的项目中。

![显示计划中所列营销活动的屏幕截图](assets/campaign_in_program.png){zoomable="yes"}