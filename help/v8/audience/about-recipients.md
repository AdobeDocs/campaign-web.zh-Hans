---
title: 开始使用配置文件
description: 了解如何在Campaign Web中监控和管理用户档案。
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 5a4bf85a1f70a0282405aededfb31038f9db17a8
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 12%

---

# 开始使用用户档案 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="用户档案"
>abstract="配置文件是接收 Adobe Campaign 发送的消息所针对的记录。从此列表中可根据您的权限查看配置文件详情。使用过滤选项浏览此列表。您可以编辑和更新配置文件的一小部分属性。"

## 什么是配置文件？ {#what}

**用户档案**，在客户端控制台中又称为“收件人”，表示存储在Campaign数据库中的记录，它用作[为投放创建受众](create-audience.md)以及[将个性化](../personalization/personalize.md)数据添加到内容的关键组件。 Adobe Campaign允许您通过Campaign Web用户界面无缝管理用户档案，从创建新条目到访问所有用户档案属性和服务订阅的全面视图。

此外，在客户端控制台中标识为“种子配置文件”的&#x200B;**[!UICONTROL 测试配置文件]**&#x200B;允许您定位不符合给定投放的定位条件的其他收件人。 这些用户档案包含虚构的联系信息或由发件人控制的联系信息。 测试用户档案是验证收件人：用于通过发送验证来测试消息。 [了解如何使用测试用户档案](test-profiles.md)

用户档案和测试用户档案均可用于在投放到达目标受众之前对其进行测试。 这样，您就可以预览消息内容和个性化，发送验证以进行测试和验证，评估各种平台和设备中的电子邮件渲染情况，并测试您的登陆页面。 [了解如何预览和测试投放](../preview-test/preview-test.md)

➡️[在视频中发现此功能](#video)

## 访问配置文件列表 {#access}

配置文件可通过左侧导航边栏中的&#x200B;**[!UICONTROL 客户管理]** > **配置文件**&#x200B;条目在Adobe Campaign Web中进行访问和编辑。 您还可以在&#x200B;**[!UICONTROL 资源管理器]**&#x200B;视图中，从&#x200B;**[!UICONTROL 配置文件和目标]** > **[!UICONTROL 收件人]**&#x200B;节点访问它们。 从该位置，您可以浏览、创建和管理文件夹或子文件夹，以及检查关联的权限。 [了解如何创建文件夹](../get-started/permissions.md#folders)

>[!NOTE]
>
>根据您的权限，您可能无法访问存储在数据库中的用户档案的完整列表。 [了解有关权限的详细信息](../get-started/permissions.md)。

您可以使用&#x200B;**显示筛选器**&#x200B;按钮中提供的搜索字段或筛选器来筛选&#x200B;**[!UICONTROL 用户档案]**&#x200B;列表。 您可以使用下拉列表将结果限制为特定的[文件夹](../get-started/permissions.md#folders)，或者使用[查询建模器](../query/query-modeler-overview.md)添加规则。

![](assets/profiles-list-filters.png){zoomable="yes"}

要访问配置文件的详细信息，请在列表中单击其名称。 这将打开配置文件的详细视图，允许您浏览其属性以及他订阅的服务。 [了解如何浏览用户档案的详细信息](create-profile.md)

要删除配置文件，请从&#x200B;**[!UICONTROL 更多操作]**&#x200B;菜单中选择相应的选项。

## 操作说明视频 {#video}

了解如何使用Campaign Web用户界面访问、管理和浏览用户档案。

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
