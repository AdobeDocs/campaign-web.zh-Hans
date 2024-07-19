---
audience: end-user
title: 关于只读工作流
description: 了解工作流处于只读模式的原因
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 13%

---

# 关于只读工作流 {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="此工作流为只读"
>abstract="由于您的权限或工作流类型，您无法编辑此工作流。"

某些工作流可能处于只读模式。 您可以通过查看它：

- **[!UICONTROL 设置]**&#x200B;按钮附近的提及&#x200B;**[!UICONTROL **&#x200B;只读&#x200B;**]**
- 操作按钮不可访问

![](assets/readonly-workflow.png){zoomable="yes"}

您不能在只读工作流中编辑任何内容。 不允许更改活动的设置。


![](assets/scheduler-readonly.png){zoomable="yes"}


您也无权删除工作流。

![](assets/readonly-rights.png){zoomable="yes"}

## 为何选择只读工作流

只读模式适用于没有权限和访问权限的用户编辑这些工作流。 [在此处了解详情](../get-started/permissions.md)

Campaign用户可以在Adobe Campaign中访问的数据可能受到限制。 管理员可以让他查看某些功能，但无法对其进行处理。

## 只读工作流的类型

根据工作流的类型，只读模式可能不同。

### 活动工作流

在只读营销活动工作流的情况下，用户无法访问监视按钮。

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### 技术工作流

对于营销活动用户，技术工作流处于只读模式。
对于所有用户（甚至管理员用户），内置的技术工作流都处于只读模式。 但如果需要，用户可以**暂停**&#x200B;或&#x200B;**停止**。 仅允许这些操作。 [在此处了解详情](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}
