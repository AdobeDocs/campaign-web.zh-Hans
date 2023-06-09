---
audience: end-user
title: 以文件中的收件人为目标
description: 了解如何使用外部文件中的收件人生成电子邮件受众
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f60f0e34dc5d85808c208223d83d234e22a41c34
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 64%

---

# 从文件加载电子邮件受众 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="文件选择"
>abstract="选择要上传的本地文件。支持的格式为 TXT 和 CSV。将您的文件格式与下方链接的示例文件保持一致。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="列定义"
>abstract="检查要从本地文件插入的列的格式。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="格式化参数"
>abstract="检查文件的格式化参数。"

您可以从外部文件上传联系人。用户档案不会添加到数据库中，但输入文件中的所有字段都可用于 [个性化](../personalization/gs-personalization.md). 支持的文件格式有：文本 (TXT) 和逗号分隔值 (CSV)。

>[!CAUTION]
>
>* 此功能仅适用于 **独立电子邮件投放**. 它不能用在工作流中，也不能用于短信或推送投放。
>
>* 从外部文件加载目标人群时无法使用[对照组](control-group.md)。


要直接从电子邮件界面定位本地文件中的用户档案，请执行以下步骤：

1. 打开现有的电子邮件投放，或 [创建新的电子邮件投放](../email/create-email.md).
1. 在电子邮件投放创建窗口中，从&#x200B;**受众**&#x200B;部分，单击&#x200B;**选择受众**&#x200B;按钮并选择&#x200B;**从文件选择**&#x200B;选项。

   ![](assets/select-from-file.png)

1. 选择要上传的本地文件。格式必须与 [示例文件](#sample-file).
1. 在屏幕的中央部分预览和检查如何映射数据。
1. 从&#x200B;**地址字段**&#x200B;下拉列表中选择包含电子邮件地址的列。如果在输入的文件中有阻止列表列，则还可选择此类信息。
1. 从可用的选项调整列设置和如何格式化数据。
1. 在确认设置正确后，单击&#x200B;**确认**。

创建和个性化消息内容时，您可以从的输入文件中选择字段 [个性化编辑器](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## 示例文件 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="示例文件"
>abstract="支持的文件格式：txt、csv。使用第一行作为列标题。"

支持的格式为 TXT 和 CSV。第一行是列标题。

将文件格式与下面的示例文件对齐：

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
