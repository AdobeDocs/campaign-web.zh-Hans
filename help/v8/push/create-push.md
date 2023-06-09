---
audience: end-user
title: 创建推送通知投放
description: 了解如何使用Adobe Campaign Web创建推送通知投放
badge: label="Alpha" type="Positive"
source-git-commit: b18fb70aa498e3592f88f698bb6b526c9fb1439b
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 68%

---

# 创建推送通知投放 {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="定义推送受众"
>abstract="选择最适合您的推送消息的受众。"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="推送通知模板"
>abstract="选择推送通知模板以开始推送投放。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="推送投放属性"
>abstract="管理推送投放属性。"

1. 从&#x200B;**[!UICONTROL 投放]**&#x200B;主页上单击&#x200B;**[!UICONTROL 创建投放]**。

1. 在 **[!UICONTROL 渠道]** 部分，选择推送通知作为渠道，并根据所选的操作系统(Android或iOS)选择模板。 [详细了解模板](../msg/delivery-template.md)

1. 单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮以进行确认。

   ![](assets/push_create_1.png)

1. 输入投放的&#x200B;**[!UICONTROL 标签]**&#x200B;并访问&#x200B;**[!UICONTROL 其他选项]**&#x200B;下拉列表。

   +++根据您的要求配置以下设置。
   * **[!UICONTROL 内部名称]**：为投放分配一个唯一标识符。
   * **[!UICONTROL 文件夹]**：将投放存储在特定文件夹中。
   * **[!UICONTROL 投放代码]**：使用您自己的命名惯例整理投放。
   * **[!UICONTROL 描述]**：提供投放的描述。
   * **[!UICONTROL 性质]**：指定电子邮件的性质以进行分类。
+++

1. 从 **[!UICONTROL Audience]** 菜单，选择要用于此投放的应用程序。

1. 单击&#x200B;**[!UICONTROL 选择受众]**&#x200B;按钮以现有受众为目标或创建您自己的受众。[了解详情](../audience/about-audiences.md)

   请注意，默认情况下，您的推送通知将发送给应用程序的所有订阅者。

   ![](assets/push_create_2.png)

1. 开启&#x200B;**[!UICONTROL 启用对照组]**&#x200B;选项以设置对照组以衡量投放的作用，并使您可比较收到消息的人群的行为与未收到消息的联系人的行为。[了解详情](../audience/control-group.md)

1. 单击 **[!UICONTROL 编辑内容]** 以开始设计推送通知的内容。

1. 要安排在特定的日期和时间投放，请开启&#x200B;**[!UICONTROL 启用计划]**&#x200B;选项。开始投放后，将在您为收件人定义的确切日期和时间自动发送消息。

   ![](assets/push_create_3.png)

1. 单击 **[!UICONTROL 配置投放设置]** 访问与投放模板相关的高级选项。 [了解详情](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
