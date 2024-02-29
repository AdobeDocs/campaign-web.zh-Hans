---
title: Campaign Web用户界面工作流的护栏和限制
description: 在Campaign Web用户界面中使用工作流时的护栏和限制
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 93%

---

# 工作流的护栏和限制 {#guardrails-limitations}

在 Campaign Web 用户界面中使用在 Campaign 客户端控制台中创建或修改的组件时，以下列出的护栏和限制适用。

请注意，虽然此页面列出了在控制台和 Web 用户界面中使用工作流时的主要注意事项，但并未涵盖两个界面之间的所有潜在不兼容性。

## 工作流活动 {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="活动不可编辑"
>abstract="如果&#x200B;**查询**&#x200B;或&#x200B;**扩充**&#x200B;活动是在控制台中使用附加数据配置的，则会在 Campaign Web 中考虑扩充数据并将其传递到出站过渡中，但无法对其进行编辑。"

Campaign Web 用户界面中尚不支持的工作流活动为只读活动，并显示为不兼容的活动。仍可执行工作流、发送消息、检查日志等。可编辑在 Campaign Web 用户界面和客户端控制台中都能找到的工作流活动。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

如果&#x200B;**查询**&#x200B;或&#x200B;**扩充**&#x200B;活动是在控制台中使用附加数据配置的，则会在 Campaign Web 中考虑扩充数据并将其传递到出站过渡中，但无法对其进行编辑。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

在控制台中，**扩充**&#x200B;活动可执行协调和扩充。如果已在客户端控制台中定义&#x200B;**扩充**&#x200B;活动中的协调设置，则该活动将在 Campaign Web 用户界面中显示为&#x200B;**协调**&#x200B;活动。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

## 工作流画布 {#wkf-canvas}

在 Campaign Web 用户界面中创建新工作流时，画布仅支持一个入口点。但是，如果在控制台中创建具有多个入口点的工作流，则可在 Campaign Web 用户界面中打开并编辑该工作流。

| 控制台 | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

每次添加或移除活动时都会刷新节点的定位。如果在控制台中创建工作流，使用 Campaign Web 用户界面修改它，然后在控制台中重新打开，则可能会发现一些细微的定位瑕疵。这种情况不影响工作流的过程和任务。

| 初始工作流 | 定位更改 |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |
