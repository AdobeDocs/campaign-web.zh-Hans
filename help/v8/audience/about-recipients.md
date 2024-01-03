---
title: 监控和管理用户档案
description: 了解如何在Campaign Web中监控和管理用户档案。
badge: label="有限发布版"
source-git-commit: a53f33360f0dc7ca80b235bd5814fd3ccc0ff698
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 10%

---

# 监控和管理用户档案 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360个配置文件视图"
>abstract="创建新的用户档案，并通过功能强大的报告和工具监控这些用户档案。 访问用户档案的属性、交互和日志。 使用筛选选项浏览用户档案列表，编辑和更新其用户档案。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="请参阅发行说明"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="用户档案"
>abstract="配置文件是单个对象，旨在接收 Adobe Campaign 发送的消息。从该列表中，您可以查看用户档案的详细信息（基于您的权限）。 使用过滤选项浏览此列表。您可以编辑和更新一小部分用户档案的属性。"

## 开始使用用户档案 {#gs}

Adobe Campaign Web中的用户档案是存储在数据库中的个人，充当为投放创建受众并将个性化数据添加到内容的关键组件。 各种类型的用户档案都存储在数据库中，例如测试用户档案，这些用户档案用于在将投放发送给最终受众之前对其进行测试。 [了解如何使用测试用户档案](test-profiles.md)

只能从Campaign客户端控制台添加用户档案。 但是，在Adobe Campaign Web中，可以从以下位置访问它们： **配置文件** 条目进行导航。 您还可以从以下位置访问它们： **资源管理器** 视图，可在其中浏览、创建文件夹和子文件夹，并检查关联的权限。

您可以使用以下位置提供的搜索字段或过滤器来筛选用户档案列表： **显示筛选器** 按钮。

![](assets/profiles-list.png)

>[!NOTE]
>
>根据您的权限，您可能无法访问存储在数据库中的用户档案的完整列表。 可在[此部分](../get-started/permissions.md)中详细了解权限。

## 访问和编辑用户档案的属性 {#access}

要访问配置文件的详细信息，请在配置文件列表中单击其名称。

![](assets/profiles-details.png)

在此屏幕中，您可以访问有关用户档案的详细信息：

* 此 **[!UICONTROL 详细信息]** 选项卡允许您浏览配置文件的属性。 要编辑属性，请在所需字段中进行更改，然后单击 **[!UICONTROL 保存]** 按钮。
* 此 **[!UICONTROL 订阅]** 选项卡提供有关用户档案订阅的服务的信息。 [了解如何使用订阅服务](manage-services.md)
* 此 **[!UICONTROL 日志]** 通过屏幕右上角的按钮，您可以通过发送、排除和跟踪日志查看用户档案交互的历史记录以及呈现给用户档案的建议。
