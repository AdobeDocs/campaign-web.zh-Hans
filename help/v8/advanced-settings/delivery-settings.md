---
audience: end-user
title: 投放设置
description: 详细了解Campaign Web中的投放设置
feature: Email
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '2429'
ht-degree: 53%

---


# 电子邮件投放设置 {#email-del-settings}

电子邮件投放设置包括 **技术投放参数** 在电子邮件模板中定义的电子邮件收件人。 每次投放都会使其过载。

这些设置可从 **设置** 编辑电子邮件投放或电子邮件投放模板时可用的按钮。

## 电子邮件投放设置 {#email-delivery-settings}

>[!CAUTION]
>
>对这些设置的描述仅供参考。其中一些描述取决于您的配置和权限。不得在此版本的产品中修改它们。

## 类型设置 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="类型"
>abstract="利用类型规则，营销人员可以标准化所有投放中的业务实践。类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。在准备阶段，符合类型规则的配置文件将排除在投放受众之外。在 Campaign 客户端控制台中创建类型和类型规则。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="投放的类型设置"
>abstract="利用类型规则，营销人员可以标准化所有投放中的业务实践。类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。在准备阶段，符合类型规则的配置文件将排除在投放受众之外。在 Campaign 客户端控制台中创建类型和类型规则。"


类型是一组 **类型规则** 以便在准备阶段执行，以便一次性轻松地将多个筛选规则应用于投放。 借助这些工具，营销人员可以标准化所有投放的业务实践，因为他们可以控制、筛选投放投放并安排其发送优先级。

将分类与消息或消息模板关联时，将执行包含在分类中的分类规则，以在消息准备期间检查投放的有效性。 然后，会从投放受众中排除与分类规则中标准匹配的用户档案。

分类功能可确保电子邮件始终包含特定元素（如退订链接或主题行）或用于从预期目标中排除分组（如未订阅者、竞争对手或不忠诚客户）的筛选规则。

![](assets/delivery-settings-typology.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>分类和分类规则是在Campaign客户端控制台中创建的。 在中详细了解压力规则以及如何配置疲劳管理 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=zh-Hans){target="_blank"}.

### 压力参数 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="投放的压力参数"
>abstract="利用投放权重，您可以确定疲劳管理框架内的优先级最高的投放。具有最高权重的消息优先。"


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="投放权重"
>abstract="利用投放权重，您可以确定压力管理框架内的优先级最高的投放。具有最高权重的消息优先。"

在本节中，压力参数允许您定义 **阈值** 以设置疲劳管理规则，疲劳管理规则是在给定时间段内可以发送到一个用户档案的最大消息数。

达到此阈值后，只有在所考虑的时段结束后，才会再进行投放。通过此流程，可在消息数量超过设置的阈值时，自动从投放中排除配置文件，从而避免过度通信。

阈值可以是常量，也可以是变量。这意味着在指定的时间段内，阈值可能因配置文件而异，甚至对于同一配置文件也可能有所不同。

在&#x200B;**[!UICONTROL 权重类型]**&#x200B;字段中，有三个可用选项：

* **[!UICONTROL 常量]**
* **[!UICONTROL 取决于收件人]**
* **[!UICONTROL 在每个规则中定义]**

使用&#x200B;**[!UICONTROL 投放权重]**&#x200B;字段可定义投放优先级。每个投放都有一个代表其优先级的权重。默认情况下，投放权重设置为 5。压力规则可让您定义它们应用于的投放权重。可以通过公式设置或计算权重以满足收件人的需求。例如，您可以根据收件人兴趣来定义投放权重。

使用&#x200B;**[!UICONTROL 投放模式]**&#x200B;字段选择目标评估模式。提供了三种模式：

* **[!UICONTROL 目标估计和消息个性化]**
* **[!UICONTROL 暂定目标的估算和审批]**
* **[!UICONTROL 目标评估]**

>[!NOTE]
>
>疲劳管理是在Campaign客户端控制台中配置的。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hans){target="_blank"}.

### 容量设置 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="投放的容量设置"
>abstract="在传递消息之前，请使用容量规则来确保您的组织可以处理投放、投放可能生成的集客消息，以及为联系订阅者所要进行的呼叫次数等。在 Adobe Campaign v8 控制台中定义容量规则。在此屏幕中，选择与电子邮件渠道关联的规则。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="收件人的重要性"
>abstract="收件人的重要性是一个公式，用于确定在超出容量类型规则时保留的收件人。"


在此部分中，您可以选择在Adobe Campaign v8控制台中定义的容量规则。 此规则与电子邮件渠道关联。

此 **[!UICONTROL 收件人的重要性]** 字段是一个公式，用于确定在超出容量类型规则时保留哪些收件人。

