---
audience: end-user
title: 工作流事件变量
description: 了解如何在工作流中利用事件变量。
source-git-commit: 313b5688eee169612007b9704036ce1d8b89dd86
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# 工作流事件变量 {#event-variables}

某些工作流活动允许您在表达式编辑器中编辑脚本以执行特定操作，例如检索来自先前活动的数据、构建条件或根据事件变量计算文件名。

## 什么是事件变量 {#scripting}

在工作流上下文中执行的脚本访问一系列其他全局 **对象** 例如正在执行的工作流本身(`ìnstance`)，其各种任务(`task`)，或激活给定任务的事件(`event`)。

到每种类型 **对象** 与以下类别关联： **变量** 在编辑活动（例如）中的脚本时，可在表达式编辑器中利用的区段 **[!UICONTROL JavaScript代码]** 或 **[!UICONTROL 测试]**.

* **实例变量** (`instance.vars.xxx`)与全局变量具有可比性。 所有活动都共享它们。
* **任务变量** (`task.vars.xxx`)与局部变量具有可比性。 它们仅由当前任务使用。 这些变量由永久性活动用来保留数据，有时也用于在同一活动的不同脚本之间交换数据。
* **事件变量** (`vars.xxx`)支持在工作流进程的基本任务之间交换数据。 这些变量由激活正在进行的任务的任务传递。 然后，它们会被传递到以下活动。 **事件变量** 是最常用的变量，应该优先使用它们而不是实例变量。

>[!NOTE]
>
>有关脚本以及Adobe Campaign中公开的对象和变量的其他信息，请参阅Campaign v8（客户端控制台）文档中的 [本节](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>请注意，虽然此资源提供了有价值的分析，但可能存在差异，因为它具体适用于客户端控制台，而不是Campaign Web用户界面。

## 在表达式编辑器中利用事件变量 {#expression-editor}

预定义事件变量可用于表达式编辑器左侧窗格。 您也可以通过在代码中初始化新变量来创建新变量。

![](assets/event-variables.png)

除了这些事件变量之外，您还可以利用 **[!UICONTROL 条件]** 菜单来构建条件和 **[!UICONTROL 添加当前日期]** 菜单，用于使用与日期格式相关的函数。
