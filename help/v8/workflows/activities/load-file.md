---
audience: end-user
title: 使用加载文件工作流活动
description: 了解如何使用加载文件工作流活动
badge: label="有限发布版"
source-git-commit: 6068e3695ebed22a94a75b9aded59d1e5fb6b47a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 34%

---

# 加载文件 {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="加载文件活动"
>abstract="此 **加载文件** 活动是 **数据管理** 活动。 使用此活动可使用存储在外部文件中的用户档案。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="示例文件"
>abstract="示例文件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="文件名称"
>abstract="文件名称"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="目标数据库"
>abstract="目标数据库"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="加载文件活动的拒绝管理"
>abstract="加载文件活动的拒绝管理"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="拒绝管理出站过渡"
>abstract="拒绝管理出站过渡"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="针对拒绝的拒绝管理出站过渡"
>abstract="针对拒绝的拒绝管理出站过渡"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="加载文件活动的格式设置"
>abstract="加载文件活动的格式设置"


此 **加载文件** 活动是 **数据管理** 活动。 使用此活动可使用存储在外部文件中的用户档案。 用户档案不会添加到数据库中，但输入文件中的所有字段都可用于 [个性化](../../personalization/gs-personalization.md)，或者更新用户档案。


>[!NOTE]
>支持的文件格式为：文本(TXT)和逗号分隔值(CSV)。


此活动可与 [调解](reconciliation.md) 活动，用于将未识别的数据链接到现有资源。 例如， **加载文件** 活动可放在之前 **调解** 活动。


## 配置加载文件活动 {#load-configuration}

按照以下步骤配置 **加载文件** 活动：


1. 拖放 **加载文件** 活动添加到工作流中。 单击 **从文件选择** 按钮。
1. 选择要使用的本地文件。 格式必须与 [示例文件](../../audience/file-audience.md#sample-file).
1. 在屏幕的中央部分预览和检查如何映射数据。
1. 从可用的选项调整列设置和如何格式化数据。
1. 在确认设置正确后，单击&#x200B;**确认**。

## 示例{#load-example}

外部文件加载的示例可在 **调解** 中的活动 [本节](reconciliation.md#example).