>[!NOTE]
>
>类型规则是在Campaign客户端控制台中配置的。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.

## 受众设置 {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="投放的受众设置"
>abstract="在可用的映射中选择一个&#x200B;**目标映射**。在 Adobe Campaign v8 控制台中定义目标映射。您还设置投放的排除参数。 "

在此部分中，您可以在这些可用的&#x200B;**目标映射**&#x200B;中选择一个。在 Adobe Campaign v8 控制台中定义目标映射。目标映射是操作正在处理的数据类型。 它允许您定义目标群体：收件人、合同受益人、操作员、订阅者等。

要了解有关目标映射的更多信息，请参阅 [本节](../audience/targeting-dimensions.md).

在 **[!UICONTROL 排除项]** 字段中，您可以选择排除不再希望被联系或隔离的收件人。 [了解详情](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## 投放 {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="投放的投放设置"
>abstract="投放参数是应用于投放的技术设置。您可以更改投放和例行模式、激活电子邮件密件抄送、使用批次发送，以及选择已发送电子邮件的格式。 这些选项仅供专家用户使用。"

**[!UICONTROL 投放]** 参数是适用于投放的技术设置。

![](assets/delivery-settings-delivery.png){zoomable=&quot;yes&quot;}

集成的电子邮件 **[!UICONTROL 路由]** 默认提供外部帐户。 其中包含允许应用程序发送电子邮件的技术参数。

您可以定义 **[!UICONTROL 正在发送]** 以下设置。

* **[!UICONTROL 投放优先级]**：使用此选项可通过设置投放的优先级来更改其发送顺序：正常、高或低。

* **[!UICONTROL 消息批次数量]**：使用此选项可定义在同一个XML投放包中分组的消息数。 如果参数设置为0，则消息将自动分组。 程序包大小由计算定义 `<delivery size>/1024`，则每个包最少8条消息，最多256条消息。

  >[!IMPORTANT]
  >
  >通过复制现有投放创建投放时，此参数会重置。

* **[!UICONTROL 测试SMTP投放]**：此选项用于测试通过SMTP进行的发送。 处理投放直至连接到SMTP服务器，但不发送：对于投放的每个收件人，Campaign会连接到SMTP提供商服务器，执行SMTP RCPT TO命令，并在SMTP DATA命令之前关闭连接。

* **[!UICONTROL 电子邮件密送]**：此选项用于通过密件抄送在外部系统上存储电子邮件，只需将密件抄送电子邮件地址添加到消息目标即可。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

在 **[!UICONTROL 波次定义]** 部分，选择 **[!UICONTROL 使用多个批次发送]** 用于逐步增加使用批次发送的数量。 这将避免您的邮件被标记为垃圾邮件或您想要限制每天的邮件数。 利用批次，您可以将投放分为多个批次，而不是同时发送大量消息。 [了解详情](send-using-waves.md)

您也可以更改 **[!UICONTROL 邮件格式]** ，如下所述。

* **[!UICONTROL 使用收件人偏好设置]** （默认模式）

  根据收件人用户档案中存储的数据定义消息格式。 如果收件人希望以特定格式接收消息，则会将该格式用于发送的邮件。如果未填写该字段，则会发送multipart-alternative消息（请参阅下文）。

* **[!UICONTROL 让收件人邮件客户端选择最合适的格式]**

  该消息包含两种格式：文本和HTML。 接收时显示的格式取决于收件人邮件软件的配置(multipart-alternative)。

  >[!IMPORTANT]
  >
  >此选项包括文档的两个版本。 因此，它会影响投放率，因为邮件大小更大。

* **[!UICONTROL 以文本格式发送所有消息]**

  消息以文本格式发送。 不会发送HTML格式，但仅当收件人单击消息时，才会将其用于镜像页面。

## Web 分析 {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="投放的网站分析设置"
>abstract="选择一个网站分析帐户。在 Campaign 客户端控制台中配置此帐户。您还可以定义与您正在使用的分析工具共享的标记。"

在此部分中，您可以选择网站分析帐户。 此帐户是在Campaign客户端控制台中配置的。

您还可以定义与您正在使用的分析工具共享的标记。

>[!NOTE]
>
>可以在Campaign客户端控制台中配置网站分析功能。 了解详情，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## 重试 {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="最大重试次数"
>abstract="如果消息因临时错误而失败，则会执行重试，直到投放持续时间结束。"

<!--Currently not visible in UI > ??-->

由于软错误或忽略错误而临时取消发送的邮件将会自动重试。 默认情况下，安排在投放的第一天进行五次重试，最小间隔为一小时分布在一天中的24小时内。

在中了解有关重试管理的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## 审批 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="投放的审批模式"
>abstract="选择审批模式。如果在准备投放期间产生了警告，则可配置投放以定义是否仍应执行它。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="投放的审批模式"
>abstract="根据此模板选择投放的审批模式。如果在准备投放期间产生了警告，则可配置投放以定义是否仍应执行它。"

如果在投放准备期间生成警告，您可以配置投放以定义它是否仍应执行。默认情况下，用户必须在分析阶段结束时确认消息的发送：这是&#x200B;**手动**&#x200B;验证。

您可以在相应的字段中选择其他审批方式。可用的模式为：

* ****[!UICONTROL 手动]****：在分析阶段结束时，用户必须确认投放以开始发送。

* **[!UICONTROL 半自动]**：如果分析阶段未生成警告消息，则自动开始发送。

* **[!UICONTROL 自动]**：发送在分析阶段结束时自动开始，不管分析结果如何。

## 有效性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="设置有效期"
>abstract="**投放持续时间**&#x200B;字段可让您输入全球投放重试次数的限制。这意味着，Adobe Campaign 从开始日期开始发送消息，然后对于仅返回错误的消息，将执行定期、可配置的重试，直至达到有效期限。<br>**资源有效期限**&#x200B;字段用于已上传的资源，如镜像页面或图像。一旦达到期限，资源将不再可用。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="资源有效期限"
>abstract="**资源有效期限**&#x200B;字段用于已上传的资源，如镜像页面或图像。这些资源在有限的时间内有效：一旦达到限制，资源将不再可用。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="投放持续时间"
>abstract="**投放持续时间**&#x200B;字段可让您输入全球投放重试次数的限制。这意味着，Adobe Campaign 从开始日期开始发送消息，然后对于仅返回错误的消息，将执行定期、可配置的重试，直至达到有效期限。"

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### 有效期 {#validity-period}

**[!UICONTROL 投放持续时间]**&#x200B;字段可让您输入全球投放重试次数的限制。这意味着，Adobe Campaign 从开始日期开始发送消息，然后对于仅返回错误的消息，将执行定期、可配置的重试，直至达到有效期限。

您也可以选择指定日期。为此，请选择&#x200B;**[!UICONTROL 明确设置有效期]**。在此情况下，也可以使用投放和有效期限日期指定时间。默认情况下使用当前时间，但您可以直接在输入字段中修改此项。

**[!UICONTROL 资源有效期限]** 用于已上传的资源，主要用于镜像页面和图像。 本页上的资源仅在限制时间内有效（以节省磁盘空间）。在此限制之后，这些资源将不再可用。

![](assets/delivery-settings-validity.png){zoomable=&quot;yes&quot;}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

在中了解有关投放有效期的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### 镜像页面管理 {#mirror}

镜像页面是可通过 Web 浏览器在线访问的 HTML 页面。其内容与电子邮件的内容相同。默认情况下，如果将链接插入到电子邮件内容中，则会生成镜像页面。

除默认模式外，还提供了以下选项：

* **[!UICONTROL 强制生成镜像页面]**：使用此模式可生成镜像页面，即使投放中未插入指向镜像页面的链接也是如此。
* **[!UICONTROL 不生成镜像页面]**：使用此模式可避免生成镜像页面，即使投放中存在链接也是如此。
* **[!UICONTROL 生成仅可使用消息标识符访问的镜像页面]**：如果电子邮件内容中不存在镜像页面链接，请使用此选项启用从客户端控制台在投放日志窗口中访问镜像页面内容的功能。


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

**[!UICONTROL 跟踪]** 参数在相关部分中定义。 可能的选项为：

**[!UICONTROL 跟踪有效期限制]**：使用此选项可更改在URL上激活跟踪的持续时间。

**[!UICONTROL 过期URL的替换URL]**：使用此选项可输入回退网页的URL：跟踪过期后即会显示。

## 校样设置 {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="定义投放的校样设置"
>abstract="选择排除参数并自定义校样的标签。"

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

您可以在此部分中设置排除参数。可用的选项为：

* ****[!UICONTROL 保持双面]**** 可让您授权向满足多个定位标准的收件人进行多次投放。

* **[!UICONTROL 保留已列入阻止列表的地址]**&#x200B;可让您从目标中保留不再是投放目标的任何配置文件，例如在退订（选择退出）之后。

* **[!UICONTROL 保留隔离地址]**&#x200B;可让您从目标中保留任何具有不响应地址的配置文件。

您还可以自定义校样的标签：

* 使用 **[!UICONTROL 保留投放代码以作验证]** 将为其相关的投放定义的投放代码与相同的投放代码关联到证明。

* 默认情况下，验证的主题的前缀为“PROOF #”，其中#是验证的编号。 您可以在&#x200B;**[!UICONTROL 标签前缀]**&#x200B;字段中更改此前缀。