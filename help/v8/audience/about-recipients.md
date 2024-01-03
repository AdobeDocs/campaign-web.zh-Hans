---
title: 监控和管理用户档案
description: 了解如何在Campaign Web中监控和管理用户档案。
badge: label="有限发布版"
source-git-commit: e61878f325575377865186fb9cb63b831ac843fd
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 8%

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

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="基本详细信息"
>abstract="此部分提供有关用户档案的基本详细信息的见解。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="联系人信息"
>abstract="此部分提供有关用户档案的联系信息的洞察。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title= "Address"
>abstract="此部分提供有关用户档案的邮政地址和地址质量的见解。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="帐户详细信息"
>abstract="此部分提供有关配置文件帐户详细信息的洞察。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="收件人不再联系"
>abstract="此部分提供有关用户档案的联系人首选项的分析。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="自定义字段"
>abstract="自定义字段是根据您的需求定制的特定属性，这些属性已针对您的实例进行了配置。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="其他"
>abstract="本节提供了其他内置属性。 要修改任何信息，请直接在相应字段内进行更改，然后单击 **保存** 按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="收件人订阅列表"
>abstract="此选项卡列出了配置文件订阅的所有服务。"

要访问配置文件的详细信息，请在配置文件列表中单击其名称。

![](assets/profiles-details.png)

在此屏幕中，您可以访问有关用户档案的详细信息：

* 此 **[!UICONTROL 详细信息]** 选项卡允许您浏览配置文件的内置属性和自定义属性。 要编辑属性，请在所需字段中进行更改，然后单击 **[!UICONTROL 保存]** 按钮。
* 此 **[!UICONTROL 订阅]** 选项卡提供有关用户档案订阅的服务的信息。 [了解如何使用订阅服务](manage-services.md)
* 此 **[!UICONTROL 日志]** 通过屏幕右上角的按钮，您可以通过发送、排除和跟踪日志查看用户档案交互的历史记录以及呈现给用户档案的建议。
