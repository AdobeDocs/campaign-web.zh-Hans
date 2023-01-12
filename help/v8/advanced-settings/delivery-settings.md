---
audience: end-user
title: 电子邮件投放设置
description: Campaign v8 Web文档
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: ed814fbb9d3f9daeb725f44a7a1929217d1d48d2
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 14%

---

# 电子邮件投放设置 {#email-del-settings}

![](../assets/do-not-localize/badge.png)

这些设置包括 **技术交付参数** 在电子邮件模板中定义的附加内容。

## 电子邮件投放设置 {#email-delivery-settings}

>[!CAUTION]
>
> 这些设置仅供您参考。 其中某些权限取决于您的配置和权限。 不得在此版本的产品中修改它们。

## 类型 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="类型"
>abstract="利用分类，可控制、过滤和监控投放的发送。"

分类是在消息分析阶段执行的一系列&#x200B;**分类规则**。利用分类，可确保电子邮件始终包含特定元素（如退订链接或主题行）或用于从预期目标中排除分组（如未订阅者、竞争对手或不忠诚客户）的筛选规则。

当将分类与消息或消息模板关联时，执行包括在分类中的分类规则以在消息准备期间检查消息的有效性。

![](assets/delivery-settings-1.png)


### 压力参数 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="投放权重"
>abstract="投放权重允许您确定压力管理框架内优先级最高的投放。 权重最高的消息具有优先级。"

在此部分中，压力参数允许您定义 **阈值**. 这是指定时间段内可向一个用户档案发送的消息数量上限。 达到此阈值后，只有在所考虑的时段结束后，才会再进行投放。通过此流程，可在消息数量超过设置的阈值时，自动从投放中排除用户档案，从而避免过度通信。

阈值可以是常量，也可以是变量。这意味着在指定的时间段内，阈值可能因用户档案而异，甚至对于同一用户档案也可能有所不同。

在 **粗细类型** 字段中，提供了三个选项：

* **常量**
* **取决于收件人**
* **在每个规则中定义**

使用 **交付重量** 字段来定义投放优先级。 每个投放都有一个权重，该权重表示其优先级级别。 默认情况下，投放的权重设置为5。 压力规则允许您定义要应用于的投放的权重。权重可以通过公式设置或计算，以适合收件人。 例如，您可以根据收件人兴趣定义投放的权重。


使用 **投放模式** 字段来选择目标评估模式。 提供了三种模式：

* **目标估计和消息个性化**
* **暂定目标的估算和审批**
* **目标评估**

疲劳管理随 **促销活动优化** 附加组件。 详细了解压力规则以及如何在 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hans){target="_blank"}.

### 容量设置 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="收件人的重要性"
>abstract="收件人的重要性是一个公式，用于确定在超出容量分类规则时保留哪些收件人。"

在此部分中，您可以选择在Adobe Campaign v8控制台中定义的容量规则。 此规则与电子邮件渠道关联。

的 **收件人的重要性** 字段是一个公式，用于确定在超出容量分类规则时保留哪些收件人。

了解有关一致性和容量规则以及如何在 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## 受众 {#audience}

在此部分中，您可以选择 **目标映射** 其中包括。 目标映射在Adobe Campaign v8控制台中定义。

了解有关 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## 投放 {#delivery}

投放参数是适用于您的投放的技术设置。

* **路由**:默认情况下，会提供集成的电子邮件路由外部帐户。 其中包含允许应用程序发送电子邮件的技术参数。

* **测试SMTP投放**:此选项用于测试通过SMTP发送的内容。 投放会一直处理到与SMTP服务器的连接，但不会发送：对于投放的每个收件人，Campaign会连接到SMTP提供程序服务器，执行SMTP RCPT TO命令，然后在SMTP DATA命令之前关闭连接。

* **电子邮件密送**:此选项仅通过向消息目标添加密件抄送电子邮件地址，用于通过密件抄送在外部系统上存储电子邮件。 在中了解有关电子邮件密件抄送的更多信息 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### 重试 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="最大重试次数"
>abstract="如果消息因临时错误而失败，则会在投放持续期间执行重试。"

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

