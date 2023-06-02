---
audience: end-user
title: 使用 Adobe Campaign Web 创建工作流
description: 了解如何使用 Adobe Campaign Web 构建工作流
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 7e694f46239f782131524eed6b34bff4c4d98dca
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 20%

---

# 配置工作流设置 {#workflow-settings}

在画布中编排工作流活动时，您可以访问与工作流相关的高级设置。 例如，您可以为工作流设置特定的时区，管理工作流在出错时的行为方式，或者管理应清除工作流历史记录之前的延迟。

这些设置是在创建工作流时选择的模板中预先配置的，但可以根据此特定工作流的需要进行编辑。

要执行此操作，请单击 **[!UICONTROL 工作流设置]** 图标的工作流标签旁边。

![](assets/workflow-settings.png)

## 工作流属性 {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="工作流属性"
>abstract="本节提供了创建工作流时也可以访问的通用工作流属性。 您可以选择用于创建工作流的模板并指定标签。 展开其他选项部分以配置特定设置，例如存储文件夹或时区的工作流。"

此 **[!UICONTROL 属性]** 部分提供了在创建工作流时也可以访问的常规设置。

* **[!UICONTROL 标签]**：列表中显示的工作流的标签。
* **[!UICONTROL 名称]**：工作流的内部名称。
* **[!UICONTROL 文件夹]**：保存工作流的文件夹。
* **[!UICONTROL 链接的活动]**：如果已在营销策划中创建工作流，则会显示此字段。 它允许您打开关联的营销策划。
* **[!UICONTROL 时区]**：定义默认用于工作流所有活动的特定时区。 默认情况下，工作流的时区就是为当前 Campaign 操作人员定义的时区。
* **[!UICONTROL 主管]**：当工作流出错时，只要属于工作流监督组的操作员的电子邮件地址列在其用户档案中，该操作员就会收到电子邮件通知。
* **[!UICONTROL 描述]**：使用此字段提供工作流的描述。

## 分段设置

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="分段设置"
>abstract="在此部分中，您可以选择定向维度以在工作流中定向用户档案，然后选择在两个执行之间保留工作流结果。 此选项应仅用于测试目的，不得在生产工作流中启用。"

* **[!UICONTROL 定位维度]**：选择定向维度以用于定向用户档案：收件人、合同受益人、操作员、订阅者等。
* **[!UICONTROL 保留两次执行之间的临时人口结果]**：默认情况下，仅保留上次执行工作流的工作表。 技术工作流会清除以前执行的工作表，每天运行该工作流。

   如果启用此选项，则即使在执行工作流后，也会保留工作表。 您可以将其用于测试目的，因此必须仅将其用于开发或暂存环境。 绝不能在生产工作流中勾选该活动。

## 执行设置

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="执行设置"
>abstract="在此部分中，您可以配置与工作流执行相关的设置，如工作流历史记录保留的天数。"

* **[!UICONTROL 历史记录（天）]**：指定必须清除历史记录的天数。 历史记录包含与工作流相关的元素：日志、任务、事件（链接到工作流操作的技术对象）。 现成的工作流模板的默认值为 30 天。历史记录的清除工作由数据库清理技术工作流执行，默认情况下每天执行一次

   >[!IMPORTANT]
   >
   >如果将&#x200B;**[!UICONTROL 历史记录（天）]**&#x200B;字段保留为空，其值将被视为“1”，这表示历史记录将在 1 天后清除。

* **[!UICONTROL 默认关联]**：如果您的安装包含多个工作流服务器，请使用此字段选择将在其中执行工作流的计算机。 如果此字段中定义的值不存在于任何服务器上，则工作流将保持挂起状态。

* **[!UICONTROL 将SQL查询保存到日志中]**：用于将SQL查询从工作流保存到日志中。 此功能是为高级用户保留的。它适用于包含定向活动的工作流，例如 **[!UICONTROL 构建受众]**. 启用此选项后，工作流执行期间发送到数据库的SQL查询将显示在Adobe Campaign中，允许您分析这些查询以优化查询或诊断问题。

   查询将显示在 **[!UICONTROL SQL 日志]**&#x200B;选项卡中，该选项卡将添加到工作流（营销活动工作流除外）和&#x200B;**[!UICONTROL 属性]**&#x200B;活动中（启用该选项时）。<!-- where?-->

## 错误管理设置

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="错误管理设置"
>abstract="在此部分中，您可以管理工作流在执行期间发生错误（暂停/停止执行或忽略错误）时的行为方式。"

* **[!UICONTROL 错误管理]**：利用此字段，可定义在工作流任务出错时要执行的操作。 提供了两个可能的选项：

   * **[!UICONTROL 暂停进程]**：工作流自动暂停，其状态更改为 **[!UICONTROL 失败]**. 问题解决后，请使用恢复工作流 **[!UICONTROL 恢复]** 按钮。
   * **[!UICONTROL 忽略]**：触发错误的任务的状态更改为 **[!UICONTROL 失败]**，但工作流会保留 **[!UICONTROL 已开始]** 状态。 <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL 中止进程]**：工作流将自动停止，其状态将更改为 **[!UICONTROL 失败]**. 问题解决后，请使用重新启动工作流 **[!UICONTROL 开始]** 按钮。

* **[!UICONTROL 连续错误]**：此字段在以下情况下变为可用： **[!UICONTROL 忽略]** 值在 **[!UICONTROL 发生错误时]** 字段。 您可以指定在流程停止前可忽略的错误的数量。一旦达到此数量，工作流状态将更改为 **[!UICONTROL 失败]**. 如果此字段的值为 0，则无论错误数量是多少，工作流都绝不会停止。
