---
audience: end-user
title: 使用传输文件活动
description: 了解如何使用传输文件工作流活动
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 17%

---

# 转移文件 {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="转移文件"
>abstract="**传输文件**&#x200B;活动可以接收或发送文件、测试文件是否存在或列出服务器上的文件。使用的协议可以是服务器到服务器协议，也可以是 HTTP 协议。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="转移文件选项"
>abstract="转移文件选项"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="转移文件活动"
>abstract="转移文件活动"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="转移文件远程服务器"
>abstract="指定要连接的服务器。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="转移文件源"
>abstract="输入所需的文件名。"

**传输文件**&#x200B;活动是&#x200B;**数据管理**&#x200B;活动。 它允许您接收或发送文件、测试文件是否存在或列出服务器上的文件。 使用的协议可以是服务器到服务器协议，也可以是 HTTP 协议。

>[!NOTE]
>
>通过Campaign Web用户界面，我们通过合并&#x200B;**文件传输**&#x200B;和&#x200B;**Web下载**&#x200B;功能，将两个活动合并为一个。 此合并不会以任何方式影响该活动的功能。

按照下面详述的步骤配置&#x200B;**传输文件**&#x200B;活动。

## 选择传输协议和操作 {#protocol}

1. 将&#x200B;**传输文件**&#x200B;活动添加到您的工作流中，然后根据要使用的协议指定要执行的传输类型：

   * 对于HTTP协议，选择&#x200B;**[!UICONTROL Web下载]**。 这样，您就可以执行以GET或POST方式下载明确的URL、外部帐户或Adobe Campaign实例上的文件。
   * 对于其他服务器到服务器协议和相关操作，请选择&#x200B;**[!UICONTROL 文件传输]**。

1. 选择要对活动执行的操作。 可用操作取决于您选择的传输类型。 展开以下部分以获取更多信息。

   +++可用于&#x200B;**文件传输**&#x200B;类型活动的操作

   * **[!UICONTROL 文件下载]**：从服务器下载文件。
   * **[!UICONTROL 文件上传]**：在服务器上上传文件。
   * **[!UICONTROL 测试文件是否存在]**：检查服务器上是否存在给定的文件。 在活动后生成两个叫客过渡：“文件存在”和“文件不存在”。
   * **[!UICONTROL 文件列表]**：列出服务器上所有可用的文件。

+++

   +++可用于&#x200B;**Web下载**&#x200B;类型活动的操作

   * **[!UICONTROL 简单传输(GET)]**：检索文件。
   * **[!UICONTROL 使用表单(POST)传输]**：上传文件和其他参数。

+++

   ![](../assets/workflow-transfer-file-action.png)

1. 默认情况下，对于文件上传操作，该活动使用上一个活动中指定的文件。 若要使用其他文件，请关闭&#x200B;**[!UICONTROL 使用上一个活动的文件]**&#x200B;选项，然后单击&#x200B;**[!UICONTROL 添加文件]**&#x200B;按钮。

   在&#x200B;**[!UICONTROL Source]**&#x200B;字段中，输入所需的文件名，或使用表达式编辑器通过事件变量计算文件名。 [了解如何使用事件变量和表达式编辑器](../event-variables.md)。 重复此操作，根据需要添加任意数量的文件。

## 定义转移目标 {#destination}

1. 在&#x200B;**[!UICONTROL 远程服务器]**&#x200B;部分中，使用以下方法之一指定要连接的服务器：

   * **[!UICONTROL 使用外部帐户中定义的连接参数]**：使用外部帐户的连接参数连接到服务器。 在&#x200B;**[!UICONTROL 服务器文件夹]**&#x200B;字段中，指定文件的路径（或文件列表操作的文件夹路径）。
   * **[!UICONTROL 快速配置]**：输入文件的URL（或用于文件列表操作的文件夹）。
   * **[!UICONTROL Adobe Campaign实例]**（Web下载类型活动）：从Adobe Campaign实例服务器下载文件。

   ![](../assets/workflow-transfer-file-server.png)

1. 对于Web下载POST操作，您可以通过该操作传递其他参数。 为此，请单击&#x200B;**[!UICONTROL 添加参数]**&#x200B;按钮，然后指定参数的名称和值。 您可以根据需要添加任意数量的参数。

1. 默认情况下，对于文件上传，会自动保存服务器上上传的文件。 如果不想保留此历史记录，请关闭&#x200B;**[!UICONTROL 保留已发送文件的历史记录]**&#x200B;选项。

