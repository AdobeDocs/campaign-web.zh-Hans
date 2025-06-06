---
audience: end-user
title: 工作流事件变量
description: 了解如何在工作流中利用事件变量。
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# 工作流事件变量 {#event-variables}

某些工作流活动允许您在表达式编辑器中编辑脚本以执行特定操作，例如，从以前的活动中检索数据、构建条件或基于事件变量计算文件名。

## 什么是事件变量 {#scripting}

在工作流上下文中执行的脚本访问一系列其他全局&#x200B;**对象**，例如正在执行的工作流本身(`instance`)、其各种任务(`task`)或激活给定任务(`event`)的事件。

**对象**&#x200B;的每个类型都与&#x200B;**变量**&#x200B;的类别相关联，在编辑活动中的脚本时，可在表达式编辑器中使用该类别，例如&#x200B;**[!UICONTROL JavaScript代码]**&#x200B;或&#x200B;**[!UICONTROL 测试]**。

* **实例变量** (`instance.vars.xxx`)与全局变量类似。 所有活动都共享它们。
* **任务变量** (`task.vars.xxx`)可与局部变量比较。 它们仅由当前任务使用。 这些变量由永久性活动用来保留数据，有时也用于在同一活动的不同脚本之间交换数据。
* **事件变量** (`vars.xxx`)允许在工作流进程的基本任务之间交换数据。 这些变量由激活正在进行的任务的任务传递。 然后，它们会被传递到以下活动。 **事件变量**&#x200B;是最常用的变量，应优先使用它们而不是实例变量。

>[!NOTE]
>
>有关脚本以及Adobe Campaign中公开的对象和变量的其他信息，请参阅[此部分](https://experienceleague.adobe.com/zh-hans/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates)中的Campaign v8 （客户端控制台）文档。
>
>请注意，虽然此资源提供了有价值的分析，但可能存在差异，因为它具体适用于客户端控制台，而不是Campaign Web用户界面。

## 在表达式编辑器中利用事件变量 {#expression-editor}

预定义的事件变量可在表达式编辑器的左侧窗格中使用。 您也可以通过在代码中初始化新变量来创建新变量。

![在表达式编辑器的左侧窗格中显示预定义事件变量的屏幕截图](assets/event-variables.png)

除了这些事件变量之外，您还可以使用左窗格中的&#x200B;**[!UICONTROL 条件]**&#x200B;菜单来构建条件，并使用&#x200B;**[!UICONTROL 添加当前日期]**&#x200B;菜单来应用与日期格式相关的函数。