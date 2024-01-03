---
title: 使用收件人和受众
description: 了解如何使用收件人Campaign Web
badge: label="Beta 版"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 34%

---

# 使用收件人和受众 {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="全面查看收件人"
>abstract="创建新的收件人，并通过强大的报告和工具对其进行监控。获取有关收件人属性、交互和日志方面的信息。使用过滤选项浏览收件人列表、编辑和更新其配置文件。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="请参阅发行说明"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="用户档案"
>abstract="配置文件是单个对象，旨在接收 Adobe Campaign 发送的消息。在 Adobe Campaign 中，收件人是发送投放（电子邮件、短信）所针对的默认配置文件。从此列表中可根据您的权限查看收件人的配置文件。使用过滤选项浏览此列表。可编辑和更新收件人的一小部分属性。"

收件人是一个配置文件，旨在接收 Adobe Campaign 发送的消息。在 Adobe　Campaign 中，收件人是发送投放内容（电子邮件、短信等）所定位的默认用户档案。通过数据库中存储的收件人数据，您可以创建将接收任何给定投放的受众，并在投放内容中添加个性化数据。 其他类型的用户档案存储在数据库中。 它们专为不同的用途而设计：例如，种子用户档案用于在将投放内容发送给最终受众之前对其进行测试。

只能从Campaign客户端控制台添加收件人。 但是，它们在Campaign Web中可见，位于 **收件人** 左侧导航栏的条目。 您还可以从该屏幕编辑收件人的属性。

要编辑收件人的数据，请单击其名称旁边的三个圆点，然后选择 **编辑……**.

![编辑收件人配置文件](assets/recipient-edit.png)

您可以更新一组有限的属性，这些属性包括：其名字、姓氏、电子邮件和电话号码。

![更新收件人配置文件](assets/recipient-update.png)

>[!NOTE]
>
>此有限的用户档案编辑表单仅供测试版计划测试使用。 将在未来版本中对其进行改进。 它允许用户将电子邮件地址和电话号码快速添加到任何用户档案，以便他/她可以测试电子邮件和短信渠道并接收发送的消息。

您可以使用搜索字段，从 **显示筛选器** 按钮。

您还可以从访问收件人 **资源管理器** 查看、浏览和创建文件夹和子文件夹，并检查关联的权限。

![资源管理器视图中的收件人列表](assets/recipients-from-explorer.png)

>[!NOTE]
>
>根据您的权限，您可能无法访问存储在数据库中的完整收件人列表。 可在[此部分](../get-started/permissions.md)中详细了解权限。

此外，您还可以管理收件人对服务（如新闻稿）的订阅和退订。 了解如何使用中的订阅服务 [此页面](manage-services.md)

您可以构建工作流以删除重复、扩充、组合用户档案和构建受众。 可在[此小节](../workflows/gs-workflows.md)中了解详情。
