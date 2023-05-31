---
audience: end-user
title: 使用工作流活动
description: 了解如何工作流活动
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: acc3f2cdc50fc8727a472d427c2f8077775a8744
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 74%

---


# 工作流活动 {#workflow-activities}

## 定位活动 {#targeting}

内容待定

<!--à reformuler-->利用这些活动，您可以通过定义集合并使用交集、并集或差集操作来拆分或合并这些集合，从而构建一个或多个目标。

### 构建受众 {#build-audience}

### 结合 {#combine}

## 渠道活动 {#channel}

通过Adobe Campaign Web，您可以跨多个渠道（如电子邮件、短信或推送）自动执行营销活动。 借助Adobe Campaign工作流，您可以将渠道活动合并到画布中，以创建可根据客户行为触发操作的跨渠道工作流。

例如，您可以创建一个欢迎电子邮件促销活动，其中包含跨不同渠道的一系列消息，例如电子邮件、短信和推送。 您还可以在客户完成购买后发送跟进电子邮件，或通过短信向客户发送个性化的生日消息。

通过使用渠道活动，您可以创建全面的个性化营销活动，在多个接触点吸引客户并促进转化。

渠道活动可从屏幕左侧的面板的“渠道”部分中使用。

### 电子邮件 {#email}

描述，可以执行哪个用例（可以在活动前后链接的其他常见活动）

如何添加和配置活动

工作流中已配置活动的示例


利用电子邮件投放活动，可在工作流中配置发送电子邮件。

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

同一工作流中的上游活动，通过受众定位活动定义了电子邮件收件人。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### 短信 {#sms}

### 推送通知 (Android) {#push-android}

### 推送通知 (iOS) {#push-ios}

## 流量控制活动 {#flow-control}

内容待定

<!--à reformuler-->利用这些活动，您可以通过定义集合并使用交集、并集或差集操作来拆分或合并这些集合，从而构建一个或多个目标。

流量控制活动用于协调工作流活动。

### 分叉 {#fork}

### AND-连接 {#end}


### 等待 {#end}

### 结束 {#end}

## 数据管理活动 {#data-management}

概述：它们的用途
可以使用它们执行哪些用例

列出可用活动 + 简短描述 + 参考章节

### 扩充 {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="扩充活动"
>abstract="扩充活动可让您使用数据库中的其他信息来增强目标数据。它通常用于定位活动之后的工作流中。<br/>在将扩充数据添加到工作流中后，可以在扩充活动后添加的活动中使用它，以根据客户的行为、偏好和需求来将客户分成不同的组，或者创建更可能让目标受众产生共鸣的个性化营销邮件和营销活动。"

扩充活动可让您使用数据库中的其他信息来增强目标数据。它通常用于定位活动之后的工作流中。

扩充数据可来自：

* **同一个工作表**，此工作表与工作流中的目标工作表相同：

   *定位一组客户，并将“出生日期”字段添加到当前工作表*

* **另一个工作表**：

   *定位一组客户，并添加“采购”表中的“金额”和“产品类型”字段*。

在将扩充数据添加到工作流中后，可以在扩充活动后添加的活动中使用它，以根据客户的行为、偏好和需求来将客户分成不同的组，或者创建更可能让目标受众产生共鸣的个性化营销邮件和营销活动。

例如，可以将与客户购买相关的信息添加到工作流工作表中，并使用此数据来个性化包含客户最近一次购买或在这些购买中花费的金额的电子邮件。

要将扩充活动添加到工作流，请执行以下步骤：

1. 添加活动
1. 选择要用作扩充数据的属性

   显示高级字段选项
i 按钮

   注意：来自目标维度的属性

1. 选择数据收集方式
1. 要检索的记录数（如果要检索多条记录的集合）
1. 应用筛选器和生成规则

   选择现有筛选器
保存筛选器以便重用
以可视方式或在代码视图中查看筛选器的结果

1. 使用属性对记录进行排序

在营销活动中利用扩充数据

我们可以在何处使用扩充数据：个性化电子邮件，其他用例？
