---
audience: end-user
title: 使用JavaScript代码工作流活动
description: 了解如何使用JavaScript代码工作流活动
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: 040a7f68f072d5c3a7ce56a61d3383f0baccf8a8
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 30%

---

# JavaScript 代码 {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript 代码"
>abstract="**JavaScript 代码**&#x200B;活动允许您在工作流上下文中执行 JavaScript 脚本。您可以使用它来执行操作或从数据库收集信息。使用&#x200B;**简单的** JavaScript 代码活动在执行工作流时执行一个代码片段。**高级** Javascript 代码活动允许您通过按顺序执行两个不同的代码片段来执行更复杂的操作。工作流第一次启动时，会执行第一个调用。工作流每次再次运行时，都会执行第二次调用中定义的代码。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript 代码片段"
>abstract="定义运行活动时要执行的脚本。如果您正在配置&#x200B;**高级** JavaScript 活动，则需要编辑两个代码片段：在第一次执行工作流时执行的第一个调用代码，以及在下一次调用工作流时执行的下一个调用代码。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript 执行"
>abstract="配置延迟执行，以便在执行一段时间后停止活动。默认情况下，执行阶段不能超过 1 小时。延迟之后，该进程将会中止并会显示错误消息，并且活动执行会失败。若要忽略此限制，请将该值设置为 0。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript 过渡"
>abstract="切换&#x200B;**[!UICONTROL 流程错误]**&#x200B;选项，将执行脚本期间发生的错误保留在额外的输出过渡中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_processerrors"
>title="流程错误"
>abstract="流程错误"

**JavaScript代码**&#x200B;活动是&#x200B;**数据管理**&#x200B;活动。 使用此活动可在工作流的上下文中执行JavaScript脚本。 这允许您从数据库收集信息或执行其他复杂操作。

## 配置JavaScript代码活动 {#javascript-code-configuration}

按照以下步骤配置&#x200B;**JavaScript代码**&#x200B;活动：

1. 将&#x200B;**JavaScript代码**&#x200B;活动添加到您的工作流中。

1. 选择要创建的活动类型：

   * **Simple**：执行一个代码段。
   * **高级**：此选项允许您通过执行两个不同的代码片段来执行更高级的操作。 [了解如何配置高级JavaScript活动](#advanced)

   >[!NOTE]
   >
   >通过Campaign Web用户界面，我们通过合并&#x200B;**简单**&#x200B;和&#x200B;**高级** JavaScript代码功能，将两个活动合并为一个。 此合并不会以任何方式影响该活动的功能。

1. 确认，然后单击&#x200B;**[!UICONTROL 编辑代码]**&#x200B;按钮以打开表达式编辑器。 左侧窗格提供了预定义的语法，您可以利用它来构建代码，包括事件变量。 [了解如何使用事件变量和表达式编辑器](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. 在&#x200B;**[!UICONTROL 执行]**&#x200B;部分中，将延迟配置为在执行一段时间后停止活动。 默认情况下，执行阶段不能超过 1 小时。延迟之后，该进程将会中止并会显示错误消息，并且活动执行会失败。若要忽略此限制，请将该值设置为 0。

   ![](../assets/javascript-config.png)

1. 切换&#x200B;**[!UICONTROL 流程错误]**&#x200B;选项，将执行脚本期间发生的错误保留在额外的输出过渡中。

## 高级JavaScript代码活动 {#advanced}

利用高级JavaScript活动，可执行复杂的操作。 它允许您：

* 执行两个不同的代码段。 在第一次启动工作流时执行第一个代码片段。 每次再次运行工作流时，都会执行第二次调用中定义的代码片段。
* 添加多个可使用脚本动态交互的输出过渡。

要配置高级JavaScript代码活动，请执行以下步骤：

1. 选择&#x200B;**高级**&#x200B;类型，然后配置要执行的代码段：

   * 单击&#x200B;**[!UICONTROL 编辑首次调用代码]**&#x200B;以定义要在首次调用期间执行的脚本。
   * 单击&#x200B;**[!UICONTROL 编辑下一个调用代码]**&#x200B;以定义要在工作流下次调用期间执行的脚本。 （可选）

1. 要添加一个或多个输出过渡，请单击&#x200B;**[!UICONTROL 添加过渡]**&#x200B;按钮，并为每个过渡指定标签和内部名称。

   在此示例中，我们配置了两个由脚本根据特定条件在代码片段中激活的过渡。

   ![](../assets/javascript-transitions.png)

1. 完成活动的配置并启动工作流。

## 示例 {#javascript-code-example}

### 根据传入群体初始化变量 {#example1}

此示例说明如何根据工作流定向的用户档案数初始化变量。

![](../assets/javascript-example1.png)

在本例中，我们定位的是数据库中的VIP用户档案。 我们希望创建一个名为“channel”的变量，该变量的值取决于构建受众活动定向的用户档案数：

* 如果目标用户档案超过1000个，则使用值“email”初始化变量。
* 否则，使用值“sms”初始化它。

为此，请执行以下步骤：

1. 在&#x200B;**生成受众**&#x200B;活动之后添加类型为&#x200B;**Simple**&#x200B;的&#x200B;**JavaScript代码**&#x200B;活动。

1. 单击&#x200B;**编辑代码**&#x200B;并配置代码段，如下所示：

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. 启动工作流。 根据&#x200B;**构建受众**&#x200B;活动定向的用户档案数，将使用“email”或“sms”值创建“channel”变量。

### 根据变量的值触发过渡 {#example2}

此示例说明如何根据变量的值触发过渡。

![](../assets/javascript-example2-transitions.png)

在此处，工作流以&#x200B;**外部信号**&#x200B;活动开始，变量(`interest`)从另一个工作流传递到此活动中。 变量的值为“正在运行”或“瑜伽”，具体取决于在初始工作流中执行的筛选操作。

我们希望根据变量的值，在工作流中触发不同的过渡。

为此，请执行以下步骤：

1. 在类型为&#x200B;**高级**&#x200B;的外部信号活动之后添加&#x200B;**JavaScript代码**&#x200B;活动。

1. 添加两个过渡：每个可能的变量值（“正在运行”、“瑜伽”）各一个。

1. 单击&#x200B;**编辑第一个调用代码**&#x200B;并配置代码段，如下所示：

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. 根据需要完成每个过渡的配置，然后启动工作流。 已根据通过&#x200B;**外部信号**&#x200B;活动传递的`interest`变量的值激活两个输出转换之一。
