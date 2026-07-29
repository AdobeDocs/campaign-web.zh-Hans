---
audience: end-user
title: 开始使用选件管理
description: 了解如何在Adobe Campaign Web中管理优惠
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 763
ht-degree: 3%

---

# 开始使用选件管理 {#gs-offer-management}

此功能可让您向投放添加个性化优惠，并针对给定上下文中的每个用户档案显示最相关的优惠。 选件可以是一条简单的通信消息，也可以是一款或多款产品上的促销活动。 根据资格规则和优先级权重，优惠引擎会选择要呈现的最佳建议。

通过Campaign Web用户界面，您可以对优惠进行端到端管理。 您可以创建和配置优惠环境、设计优惠空间、构建优惠目录、设置资格规则、编辑优惠内容和发布优惠。

然后根据&#x200B;**资格规则**&#x200B;和&#x200B;**优先级权重**&#x200B;通过投放将优惠呈现给收件人，以便在给定的上下文中为每个用户档案选择最佳优惠。

>[!NOTE]
>
>Campaign Web用户界面侧重于最常见的选件管理用法。 高级配置在Campaign客户端控制台中仍然可用。 请参阅[Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=zh-Hans){target="_blank"}

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## 重要概念 {#concepts}

在开始使用选件之前，请熟悉所涉及的主要对象。

* **优惠环境** — 包含优惠目录和相关优惠空间的容器。 有两种类型，即&#x200B;**设计**&#x200B;环境和只读&#x200B;**[!UICONTROL 实时]**&#x200B;环境，前者用于创建和配置选件，后者包含可供交付的已批准和已部署对象。 [了解详情](offer-environment.md)

* **优惠空间** — 定义优惠的公开位置和方式（电子邮件、直邮、短信、入站Web等）。 此空格列出了可在优惠中使用的内容字段、构建优惠表示的渲染函数，以及驱动建议状态的存储设置。 [了解详情](offer-space.md)

* **优惠目录和类别** — 优惠按&#x200B;**类别**&#x200B;和子类别的分层目录组织。 每个类别可以共享资格规则、有效日期和&#x200B;**应用程序主题**。 设计环境中提供了一个默认类别来接收所有选件。

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **选件** — 具有自己的资格期限、目标筛选器、权重和内容的单个选件。 在向收件人展示优惠之前，会批准并部署优惠。 [了解详情](create-offer.md)

* **优惠建议** — 在给定空间（网站上的横幅、电子邮件、短信等）向联系人展示优惠的结果。 当[在投放](../msg/offers.md)中设置选件时，会配置每个投放的建议数量。

* **套利** — 优惠引擎按优先级对合格优惠进行排名以选择要显示的优惠的原则。 套利使用在类别、选件和上下文选件上定义的标准。

## 选件管理流程 {#workflow}

Campaign Web UI中的典型端到端流程如下：

1. **查看优惠环境设置** — 检查设计/实时映射、资格和权重管理设置。 [了解详情](offer-environment.md)

1. **创建优惠空间** — 定义与渠道匹配的内容字段、渲染函数和高级参数。 [了解详情](offer-space.md)

1. **在目录中创建选件** — 设置每个选件的资格期限、目标筛选器、权重和内容。 [了解详情](create-offer.md)

1. **批准和部署** — 提交优惠以供批准，批准其内容和资格，然后让部署过程将其发布到实时环境。 [了解详情](create-offer.md#approve-deploy)

1. **将优惠添加到投放** — 引用优惠空间以及电子邮件、短信、推送或直邮投放中的建议。 [了解详情](../msg/offers.md)

## 访问Web UI中的选件 {#access}

可从左侧菜单&#x200B;**[!UICONTROL 选件]**&#x200B;中获得选件。 在此处，您可以浏览目录、打开选件进行编辑，并监控其批准和部署状态。

![显示“选件”菜单的屏幕截图。](assets/offers-gs.png){zoomable="yes"}

通过&#x200B;**[!UICONTROL Explorer]**，导航到相应的文件夹来访问优惠环境和优惠空间。


## 仅控制台补充 {#console-complements}

某些选件功能尚未在Web用户界面中公开，仍必须从客户端控制台进行配置：

* **优惠模拟** — **Simulation**&#x200B;模块，允许您在发送之前测试优惠的分布。 查看[优惠模拟](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html#offer-simulation){target="_blank"}。

* **预定义过滤器**&#x200B;管理 — 可从任何选件引用的可重用过滤器规则。 请参阅[管理预定义过滤器](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}。

* **优惠跟踪** — 配置优惠建议的跟踪以馈送建议历史记录。 查看[跟踪优惠建议](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html){target="_blank"}。

* **操作员角色** — 分配选件管理器/投放管理器权限。 查看交互模块[&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}的操作员。

* **交互最佳实践和套利规则**。 请参阅[Campaign交互最佳实践](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}。

* **报告** — Web用户界面中尚未提供专用的优惠和建议报告。