了解有关重试管理的更多信息，请参阅 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## 审批 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="审批方式"
>abstract="投放的每个步骤都可获得批准，以确保对各个流程进行全面监控和控制。"

如果在投放准备期间生成警告，则可以配置投放以定义是否应仍执行该投放。 默认情况下，用户必须在分析阶段结束时确认消息的发送：此为 **手动** 验证。

您可以在相应的字段中选择其他批准模式。 可用模式包括：

* **手动**:在分析阶段结束时，用户必须确认投放以开始发送。

* **半自动**:如果分析阶段未生成警告消息，则自动开始发送。

* **自动**:发送在分析阶段结束时自动开始，而不管其结果如何。


## 有效性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="投放持续时间"
>abstract="利用投放持续时间字段，可输入全局投放重试的限制。 这意味着Adobe Campaign从开始日期开始发送消息，然后，对于仅返回错误的消息，会执行常规的可配置重试，直到达到有效性限制为止。"

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="资源有效期限"
>abstract="“有效性限制”字段用于已上传的资源，主要用于镜像页面和图像。 此页面上的资源在有限的时间内有效。"


的 **投放持续时间** 字段允许您输入全局投放重试的限制。 这意味着Adobe Campaign从开始日期开始发送消息，然后，对于仅返回错误的消息，会执行常规的可配置重试，直到达到有效性限制为止。

您还可以选择指定日期。 要执行此操作，请选择 **明确设置有效日期**. 在这种情况下，投放和有效期限制日期还允许您指定时间。 默认使用当前时间，但您可以直接在输入字段中修改此时间。

**资源有效性限制** 用于已上传的资源，主要用于镜像页面和图像。 本页上的资源仅在限制时间内有效（以节省磁盘空间）。

![](assets/delivery-settings-2.png)


了解有关投放有效期的更多信息(位于 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### 镜像页面管理 {#mirror}

镜像页面是可通过Web浏览器在线访问的HTML页面。 其内容与电子邮件相同。 默认情况下，如果将链接插入到邮件内容中，则会生成镜像页面。

除了默认模式之外，还提供以下选项：

* **[!UICONTROL 强制生成镜像页面]**:即使投放中未插入指向镜像页面的链接，也会创建镜像页面。
* **[!UICONTROL 不生成镜像页面]**:即使投放中存在链接，也不会生成镜像页面。
* **[!UICONTROL 生成仅使用消息标识符可访问的镜像页面]**:此选项允许您在投放日志窗口中访问包含个性化信息的镜像页面的内容。 为此，在投放结束后，单击 **[!UICONTROL 投放]** 选项卡上，选择要查看其镜像页面的收件人行。 单击 **[!UICONTROL 显示此消息的镜像页面……]** 链接。


### 跟踪 {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="有效期"
>abstract="此选项定义在URL上激活跟踪的持续时间。"

跟踪参数在相关部分中定义。 可能的选项包括：

**跟踪有效性限制**:使用此选项可更改在URL上激活跟踪的持续时间。

**过期URL的替换URL**:使用此选项可输入回退网页的URL:跟踪过期后，将显示该标记。

## 测试设置 {#test-setttings}

您可以在此部分中设置排除参数。 可用选项包括：

* **保持双倍** 允许您向满足多个定位标准的收件人授权多个投放。

* **保留列入阻止列表地址** 允许您从目标中保留任何不再被投放定向的用户档案，例如在退订（选择退出）后。

* **保留隔离的地址** 允许您从目标中保留任何地址未响应的用户档案。

您还可以自定义校样的名称。

使用 **保留校样的投放代码** 将与校样关联的投放代码与为与之关联的投放定义的交付代码相关联。

默认情况下，校样的主题以“PROOF #”为前缀，其中#是校样的编号。 您可以在 **标签前缀** 字段。