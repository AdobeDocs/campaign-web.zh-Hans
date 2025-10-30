---
audience: end-user
title: 关于只读工作流
description: 了解工作流处于只读模式的原因
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 11%

---

# 关于只读工作流 {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="此工作流为只读"
>abstract="由于您的权限或工作流类型，您无法编辑此工作流。"

某些工作流是只读的。 内置的技术工作流始终是只读的，但此限制也适用于其他类型的工作流。

Campaign用户对Adobe Campaign数据的访问权限可能受限。 Campaign管理员可以授予他们查看特定功能的权限，但不能编辑或修改这些功能。 用户对数据的权限对于确保数据和流程的安全性至关重要。 在[本节](../get-started/permissions.md)中了解有关Campaign中权限管理的更多信息。

当工作流处于只读模式时：

* 提及&#x200B;**[!UICONTROL 只读]**&#x200B;出现在&#x200B;**[!UICONTROL 设置]**&#x200B;按钮附近。
* 无法访问操作按钮。

![只读工作流界面显示“设置”按钮和禁用的操作按钮。](assets/readonly-workflow.png){zoomable="yes"}

用户无法在只读工作流中编辑任何内容。 不允许他们更改活动的设置。

![处于只读模式的计划程序接口，显示已禁用的设置选项。](assets/scheduler-readonly.png){zoomable="yes"}

用户无法删除工作流。

![界面显示删除工作流的受限权限。](assets/readonly-rights.png){zoomable="yes"}

## 只读工作流的类型 {#readonly-workflow-types}

根据工作流的类型，只读模式可能会有所不同。

### 活动工作流 {#readonly-campaign-wf}

在只读营销活动工作流中，用户无法访问监视按钮。

![只读模式下的Campaign工作流界面，显示已禁用的监视选项。](assets/readonly-campaign-workflow.png){zoomable="yes"}

### 技术工作流 {#readonly-tech-wf}

对于所有Campaign用户（包括管理员），内置技术工作流均为只读。 但是，如果需要，用户可以&#x200B;**暂停**&#x200B;或&#x200B;**停止**。 仅允许执行上述操作。

![只读模式的技术工作流界面，显示暂停或停止工作流的选项。](assets/readonly-technical-workflow.png){zoomable="yes"}

在[本节](https://experienceleague.adobe.com/zh-hans/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)中了解有关技术工作流的更多信息。