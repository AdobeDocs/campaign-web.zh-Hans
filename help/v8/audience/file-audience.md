---
audience: end-user
title: 从文件定位收件人
description: 了解如何使用外部文件中的收件人构建电子邮件受众
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 231d117247462645fe2b72f324486c4ea9122faf
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 21%

---

# 从文件加载收件人 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="文件选择"
>abstract="选择要上传的本地文件。支持的格式为TXT和CSV。 将文件格式与下面链接的样例文件对齐。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="列定义"
>abstract="检查要从本地文件插入的列的格式。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="格式化参数"
>abstract="检查文件的格式参数。"

您可以从外部文件上传联系人。 此功能仅适用于电子邮件投放。 支持的文件格式包括：文本(TXT)和逗号分隔值(CSV)。 用户档案不会添加到数据库中，但输入文件中的所有字段都可用于进行个性化。

>[!NOTE]
>
>您可以构建导入工作流，以添加或更新数据库中的多个用户档案。 了解详情


要直接从界面定位本地文件中的配置文件，请执行以下步骤：

1. 在电子邮件投放创建窗口中，从 **Audience** 部分，单击 **选择受众** 按钮并选择 **从文件选择** 选项。

   ![](assets/select-from-file.png)

1. 选择要上传的本地文件。
1. 在屏幕的中心部分中预览并检查数据映射方式。
1. 从中选择包含电子邮件地址的列 **地址字段** 下拉菜单。 阻止列表如果输入文件中包含此类信息，也可以选择列。
1. 调整列设置，以及如何使用可用选项设置数据格式。
1. 在确认设置正确后，单击&#x200B;**确认**。

在创建和个性化消息内容时，可以在个性化编辑器中从输入文件中选择字段。

![](assets/select-external-perso.png)

## 示例文件 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="示例文件"
>abstract="支持的文件格式： txt、csv。 使用第一行作为列标题。"


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
