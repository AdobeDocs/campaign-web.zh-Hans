---
audience: end-user
title: 从文件导入收件人
description: 了解如何从外部文件导入收件人
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f103fe804deccc83638a3e56a03f6e715e68e550
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 10%

---

# 从文件导入收件人 {#audience-from-file}

您可以通过上传文本文件(TXT)或逗号分隔值文件(CSV)，从投放界面添加或更新联系人。 然后系统会将它们添加到数据库中。

>[!NOTE]
>
>您还可以构建导入工作流以添加或更新多个用户档案。


要直接从界面从本地文件添加用户档案，请执行以下步骤：

1. 在投放创建窗口中，单击 **选择受众** 按钮并选择 **从文件中选择** 选项。
1. 选择要上传的本地文件。
1. 定义列设置以及如何设置数据格式。 您可以使用 **忽略列** 切换。
1. 在屏幕的中央部分预览数据的映射方式。
1. 单击 **确认** 设置正确后。

创建和个性化消息内容时，您可以从个性化编辑器的输入文件中选择字段。

## 示例文件 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="示例文件"
>abstract="支持的文件格式：txt、csv、xls。 使用第一行作为列标题."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
