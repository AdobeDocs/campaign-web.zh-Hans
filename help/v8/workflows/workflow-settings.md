---
audience: end-user
title: 配置工作流设置
description: 了解如何使用Adobe Campaign Web配置工作流设置
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: d4eef621d2287881bfa7ef57e5d90026adceb49c
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 29%

---


# 配置工作流设置 {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="工作流属性"
>abstract="在此屏幕中，选择要用于创建工作流的模板并指定标签。展开&#x200B;**其他选项**&#x200B;部分以配置更多设置，例如工作流内部名称、其文件夹、时区和主管组。强烈建议选择一个主管组，以便如果出错，可提醒操作员。"

在画布中创建工作流或编排工作流活动时，您可以访问与工作流相关的高级设置。 例如，您可以为工作流设置特定时区，管理工作流在出错时的行为方式，或管理应清除工作流历史记录的延迟。

这些设置是在创建工作流时选择的模板中预先配置的，但可以根据需要为此特定工作流进行编辑。

![](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## 工作流属性 {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="工作流属性"
>abstract="此部分提供了通用工作流属性，在创建工作流时也可以访问这些属性。您可以选择要用于创建工作流的模板并指定标签。展开“其他选项”部分以配置特定设置，例如工作流存储文件夹或时区。"

**[!UICONTROL 属性]**&#x200B;部分提供了可在创建工作流时配置的常规设置。 要访问现有工作流的属性，请单击工作流画布上方操作栏中可用的&#x200B;**[!UICONTROL 设置]**&#x200B;按钮。


![](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}


这些属性包括：

* 列表中显示的工作流的&#x200B;**[!UICONTROL 标签]**。
* 工作流的&#x200B;**[!UICONTROL 内部名称]**。
* 应保存工作流的&#x200B;**[!UICONTROL 文件夹]**。
* 在工作流的所有活动中使用的默认&#x200B;**[!UICONTROL 时区]**。 默认情况下，工作流的时区就是为当前Campaign操作员定义的时区。
可能的值包括：
   * **服务器时区**&#x200B;以使用Adobe Campaign应用程序服务器的时区
   * **操作员时区**，使用在客户端控制台中执行工作流的Adobe Campaign操作员的时区，如操作员的配置文件中所定义
   * **数据库的时区**&#x200B;以使用数据库服务器的时区
   * 特定时区
* 当工作流失败时，会通过电子邮件通知属于在&#x200B;**[!UICONTROL 主管]**&#x200B;字段中选择的操作员组的操作员。
* 您还可以输入工作流的&#x200B;**[!UICONTROL 描述]**。

当工作流为[与营销活动](create-workflow.md)关联时，它显示在&#x200B;**[!UICONTROL 链接营销活动]**&#x200B;字段中。 您可以从该字段打开关联的营销策划。


## 分段设置  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="分段设置"
>abstract="在此部分中，您可以选择工作流中目标配置文件的目标选择维度，并选择保留两次执行之间的工作流结果。此选项只应用于测试目的，且不得在生产工作流中启用。"

* **[!UICONTROL 定向维度]**：选择要用于定向用户档案的定向维度：收件人、合同受益人、操作员、订阅者等。 [了解有关定向维度的更多信息](../audience/targeting-dimensions.md)

* **[!UICONTROL 保留两次执行之间的临时人口结果]**：默认情况下，仅保留工作流上次执行的工作表。 以前执行的工作表由每天运行的技术工作流清除。

  如果启用此选项，则即使在执行工作流后，也会保留工作表。 您可以将其用于测试目的，因此必须&#x200B;**仅**&#x200B;用于开发或暂存环境。 绝不能在生产工作流中勾选该活动。

## 执行设置  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="执行设置"
>abstract="在此部分中，您可以配置与工作流执行相关的设置，例如工作流历史记录的保留天数。"

* **[!UICONTROL 历史记录（以天为单位）]**：指定必须清除历史记录的天数。 历史记录包含与工作流相关的元素：日志、任务、事件（链接到工作流操作的技术对象）。 现成工作流模板的默认值为30天。 历史记录的清除工作由数据库清理技术工作流执行，默认情况下每天执行一次

  >[!IMPORTANT]
  >
  >如果将&#x200B;**[!UICONTROL 历史记录（天）]**&#x200B;字段保留为空，其值将被视为“1”，这表示历史记录将在 1 天后清除。

* **[!UICONTROL 默认关联性]**：如果您的安装包含多个工作流服务器，请使用此字段指定将在其中执行工作流的服务器。 这强制在特定服务器上执行该工作流。 您可以选择任何现有的关联名称，但请确保不使用空格或标点符号。 如果使用不同的服务器，请指定不同的名称（用逗号分隔）。

  >[!IMPORTANT]
  >
  >如果此字段中定义的值在任何服务器上不存在，则工作流将保持挂起状态。


* **[!UICONTROL 将SQL查询保存到日志]**：选中此选项可将SQL查询从工作流保存到日志中。 此功能是为高级用户保留的。它适用于包含定向活动（如&#x200B;**[!UICONTROL 生成受众]**）的工作流。 启用此选项后，工作流执行期间发送到数据库的SQL查询将显示在工作流的日志中，允许您分析这些查询以优化查询或诊断问题。

## 错误管理设置  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="错误管理设置"
>abstract="在本部分中，您可以定义工作流在执行期间应如何管理错误。您可以选择暂停流程、忽略一定数量的错误或停止执行工作流程。"

* **[!UICONTROL 错误管理]**：此字段允许您定义工作流任务出现错误时要执行的操作。 有三种可能的选项：

   * **[!UICONTROL 挂起进程]**：工作流已自动暂停，其状态更改为&#x200B;**[!UICONTROL 失败]**。 问题解决后，使用&#x200B;**[!UICONTROL 恢复]**&#x200B;按钮恢复工作流。
   * **[!UICONTROL 忽略]**：触发错误的任务状态更改为&#x200B;**[!UICONTROL 失败]**，但工作流会保留&#x200B;**[!UICONTROL 已启动]**&#x200B;状态。<!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL 中止进程]**：工作流已自动停止，其状态更改为&#x200B;**[!UICONTROL 失败]**。 问题解决后，使用&#x200B;**[!UICONTROL 启动]**&#x200B;按钮重新启动工作流。

* **[!UICONTROL 连续错误]**：在&#x200B;**[!UICONTROL 如果出现错误]**&#x200B;字段中选择&#x200B;**[!UICONTROL 忽略]**&#x200B;值时，此字段将变为可用。 您可以指定在流程停止前可忽略的错误的数量。一旦达到此数量，工作流状态将更改为&#x200B;**[!UICONTROL 失败]**。 如果此字段的值为 0，则无论错误数量是多少，工作流都绝不会停止。

## 初始化脚本 {#initialization-script}

**初始化脚本**&#x200B;允许您初始化变量或修改活动属性。 单击&#x200B;**编辑代码**&#x200B;按钮并键入要执行的代码片段。 工作流执行时将调用脚本。 请参阅与[事件变量](../workflows/event-variables.md)相关的部分。

