---
audience: end-user
title: 计划和项目
description: 了解如何在Adobe Campaign中创建和配置计划和程序
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 1a751aed6d5185e700dafb1de2afd88300dfcd79
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 3%

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

## 创建和配置程序

要在计划中创建计划（[了解有关创建计划的详细信息](#create-plan)），请导航到您的计划并创建文件夹类型为&#x200B;**[!UICONTROL 计划]**&#x200B;的文件夹。 [了解有关创建文件夹的更多信息](../get-started/work-with-folders.md)。

![显示程序文件夹创建的屏幕截图](assets/program_create.png){zoomable="yes"}

转到程序的&#x200B;**[!UICONTROL 文件夹设置]**&#x200B;对其进行管理。

![显示程序文件夹设置的屏幕截图](assets/program_settings.png){zoomable="yes"}

定义&#x200B;**[!UICONTROL 自定义选项]**，并设置程序的计划日期。

![显示程序自定义选项的屏幕截图](assets/program_options.png){zoomable="yes"}

要管理&#x200B;**[!UICONTROL 自定义选项]**：

1. 浏览到&#x200B;**[!UICONTROL 架构]**。
1. 在筛选器中选择&#x200B;**[!UICONTROL 可编辑的]**&#x200B;架构。
1. 单击架构。

![显示编辑程序自定义详细信息的屏幕截图](assets/program_edit.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 屏幕版本]**&#x200B;按钮。

   ![](assets/program_edit2.png){zoomable="yes"}

配置自定义选项：

![显示程序自定义字段配置的屏幕截图](assets/program_customfields.png){zoomable="yes"}

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