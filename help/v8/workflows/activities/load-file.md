---
audience: end-user
title: 使用加载文件工作流活动
description: 了解如何使用加载文件工作流活动
badge: label="有限发布版"
source-git-commit: ae925f16aa39b2e1de9b9957c380d17d299ad114
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 35%

---

# 加载文件 {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="加载文件活动"
>abstract=" **加载文件**&#x200B;活动是一项&#x200B;**数据管理**&#x200B;活动。使用此活动可以处理存储在外部文件中的数据。"

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

 **加载文件**&#x200B;活动是一项&#x200B;**数据管理**&#x200B;活动。使用此活动可使用存储在外部文件中的用户档案和数据。 用户档案和数据不会添加到数据库中，但输入文件中的所有字段都可用于 [个性化](../../personalization/gs-personalization.md)，或者更新用户档案或任何其他表。

>[!NOTE]
>支持的文件格式为：文本(TXT)和逗号分隔值(CSV)。

此活动可与 [调解](reconciliation.md) 活动，用于将未识别的数据链接到现有资源。 例如， **加载文件** 活动可放在之前 **调解** 活动。

## 配置加载文件活动 {#load-configuration}

按照以下步骤配置 **加载文件** 活动：

1. 拖放 **加载文件** 活动添加到工作流中。 单击 **从文件选择** 按钮。

1. 选择要使用的本地文件。 格式必须与此对齐 [示例文件](../../audience/file-audience.md#sample-file).

1. 在屏幕的中央部分预览和检查如何映射数据。

   ![](../assets/load-file.png)

1. 使用 **列** 部分来调整每列的数据类型和宽度。

1. 在 **格式化** 在列配置下的部分，指定外部文件的格式以确保正确导入数据。

1. 在确认设置正确后，单击&#x200B;**确认**。

## 示例{#load-example}

外部文件加载示例，用于 **调解** 活动的可用位置 [本节](reconciliation.md#example).