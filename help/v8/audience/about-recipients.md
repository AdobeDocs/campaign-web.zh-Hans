---
title: 开始使用配置文件
description: 了解如何在Campaign Web中监控和管理用户档案。
badge: label="有限发布版"
source-git-commit: 462725104d28a967dd8a072ef6064b74dad91c58
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 26%

---

# 开始使用配置文件 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="全面查看配置文件"
>abstract="创建新的配置文件，并通过强大的报告和工具对其进行监测。访问配置文件的属性、交互和日志。使用过滤选项浏览配置文件列表、编辑和更新其配置文件。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=zh-Hans" text="请参阅发行说明"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="全面查看配置文件"
>abstract="创建新的配置文件，并通过强大的报告和工具对其进行监测。访问配置文件的属性、交互和日志。使用过滤选项浏览配置文件列表、编辑和更新其配置文件。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=zh-Hans" text="请参阅发行说明"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="用户档案"
>abstract="配置文件是接收 Adobe Campaign 发送的消息所针对的个体。从此列表中可根据您的权限查看配置文件详情。使用过滤选项浏览此列表。您可以编辑和更新配置文件的一小部分属性。"

## 什么是配置文件？ {#what}

A **个人资料**&#x200B;在客户端控制台中又称为“收件人”，表示存储在Campaign数据库中的个人，充当以下对象的关键组件 [创建受众](create-audience.md) 用于投放和 [添加个性化](../personalization/personalize.md) 数据到您的内容。 Adobe Campaign允许您通过Campaign Web用户界面无缝管理用户档案，从创建新条目到访问所有用户档案属性和服务订阅的全面视图。

此外， **[!UICONTROL 测试用户档案]**，在客户端控制台中标识为“种子配置文件”，可让您定位与给定投放的定位标准不匹配的其他收件人。 这些用户档案包含虚构的联系信息或由发件人控制的联系信息。 可以将校样收件人添加到消息的受众，以检测收件人数据库是否用于任何欺诈行为，或确保电子邮件送达收件箱中。 [了解如何使用测试用户档案](test-profiles.md)

用户档案和测试用户档案均可用于在投放到达目标受众之前对其进行测试。 这样，您就可以预览消息内容和个性化，发送验证以进行测试和验证，评估各种平台和设备中的电子邮件渲染情况，并测试您的登陆页面。 [了解如何预览和测试投放](../preview-test/preview-test.md)

## 访问配置文件列表 {#access}

配置文件在Adobe Campaign Web中可通过以下网址访问和编辑： **[!UICONTROL 客户管理]** > **配置文件** 条目进行导航。 您还可以在以下位置访问它们： **[!UICONTROL 资源管理器]** 视图，从 **[!UICONTROL 配置文件和目标]** > **[!UICONTROL 收件人]** 节点。 从该位置，您可以浏览、创建和管理文件夹或子文件夹，以及检查关联的权限。 [了解如何创建文件夹](../get-started/permissions.md#folders)

>[!NOTE]
>
>根据您的权限，您可能无法访问存储在数据库中的用户档案的完整列表。 [了解有关权限的更多信息](../get-started/permissions.md).

您可以筛选 **[!UICONTROL 配置文件]** 使用 **显示筛选器** 按钮。 您可以将结果限制为特定 [文件夹](../get-started/permissions.md#folders) 使用下拉列表，或者使用添加规则 [查询建模器](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png)

要访问配置文件的详细信息，请在列表中单击其名称。 这将打开配置文件的详细视图，允许您浏览其属性以及他订阅的服务。 [了解如何浏览用户档案的详细信息](create-profile.md)

要删除配置文件，请从 **[!UICONTROL 更多操作]** 菜单。
