---
audience: end-user
title: 创建和管理优惠空间
description: 了解如何在Campaign Web中创建、配置、部署和预览优惠空间
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 921
ht-degree: 0%

---

# 创建和管理优惠空间 {#offer-space}

**优惠空间**&#x200B;定义优惠向联系人公开的位置和方式：它使用的渠道（电子邮件、直邮、短信、入站Web等）、优惠可以使用的内容字段以及构建最终呈现的方式。 单个环境可以包含多个选件空间 — 每个展示点对应一个选件空间。

优惠空间本身不是渠道。 它表示选件在渠道上显示的特定位置。 同一网页上的两个横幅通常对应于两个不同的优惠空间。 有关完整的概念模型，请参阅[Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}。

## 创建或修改选件空间{#create-offer-space}

选件空间存储在选件环境文件夹下。 要浏览您的平台上可用的优惠空间，请打开&#x200B;**[!UICONTROL 资源管理器]**，导航到优惠环境并选择包含这些优惠空间的子文件夹。

![显示优惠空间列表的屏幕截图。](assets/offers-space.png){zoomable="yes"}

从该位置，您可以打开现有优惠空间，或单击&#x200B;**[!UICONTROL 创建优惠空间]**&#x200B;以创建新优惠空间。

![显示优惠空间屏幕的屏幕截图。](assets/offers-space-1.png){zoomable="yes"}

### 定义属性 {#properties}

此部分允许您：

* 为优惠空间输入&#x200B;**[!UICONTROL 标签]**。
* 选择与展示点（电子邮件、直邮、短信、Web等）匹配的&#x200B;**[!UICONTROL 渠道]**。
* 如果此优惠空间除了批量投放调用外，还必须支持对优惠引擎的单一（实时、单一优惠）调用，请选择&#x200B;**[!UICONTROL 启用单一模式]**。

### 定义内容字段 {#content-fields}

内容字段列出了可在选件级别编辑并由渲染函数重用的属性。 您在选件空间中添加字段的顺序将驱动它们在选件&#x200B;**[!UICONTROL 内容]**&#x200B;部分中显示的顺序。

默认情况下，每个选件都附带以下现成的内容字段：**[!UICONTROL 标题]**、**[!UICONTROL 目标URL]**、**[!UICONTROL 图像URL]**、**[!UICONTROL HTML内容]**&#x200B;和&#x200B;**[!UICONTROL 文本内容]**。 您可以使用渲染所需的任何自定义字段扩展此列表 — 例如，**短内容**、**跟踪的URL**&#x200B;或通过架构扩展添加的任何属性。

单击&#x200B;**[!UICONTROL 添加内容字段]**，然后选择要从选件架构中公开的属性，或单击&#x200B;**[!UICONTROL 编辑表达式]**&#x200B;以定义自定义表达式。

>[!IMPORTANT]
>
>若要使自定义属性可从选件&#x200B;**[!UICONTROL 内容]**&#x200B;部分中编辑，还必须在[!DNL nms:offer]架构的&#x200B;**[!UICONTROL 选件内容]**&#x200B;部分中声明该属性。 在[使用架构](../administration/schemas.md)中了解详情。

### 配置渲染函数 {#rendering}

渲染函数从内容字段构建最终优惠表示形式。 您可以选择默认呈现（仅按原样输出内容）或将字段与HTML、XML或文本组合在一起的自定义函数。

选择&#x200B;**[!UICONTROL HTML渲染]**、**[!UICONTROL XML渲染]**&#x200B;或&#x200B;**[!UICONTROL 文本渲染]**&#x200B;选项卡，并启用&#x200B;**[!UICONTROL 重载渲染函数]**&#x200B;以激活它。

使用表达式编辑器编写渲染函数。 您可以引用[表达式编辑器](../query/expression-editor.md)中定义的内容字段、选件属性和任何函数。

>[!NOTE]
>
>如果未定义渲染函数，则使用现成的属性按原样返回选件内容。 只有在优惠空间上选择了&#x200B;**[!UICONTROL 启用单一模式]**&#x200B;时，才能使用XML渲染函数。

### 配置存储和建议状态 {#storage}

在此部分中，您可以控制如何持久保留通过此空间生成的建议，以及建议状态在整个生命周期中如何演变：

* **[!UICONTROL 禁用建议插入]** — 阻止通过此优惠空间生成的建议插入到建议存储表中。

* 建议的&#x200B;**[!UICONTROL 状态]** — 优惠引擎返回建议时应用于该建议的状态（通常为出站投放的&#x200B;**[!UICONTROL Presented]**）。

* 接受时&#x200B;**[!UICONTROL 状态]** — 收件人与优惠交互时应用的状态（通常为&#x200B;**[!UICONTROL 已接受]**）。

可用的状态值与Client Console使用的列表相匹配。 有关详细信息，请参阅控制台文档中的[Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"}。

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### 配置高级设置 {#advanced}

此部分允许您定义&#x200B;**[!UICONTROL 目标标识]**。 单击“添加”**&#x200B;**&#x200B;并选择一或多个&#x200B;**[!UICONTROL 收件人]**&#x200B;属性，或单击“编辑表达式”**[!UICONTROL 以定义自定义表达式]**。 对于基本选件空间，此设置是可选的。 有关其完整引用和行为，请参阅[Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}。

在&#x200B;**入站Web渠道**&#x200B;上创建的优惠空间，还需要将网站配置为显示优惠并调用优惠引擎。 此集成在客户端控制台中执行 — 请参阅Campaign v8文档中的[实时显示优惠](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"}和[配置优惠引擎集成](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"}。

## 部署优惠空间 {#deploy}

必须先部署优惠空间，然后才能在投放中使用。 保存优惠空间，然后单击&#x200B;**部署**。 部署的状态会反映在优惠空间上。

![显示优惠部署的屏幕截图。](assets/offers-space-2.png){zoomable="yes"}

## 预览优惠空间 {#preview}

预览可让您模拟如何为给定目标选择和呈现选件。

1. 从优惠空间中，选择&#x200B;**[!UICONTROL 概述]**&#x200B;旁边的&#x200B;**[!UICONTROL 预览]**&#x200B;选项卡。

   ![显示优惠预览的屏幕截图。](assets/offers-space-3.png){zoomable="yes"}

1. 选择目标配置文件并运行预览。 匹配的选件将随渲染函数生成的表示法一起返回。

>[!NOTE]
>
>如果未返回建议，请检查优惠的资格规则和空间的配置。

接下来，[在目录中创建选件](create-offer.md)，并将其分配给此共享空间。
