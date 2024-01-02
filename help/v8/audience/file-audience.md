---
audience: end-user
title: 以文件中的收件人为目标
description: 了解如何使用外部文件中的收件人生成电子邮件受众
badge: label="Beta 版"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: b36de9228725e199497720d3fb3bc46427ca7663
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 35%

---

# 从文件加载电子邮件受众 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="文件选择"
>abstract="选择要上传的本地文件。支持的格式为 TXT 和 CSV。将您的文件格式与下方链接的示例文件保持一致。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="列定义"
>abstract="检查外部文件中列的格式。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="格式化参数"
>abstract="检查外部文件的格式参数。"


>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="预览文件"
>abstract="检查外部文件列的预览。 此屏幕最多只能显示 30 条记录。"


您可以定位存储在外部文件中的用户档案。 用户档案不会添加到数据库中，但输入文件中的所有字段都可用于 [个性化](../personalization/gs-personalization.md). 支持的文件格式有：文本 (TXT) 和逗号分隔值 (CSV)。本文介绍了在创建独立的电子邮件投放时如何加载外部用户档案。 要从工作流中的文件加载数据，请参阅 [此页面](../workflows/activities/load-file.md).

>[!CAUTION]
>
>* 此功能仅适用于 **电子邮件投放**. 它不能与短信或推送投放一起使用。
>
>* 从外部文件加载目标人群时无法使用[对照组](control-group.md)。
>
>* 用户档案不会添加到数据库中，只会加载并可用于此特定的独立电子邮件投放。

## 选择并配置您的文件 {#upload}

要直接从电子邮件界面定位本地文件中的用户档案，请执行以下步骤：

1. 打开现有的电子邮件投放，或 [创建新的电子邮件投放](../email/create-email.md).
1. 在电子邮件投放创建窗口中，从&#x200B;**受众**&#x200B;部分，单击&#x200B;**选择受众**&#x200B;按钮并选择&#x200B;**从文件选择**&#x200B;选项。

   ![](assets/select-from-file.png)

1. 选择要使用的本地文件。 格式必须与 [示例文件](#sample-file).
1. 在屏幕的中央部分预览和检查如何映射数据。
1. 从&#x200B;**地址字段**&#x200B;下拉列表中选择包含电子邮件地址的列。如果在输入的文件中有阻止列表列，则还可选择此类信息。
1. 从可用的选项调整列设置和如何格式化数据。
1. 在确认设置正确后，单击&#x200B;**确认**。

创建和个性化消息内容时，您可以从输入文件 [个性化编辑器](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## 示例文件 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="从文件加载受众"
>abstract="支持的文件格式为 TXT 和 CSV。使用第一行作为列标题。使您的文件格式与在下方链接中提供的示例文件一致。"

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

## 预览和测试电子邮件 {#test}

通过Campaign Web，您可以预览和发送使用从文件上传的受众的测试电子邮件。 为此，请执行以下步骤：

1. 单击 **[!UICONTROL “模拟内容”按钮]** 在投放内容编辑屏幕中，单击 **[!UICONTROL 添加测试配置文件]** 按钮。

1. 将显示上传的文件中包含的用户档案。 选择要用于预览内容的配置文件，然后单击 **[!UICONTROL 选择]**.

1. 投放内容的预览显示在屏幕的右侧窗格中。 个性化元素被替换为在左窗格中选择的配置文件中的数据。 [了解有关投放内容预览的更多信息](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png)

1. 要发送测试电子邮件，请单击 **[!UICONTROL 测试]** 按钮。

1. 单击 **[!UICONTROL 上传校对配置文件]** 按钮并选择包含验证收件人的.txt或.csv文件。

   >[!CAUTION]
   >
   >确保文件格式与用于上传受众的文件格式匹配。 任何格式错误都会显示警报。

1. 添加验证收件人并准备好发送验证时，单击 **[!UICONTROL 发送测试电子邮件]** 按钮并确认发送。

   ![](assets/file-upload-test.png)

1. 您可以随时使用查看测试电子邮件日志按钮监控测试电子邮件的发送。 [了解有关测试电子邮件监视的更多信息](../preview-test/test-deliveries.md#access-sent-test-deliveries-access-proofs)
