---
audience: end-user
title: 配置工作流设置
description: 了解如何使用Adobe Campaign Web配置工作流设置
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 26%

---


# 配置工作流设置 {#workflow-settings}

在画布中编排工作流活动时，您可以访问与工作流相关的高级设置。 例如，您可以为工作流设置特定时区，管理工作流在出错时的行为方式，或管理应清除工作流历史记录的延迟。

这些设置是在创建工作流时选择的模板中预先配置的，但可以根据需要为此特定工作流进行编辑。

要执行此操作，请单击 **[!UICONTROL 设置]** 按钮时，该按钮将在工作流画布上方的操作栏中可用。

![](assets/workflow-settings-button.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

## 工作流属性 {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="工作流属性"
>abstract="此部分提供了通用工作流属性，在创建工作流时也可以访问这些属性。您可以选择要用于创建工作流的模板并指定标签。展开“其他选项”部分以配置特定设置，例如工作流存储文件夹或时区。"

此 **[!UICONTROL 属性]** 部分提供了在创建工作流时也可以访问的常规设置。

![](assets/workflow-settings.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}


这些属性包括：

* 此 **[!UICONTROL 标签]** 显示在列表中的工作流的ID。
* 此 **[!UICONTROL 内部名称]** 工作流的。
* 此 **[!UICONTROL 文件夹]** 保存工作流的位置。
* 默认 **[!UICONTROL 时区]** 以在工作流的所有活动中使用。 默认情况下，工作流的时区就是为当前Campaign操作员定义的时区。
可能的值包括：
   * **服务器时区** 使用Adobe Campaign应用程序服务器的时区
   * **操作员时区** 在客户端控制台中，使用执行工作流的Adobe Campaign操作员的时区，如操作员的配置文件中所定义
   * **数据库的时区** 使用数据库服务器的时区
   * 特定时区
* 当工作流失败时，操作员将属于在 **[!UICONTROL 主管]** 字段会通过电子邮件接收通知。
* 您也可以输入 **[!UICONTROL 描述]** 的工作流。

当工作流为 [与活动关联](create-workflow.md)，它显示在中 **[!UICONTROL 链接的活动]** 字段。 您可以从该字段打开关联的营销策划。


## 分段设置  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="分段设置"
>abstract="在此部分中，您可以选择工作流中目标配置文件的定位维度，并选择保留两次执行之间的工作流结果。此选项只应用于测试目的，且不得在生产工作流中启用。"

* **[!UICONTROL 定位维度]**：选择定向维度以定向用户档案：收件人、合同受益人、操作员、订阅者等。 [了解有关定位维度的更多信息](../audience/targeting-dimensions.md)

* **[!UICONTROL 保留两次执行之间的临时人口结果]**：默认情况下，仅保留上次执行工作流的工作表。 以前执行的工作表由每天运行的技术工作流清除。

  如果启用此选项，则即使在执行工作流后，也会保留工作表。 您可以将其用于测试目的，因此必须使用 **仅限** 在开发或暂存环境中。 绝不能在生产工作流中勾选该活动。

## 执行设置  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="执行设置"
>abstract="在此部分中，您可以配置与工作流执行相关的设置，例如工作流历史记录的保留天数。"

* **[!UICONTROL 历史记录（天）]**：指定必须清除历史记录的天数。 历史记录包含与工作流相关的元素：日志、任务、事件（链接到工作流操作的技术对象）。 现成工作流模板的默认值为30天。 历史记录的清除工作由数据库清理技术工作流执行，默认情况下每天执行一次

  >[!IMPORTANT]
  >
  >如果将&#x200B;**[!UICONTROL 历史记录（天）]**&#x200B;字段保留为空，其值将被视为“1”，这表示历史记录将在 1 天后清除。

* **[!UICONTROL 默认关联]**：如果您的安装包含多个工作流服务器，请使用此字段指定将在其中执行工作流的服务器。 这强制在特定服务器上执行该工作流。 您可以选择任何现有的关联名称，但请确保不使用空格或标点符号。 如果使用不同的服务器，请指定不同的名称（用逗号分隔）。

  >[!IMPORTANT]
  >
  >如果此字段中定义的值在任何服务器上不存在，则工作流将保持挂起状态。


* **[!UICONTROL 将SQL查询保存在日志中]**：选中此选项可将SQL查询从工作流保存到日志中。 此功能是为高级用户保留的。它适用于包含定向活动的工作流，例如 **[!UICONTROL 构建受众]**. 启用此选项后，工作流执行期间发送到数据库的SQL查询将显示在工作流的日志中，允许您分析这些查询以优化查询或诊断问题。

## 错误管理设置  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="错误管理设置"
>abstract="在本部分中，您可以定义工作流在执行期间应如何管理错误。您可以选择暂停流程、忽略一定数量的错误或停止执行工作流程。"

* **[!UICONTROL 错误管理]**：利用此字段，可定义在工作流任务出错时要执行的操作。 有三种可能的选项：

   * **[!UICONTROL 暂停进程]**：工作流自动暂停，其状态更改为 **[!UICONTROL 失败]**. 问题解决后，请使用恢复工作流 **[!UICONTROL 继续]** 按钮。
   * **[!UICONTROL 忽略]**：触发错误的任务的状态更改为 **[!UICONTROL 失败]**，但工作流会保留 **[!UICONTROL 已开始]** 状态。 <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL 中止进程]**：工作流将自动停止，其状态将更改为 **[!UICONTROL 失败]**. 问题解决后，请使用重新启动工作流 **[!UICONTROL 开始]** 按钮。

* **[!UICONTROL 连续错误]**：当满足以下条件时，此字段将变为可用 **[!UICONTROL 忽略]** 值在 **[!UICONTROL 发生错误时]** 字段。 您可以指定在流程停止前可忽略的错误的数量。一旦达到此数量，工作流状态将更改为 **[!UICONTROL 失败]**. 如果此字段的值为 0，则无论错误数量是多少，工作流都绝不会停止。
