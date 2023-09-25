---
audience: end-user
title: 投放设置
description: 详细了解Campaign Web中的投放设置
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Beta"
source-git-commit: 47cc61510ae0dba139e0cb4d547fc4e737525931
workflow-type: tm+mt
source-wordcount: '2112'
ht-degree: 82%

---


# 投放设置 {#email-del-settings}

电子邮件投放设置包括 **技术投放参数** 在电子邮件模板中定义的电子邮件收件人。 每次投放都会使其过载。

这些设置可从 **配置投放设置** 图标在编辑电子邮件投放或电子邮件投放模板时可用。


## 电子邮件投放设置 {#email-delivery-settings}

>[!CAUTION]
>
>对这些设置的描述仅供参考。其中一些描述取决于您的配置和权限。不得在此版本的产品中修改它们。

## 类型 设置 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="类型"
>abstract="利用类型规则，营销人员可以标准化所有投放中的业务实践。类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。在准备阶段，将从投放受众中排除符合类型规则中的条件的配置文件。"


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="类型 投放设置"
>abstract="利用类型规则，营销人员可以标准化所有投放中的业务实践。类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。在准备阶段，将从投放受众中排除符合类型规则中的条件的配置文件。"


类型是一组 **类型规则**，在准备阶段执行的。 利用类型规则，营销人员可以标准化所有投放中的业务实践。类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。在投放准备阶段，会从投放受众中排除与分类规则中标准匹配的用户档案。  利用分类，可确保电子邮件始终包含特定元素（如退订链接或主题行）或用于从预期目标中排除分组（如未订阅者、竞争对手或不忠诚客户）的筛选规则。

类型规则在类型中分组在一起，以便一次性轻松地将多个筛选规则应用于投放。

将类型与消息或消息模板关联时，将执行在类型中包含的类型规则以便在消息准备期间检查消息的有效性。

![](assets/delivery-settings-1.png)




### 压力参数 {#pressure-parameters}


>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="投放压力参数"
>abstract="利用投放权重，您可以确定疲劳管理框架内的优先级最高的投放。具有最高权重的消息优先。"


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="投放权重"
>abstract="利用投放权重，您可以确定压力管理框架内的优先级最高的投放。具有最高权重的消息优先。"

在本节中，压力参数允许您定义 **阈值** 以设置疲劳管理规则。 这是可在给定时段内发送到一项配置文件的消息最大数量。达到此阈值后，只有在所考虑的时段结束后，才会再进行投放。通过此流程，可在消息数量超过设置的阈值时，自动从投放中排除配置文件，从而避免过度通信。

阈值可以是常量，也可以是变量。这意味着在指定的时间段内，阈值可能因配置文件而异，甚至对于同一配置文件也可能有所不同。

在&#x200B;**权重类型**&#x200B;字段中，有三个可用选项：

* **常量**
* **取决于收件人**
* **在每个规则中定义**

使用&#x200B;**投放权重**&#x200B;字段可定义投放优先级。每个投放都有一个代表其优先级的权重。默认情况下，投放权重设置为 5。压力规则可让您定义它们应用于的投放权重。可以通过公式设置或计算权重以满足收件人的需求。例如，您可以根据收件人兴趣来定义投放权重。


使用&#x200B;**投放模式**&#x200B;字段选择目标评估模式。提供了三种模式：

* **目标估计和消息个性化**
* **暂定目标的估算和审批**
* **目标评估**

**Campaign 优化**&#x200B;附加组件附带了疲劳管理。在中详细了解压力规则以及如何配置疲劳管理 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hans){target="_blank"}.

### 容量设置 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="投放容量设置"
>abstract="在传递消息之前，请使用容量规则来确保您的组织可以处理投放、投放可能生成的集客消息，以及为联系订阅者所要进行的呼叫次数等。容量规则在 Adobe Campaign v8 Console 中定义。在此屏幕中，选择与电子邮件渠道关联的规则。"


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="收件人的重要性"
>abstract="收件人的重要性是一个公式，用于确定在超出容量类型规则时保留的收件人。"


在此部分中，您可以选择在 Adobe Campaign v8 控制台中定义的容量规则。此规则与电子邮件渠道关联。

**收件人的重要性**&#x200B;字段是一个公式，用于确定在超出容量类型规则时保留的收件人。

详细了解一致性和容量规则以及如何在中配置它们 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## 受众设置 {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="投放受众设置"
>abstract="在可用的映射中选择一个&#x200B;**目标映射。**&#x200B;在 Adobe Campaign v8 控制台中定义目标映射。您还为投放设置排除参数。 "

在此部分中，您可以在这些可用的&#x200B;**目标映射**&#x200B;中选择一个。在 Adobe Campaign v8 控制台中定义目标映射。定向维度或目标映射是指操作所处理的数据类型。 它允许您定义目标群体：收件人、合同受益人、操作员、订阅者等。


