---
audience: end-user
title: 自动投放工作流活动
description: 了解如何使用自动投放工作流活动
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: be38a0d27ae805ac64f0c951e5ea470cd1feb859
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---

# 自动投放 {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="自动投放活动"
>abstract="工作流面板中现在提供了自动投放工作流活动。 您可以用它直接在工作流中创建或执行投放操作（准备、发送验证、准备和启动等）。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="自动投放活动"
>abstract="**自动投放**&#x200B;活动用于自动化：在工作流中创建或重用投放，然后选择要执行的操作（准备、准备和启动、发送验证等）。 您可以选择在工作流之外创建的现有显式投放，或在每次活动运行时从模板创建新投放。"

**自动交付**&#x200B;活动允许您直接在工作流中创建、配置和执行交付操作。 当您要按计划运行预定义交货，或作为自动流的一部分运行，或者当您要在每次活动运行时从模板生成新交货时，使用此模板。

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. 
-->

要配置此活动，请执行以下步骤：

1. 定义投放设置，[了解更多](#delivery-settings)
1. 选择要执行的操作，[阅读更多](#action-to-execute)
1. 设置过渡，[了解更多](#transition-to-execute)
1. 定义修改脚本，[阅读更多](#script)

## 定义投放设置 {#delivery-settings}

配置活动时，您可以选择投放的来源。 本节提供了两个选项：

![显示自动投放的屏幕截图](../assets/automated-delivery.png){zoomable="yes"}

* 当您想要对现有投放执行操作时，例如，选择独立投放或从营销活动创建的投放，请选择&#x200B;**显式投放**。 使用&#x200B;**选择投放**&#x200B;按钮选择投放。 每次工作流运行并到达此活动时，它都会对&#x200B;**相同的**&#x200B;投放执行操作。 每次执行不会创建新投放。 活动会重复使用同一投放。 当您要重复准备或发送单个投放时（例如按计划或批准步骤后），这将很有用。

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* 如果希望每次运行活动时都创建&#x200B;**新**&#x200B;投放，请选择&#x200B;**新建（从模板**&#x200B;创建）。 使用&#x200B;**选择模板**&#x200B;按钮选择投放模板。 每次执行都会根据该模板生成一个新投放。 当每个工作流执行都应导致其自身的独特交付（例如，每次运行一封电子邮件）时，请使用此选项。

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>在过渡&#x200B;**中指定的**&#x200B;和由脚本计算的&#x200B;**选项（用于高级用例）只能在客户端控制台中配置。**&#x200B;请参阅[Campaign v8文档](https://experienceleague.adobe.com/zh-hans/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}。

## 选择要执行的操作 {#action-to-execute}

在此部分中，选择活动对投放执行的操作。 可以使用以下选项：

![显示要在自动投放中执行的操作的屏幕截图](../assets/automated-delivery2.png){zoomable="yes"}

* **保存**：创建并保存投放而不分析或发送。
* **估算目标**：计算投放目标以评估其潜在价值（第一个分析阶段）。
* **准备**：运行完整分析（目标计算和内容准备）。 不发送投放。
* **发送校样**：发送投放的校样。
* **准备并启动**：运行完整分析（目标计算和内容准备）并发送投放。

## 设置过渡 {#transition-to-execute}

利用此部分，可选择是否要在活动后生成过渡。 可以使用以下选项：

![显示自动投放过渡的屏幕截图](../assets/automated-delivery3.png){zoomable="yes"}

* **生成叫客过渡**：活动完成时生成叫客过渡。
* **过渡标签**：允许您自定义画布中过渡上显示的标签。
* **进程错误**：添加用于处理错误的附加转换。

## 定义修改脚本 {#script}

您可以使用脚本更改活动的行为，例如，活动标签等投放参数。 当您需要此活动的自定义逻辑时，请使用此选项。

单击&#x200B;**创建脚本**&#x200B;并在编辑器中编写修改逻辑。

## 相关主题 {#related}

* [关于工作流活动](about-activities.md)
* [持续投放](continuous-delivery.md)
* [电子邮件、短信、推送、直邮活动](channels.md)
* [投放模板](../../msg/delivery-template.md)