## 历史化设置 {#historization}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="文件历史记录"
>abstract="每次执行&#x200B;**[!UICONTROL 传输文件]**&#x200B;活动时，都会将上载或下载的文件存储在专用文件夹中。 为工作流的每个传输文件活动创建一个文件夹。 默认情况下，文件在处理之前保存在Adobe Campaign安装文件夹(`/vars`)的默认存储目录中。 若要使用特定文件夹，请关闭&#x200B;**[!UICONTROL 使用默认存储目录]**&#x200B;选项，然后输入该目录的路径。"

每次执行&#x200B;**[!UICONTROL 传输文件]**&#x200B;活动时，都会将上载或下载的文件存储在专用文件夹中。 为工作流的每个传输文件活动创建一个文件夹。 默认情况下，文件在处理之前保存在Adobe Campaign安装文件夹(`/vars`)的默认存储目录中。 若要使用特定文件夹，请关闭&#x200B;**[!UICONTROL 使用默认存储目录]**&#x200B;选项，然后输入该目录的路径。

![](../assets/workflow-transfer-file-historization.png)

必须能够限制此文件夹的大小以保留服务器上的物理空间。 为此，您可以定义活动文件夹的文件数目上限或文件总计大小上限。 默认为 100 个文件和 50 MB。

每次执行活动时，都会按如下方式检查文件夹：

* 只考虑创建时间早于执行活动 24 小时以上的文件。
* 如果考虑的文件数大于&#x200B;**[!UICONTROL 文件数]**&#x200B;字段的值，则删除最早的文件，直到达到允许的最大文件数。
* 如果考虑的文件总大小大于&#x200B;**[!UICONTROL 最大大小（以MB为单位）]**&#x200B;参数的值，则将删除最早的文件，直到达到允许的最大大小（以MB为单位）。

>[!CAUTION]
>
>如果不再执行活动，则不会检查或清除其文件夹。考虑到这一点，在传输大文件时要多加小心。

## 高级和错误管理选项 {#advanced}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="转移后删除源文件"
>abstract="转移成功后删除源文件。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="显示会话日志"
>abstract="与转移操作相关的信息显示在工作流日志中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="列出所有文件"
>abstract="此选项会对服务器上 **vars.filenames** 事件变量中的所有文件进行索引。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="处理缺失的文件"
>abstract="此选项允许您在活动结束后激活&#x200B;**无文件**&#x200B;出站过渡。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="流程错误"
>abstract="此选项允许您在活动结束后激活&#x200B;**错误**&#x200B;出站过渡。"

1. 在&#x200B;**[!UICONTROL 高级选项]**&#x200B;中，根据您配置的活动类型，提供了其他选项。 展开以下部分以获取更多信息。

   +++用于&#x200B;**[!UICONTROL 文件传输]**&#x200B;类型活动的其他选项

   * **[!UICONTROL 传输后删除源文件]**：成功传输后擦除源文件。
   * **[!UICONTROL 显示会话日志]**：激活此选项后，执行工作流后，工作流日志中会显示与传输操作相关的信息。
   * **[!UICONTROL 列出所有文件]** （文件列表操作）：此选项对`vars.filenames`事件变量中服务器上存在的所有文件进行索引，其中文件名以`n`字符分隔。 [了解如何使用事件变量](../event-variables.md)

+++

   +++用于&#x200B;**[!UICONTROL Web下载]**&#x200B;类型活动的其他选项

   * **[!UICONTROL 遵循重定向]**：文件重定向允许您使用重定向，将数据输入或输出定向到其他类型的设备。
   * **[!UICONTROL 将HTTP标头添加到文件]**：在某些情况下，您可能希望向文件添加其他HTTP标头。 最常见的是，这些标头将用于提供其他信息以进行故障排除，用于[跨源资源共享(CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS)，或用于设置特定的缓存指令。
   * **[!UICONTROL 忽略HTTP返回代码]**： HTTP返回代码（也称为HTTP状态代码）表示HTTP请求的结果。

1. 使用&#x200B;**[!UICONTROL 进程错误]**&#x200B;选项，您可以在传输期间发生任何错误时，在活动后激活“错误”出站过渡。

   此外，对于&#x200B;**文件传输**&#x200B;类型活动，如果文件在指定路径不可用，则使用&#x200B;**[!UICONTROL 处理缺少的文件]**&#x200B;选项可在活动后激活“无文件”出站过渡。
