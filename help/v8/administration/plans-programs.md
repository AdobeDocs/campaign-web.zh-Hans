---
audience: end-user
title: 计划和项目
description: 了解如何在Adobe Campaign中创建和配置计划和程序
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: dfd5f2e000b02d4382eaac0c9bb00fe940a99f79
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 10%

---

# 计划和项目 {#plan-and-programs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="计划和项目"
>abstract="您现在可以在 Campaign Web 用户界面中配置营销计划和方案的文件夹层次结构。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

使用 Adobe Campaign 可以为营销计划和项目配置文件夹层次结构。

为了更好地组织这些活动，Adobe建议采用以下层次结构：计划`>`项目`>`营销活动

* **计划**&#x200B;可能包含多个计划。 它定义了一个时期的战略目标。
* **项目**&#x200B;可能包含其他项目以及营销策划、工作流和登陆页面。
* **营销活动**&#x200B;可能包含投放、工作流和登陆页面。

## 创建和配置计划 {#create-plan}

要创建计划，您需要创建文件夹类型为&#x200B;**[!UICONTROL 计划]** [了解有关创建文件夹的更多信息](../get-started/work-with-folders.md)。

![](assets/plan_create.png){zoomable="yes"}

转到计划的&#x200B;**[!UICONTROL 文件夹设置]**&#x200B;对其进行管理。

![](assets/plan_settings.png){zoomable="yes"}

您可以定义&#x200B;**[!UICONTROL 自定义选项]**，并设置计划的计划日期。

![](assets/plan_options.png){zoomable="yes"}

要管理&#x200B;**[!UICONTROL 自定义选项]**：

1. 浏览到&#x200B;**[!UICONTROL 架构]**
1. 选择筛选器中的&#x200B;**[!UICONTROL 可编辑]**&#x200B;架构
1. 单击&#x200B;**[!UICONTROL 编辑自定义详细信息]**&#x200B;的图标

![](assets/plan_edit.png){zoomable="yes"}

您可以对其进行配置：

![](assets/plan_customfields.png){zoomable="yes"}

## 创建和配置程序

若要在计划中创建计划（[了解有关创建计划的详细信息](#create-plan)），您需要加入计划，并创建文件夹类型为&#x200B;**[!UICONTROL 计划]** [了解有关创建文件夹的更多信息](../get-started/work-with-folders.md)。

![](assets/program_create.png){zoomable="yes"}

转到程序的&#x200B;**[!UICONTROL 文件夹设置]**&#x200B;对其进行管理。

![](assets/program_settings.png){zoomable="yes"}

您可以定义&#x200B;**[!UICONTROL 自定义选项]**，并设置程序的计划日期。

![](assets/program_options.png){zoomable="yes"}

要管理&#x200B;**[!UICONTROL 自定义选项]**：

1. 浏览到&#x200B;**[!UICONTROL 架构]**
1. 选择筛选器中的&#x200B;**[!UICONTROL 可编辑]**&#x200B;架构
1. 单击&#x200B;**[!UICONTROL 编辑自定义详细信息]**&#x200B;的图标

![](assets/program_edit.png){zoomable="yes"}

您可以对其进行配置：

![](assets/program_customfields.png){zoomable="yes"}

## 如何将营销活动链接到项目

您可以通过两种方式将营销活动链接到项目：

### 方#1：您已经有一个项目，并想要创建与其关联的营销策划

要将新营销活动链接到项目，请直接在项目中创建您的营销活动：

![](assets/program_campaign_create.png){zoomable="yes"}

**[!UICONTROL 文件夹]**&#x200B;设置将自动与程序路径一起归档。

![](assets/program_campaign_folder.png){zoomable="yes"}

### 方式#2：您已经有一个现有营销策划，并想要将其链接到现有项目

转到要链接到项目的营销活动的&#x200B;**[!UICONTROL 设置]**&#x200B;按钮：

![](assets/campaign_settings.png){zoomable="yes"}

在其&#x200B;**[!UICONTROL 属性]**&#x200B;中，单击&#x200B;**[!UICONTROL 文件夹]**&#x200B;设置中的&#x200B;**[!UICONTROL 文件夹]**&#x200B;图标，以选择您的&#x200B;**[!UICONTROL 程序]**&#x200B;文件夹。

![](assets/campaign_folder.png){zoomable="yes"}

选择您的&#x200B;**[!UICONTROL Program]**&#x200B;文件夹并单击&#x200B;**[!UICONTROL 确认]**&#x200B;按钮，然后单击&#x200B;**[!UICONTROL 保存并关闭]**&#x200B;按钮。

![](assets/campaign_linked.png){zoomable="yes"}

您的营销活动现已列于您的项目中：

![](assets/campaign_in_program.png){zoomable="yes"}
