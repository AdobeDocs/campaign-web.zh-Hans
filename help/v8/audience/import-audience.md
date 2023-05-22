---
audience: end-user
title: 从文件导入收件人
description: 了解如何从外部文件导入收件人
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 97%

---

# 从文件导入收件人 {#audience-from-file}

您可以通过上传文本文件 (TXT) 或逗号分隔值文件 (CSV) 从投放界面添加或更新联系人。然后系统会将它们添加到数据库中。

>[!NOTE]
>
>您还可以构建导入工作流来添加或更新多项配置文件。


要直接从界面添加本地文件中的配置文件，请执行以下步骤：

1. 在投放创建窗口中，单击&#x200B;**选择受众**&#x200B;按钮，并选择&#x200B;**从文件选择**&#x200B;选项。
1. 选择要上传的本地文件。
1. 定义列设置以及设置数据格式的方式。您可以使用&#x200B;**“忽略”列**&#x200B;开关来跳过列。
1. 预览数据在屏幕的中央部分中映射的方式。
1. 在确认设置正确后，单击&#x200B;**确认**。

在创建和个性化消息内容时，可以在个性化编辑器中从输入文件中选择字段。

## 示例文件 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="示例文件"
>abstract="支援的檔案格式： txt、csv。 使用第一行作为列标题。"


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