要了解有关目标映射的更多信息，请参阅 [本节](../audience/about-recipients.md#targeting-dimensions).

## 投放 {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="投放的投放设置"
>abstract="投放参数是应用于投放的技术设置。您可以为投放激活密件抄送，并更改投放和例行模式。这些选项仅供专家用户使用。"

投放参数是应用于投放的技术设置。

* **路由**：默认情况下，将提供集成电子邮件路由外部帐户。其中包含允许应用程序发送电子邮件的技术参数。

* **测试 SMTP 投放**：此选项用于测试通过 SMTP 进行发送。处理投放直至连接到 SMTP 服务器，但不发送：对于投放的每个收件人，Campaign 连接到 SMTP 提供商服务器，执行 SMTP RCPT TO 命令，并在执行 SMTP DATA 命令之前关闭连接。

* **电子邮件密件抄送**：利用此选项，只需将密件抄送电子邮件地址添加到邮件目标，即可通过密件抄送将电子邮件存储在外部系统上。要了解有关电子邮件密件抄送的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

### 网络分析 {#web-analytics}


>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="投放的网站分析设置"
>abstract="选择一个网站分析帐户。此帐户是在 Campaign 客户端控制台中配置的。您还可以定义与您正在使用的分析工具共享的标签。"

在此部分中，您可以选择网站分析帐户。 此帐户是在 Campaign 客户端控制台中配置的。

您还可以定义与您正在使用的分析工具共享的标签。

在中了解有关Web Analytics和Campaign的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.


### 重试 {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="最大重试次数"
>abstract="如果消息因临时错误而失败，则会执行重试，直到投放持续时间结束。"

由于软错误或忽略错误而临时取消发送的邮件将会自动重试。 默认情况下，安排在投放的第一天进行五次重试，最小间隔为一小时分布在一天中的24小时内。

在中了解有关重试管理的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## 审批 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="投放的审批模式"
>abstract="选择审批方式。如果在投放准备期间生成警告，您可以配置投放以定义它是否仍应执行。"


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="投放的审批模式"
>abstract="根据该模板选择投放的审批模式。如果在投放准备期间生成警告，您可以配置投放以定义它是否仍应执行。"

如果在投放准备期间生成警告，您可以配置投放以定义它是否仍应执行。默认情况下，用户必须在分析阶段结束时确认消息的发送：这是&#x200B;**手动**&#x200B;验证。

您可以在相应的字段中选择其他审批方式。可用的模式为：

* **手动**：在分析阶段结束时，用户必须确认投放以开始发送。

* **半自动**：如果分析阶段未生成警告消息，则自动开始发送。

* **自动**：发送在分析阶段结束时自动开始，不管分析结果如何。


## 有效性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="设置有效性"
>abstract="“投放持续时间”字段可让您输入全球投放重试次数的限制。这意味着，Adobe Campaign 从开始日期开始发送消息，然后定期执行可配置的重试（仅针对返回错误的消息），直到达到有效期限。有效期限字段用于上传的资源，例如镜像页面或图像。这些资源在有限的时间内有效：一旦达到限制，资源将不再可用。"



>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="资源有效期限"
>abstract="“有效期限”字段用于已上传的资源，例如镜像页面或图像。这些资源在有限的时间内有效：一旦达到限制，资源将不再可用。"


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="投放持续时间"
>abstract="“投放持续时间”字段可让您输入全球投放重试次数的限制。这意味着，Adobe Campaign 从开始日期开始发送消息，然后对于仅返回错误的消息，将执行定期、可配置的重试，直至达到有效期限。"
<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

**投放持续时间**&#x200B;字段可让您输入全球投放重试次数的限制。这意味着，Adobe Campaign 从开始日期开始发送消息，然后对于仅返回错误的消息，将执行定期、可配置的重试，直至达到有效期限。

您也可以选择指定日期。为此，请选择&#x200B;**明确设置有效期**。在此情况下，也可以使用投放和有效期限日期指定时间。默认情况下使用当前时间，但您可以直接在输入字段中修改此项。

**资源有效期限**&#x200B;字段用于已上传的资源，主要用于镜像页面和图像。本页上的资源仅在限制时间内有效（以节省磁盘空间）。在此限制之后，这些资源将不再可用。

![](assets/delivery-settings-2.png)


在中了解有关投放有效期的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### 镜像页面管理 {#mirror}

镜像页面是可通过 Web 浏览器在线访问的 HTML 页面。其内容与电子邮件的内容相同。默认情况下，如果将链接插入到电子邮件内容中，则会生成镜像页面。

除默认模式外，还提供了以下选项：


* **[!UICONTROL 强制生成镜像页面]**：使用此模式可生成镜像页面，即使在投放时未插入镜像页面的链接也是如此。
* **[!UICONTROL 不生成镜像页面]**：使用此模式可避免生成镜像页面，即使投放中存在链接也是如此。
* **[!UICONTROL 生成仅可使用消息标识符访问的镜像页面]**：当电子邮件内容中不存在镜像页面链接时，使用此选项可启用从客户端控制台在投放日志窗口中访问镜像页面内容的功能。


### 跟踪 {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->




>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="有效期"
>abstract="有效期可设定在消息 URL 上激活跟踪的持续时间。"


在相关部分中定义跟踪参数。可能的选项为：

**跟踪有效期限**：使用此选项可更改在 URL 上激活跟踪的持续时间。

**过期 URL 的替换 URL**：使用此选项可输入后备网页的 URL，它将在跟踪过期后显示。

## 测试设置 {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="投放的测试设置"
>abstract="选择排除参数并自定义测试电子邮件的标签。"

您可以在此部分中设置排除参数。可用的选项为：

* **保持双面**&#x200B;可让您向符合多个定位条件的收件人授权多次投放。

* **保留已列入阻止列表的地址**&#x200B;可让您从目标中保留不再是投放目标的任何配置文件，例如在退订（选择退出）之后。

* **保留隔离地址**&#x200B;可让您从目标中保留任何具有不响应地址的配置文件。

您也可以自定义测试电子邮件的名称。

使用&#x200B;**保留投放代码以作验证**&#x200B;可将测试电子邮件关联到为与其相关的投放定义的相同投放代码。

默认情况下，测试电子邮件的主题以“PROOF #”为前缀，其中#是测试电子邮件的编号。 您可以在&#x200B;**标签前缀**&#x200B;字段中更改此前缀。