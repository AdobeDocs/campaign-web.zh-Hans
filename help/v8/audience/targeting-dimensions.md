---
title: 目标选择维度
description: 了解有关在Adobe Campaign Web中定位维度的更多信息
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 5%

---

# 目标选择维度 {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Select the targeting dimension"
>abstract="The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, and more. By default, for emails and SMS, the target is selected from the Recipients built-in table. For Push notifications, the default target dimension is Subscriber applications."

## 工作流的定位维度 {#workflow}

工作流的定向维度由前&#x200B;**[!UICONTROL 构建受众]**&#x200B;活动定义，并用于所有后续活动，直到工作流结束。 例如，从数据库查询用户档案时，出站过渡包含“recipient”类型的数据，该数据将传输到下一个活动。

使用[更改维度活动](../workflows/activities/change-dimension.md)切换工作流中的定向维度。 这允许查询特定表（如购买或订阅）上的数据库，然后更改定向维度给收件人，以将投放发送到相应的用户档案。

在选择定向维度时（在工作流设置中或在诸如&#x200B;**构建受众**、**协调**&#x200B;或&#x200B;**更改维度**&#x200B;等活动中），默认情况下会显示常用架构的列表。 要显示所有可用的架构，请切换&#x200B;**[!UICONTROL 显示所有架构]**&#x200B;按钮。 将为每个用户保存选项选择。

![显示启用了“显示所有架构”按钮的定位维度界面的屏幕截图。](assets/targeting-dimension-show-all.png){zoomable="yes"}

## 目标选择维度 {#list}

默认情况下，电子邮件和短信投放模板会定向用户档案。 他们的目标维度使用&#x200B;**nms：recipient**&#x200B;表的字段。 对于推送通知，默认目标维度为链接到收件人表的&#x200B;**订阅者应用程序nms：appSubscriptionRcp**。

在工作流和投放中使用其他内置目标映射，如下所示：

| 名称 | 使用投放 | 架构 |
|-----------------------|-------------------------------------------------------|-------------------------|
| 收件人 | 用户档案/收件人（内置收件人表） | nms：recipient |
| 访客 | 通过反向链接收集用户档案的访客（例如，病毒式营销） | mns：visitor |
| 订阅 | 订阅新闻稿等信息服务的用户档案 | nms：subscription |
| 访客订阅 | 订阅了信息服务的访客 | nms：visitorSub |
| 运算符 | Adobe Campaign运算符 | nms：operator |
| 外部文件 | 通过包含所有必需信息的文件投放 | 无链接架构，未输入目标 |
| 订阅者应用程序 | 订阅应用程序的配置文件 | nms：appSubscriptionRcp |

此外，根据特定需求创建新的目标映射。 仅从客户端控制台执行此操作。 请参阅[Campaign v8 （客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}以了解详情。