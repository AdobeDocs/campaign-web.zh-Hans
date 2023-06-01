---
title: 创建条件内容
description: 了解如何在Adobe Campaign Web UI中定义条件以个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 5598a82bf745659b8c1db8cb51b1a82cfd184093
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# 生成条件内容{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="创建条件内容"
>abstract="创建条件内容以根据收件人的配置文件定义动态个性化，在满足某些条件时自动替换文本块和图像。 此功能可将您的营销活动提升到新的高度，并为受众提供极具针对性的个性化体验。"


条件内容是一项强大的功能，允许您根据收件人的配置文件创建动态个性化，在满足某些条件时自动替换文本块和图像。 此功能可将您的营销活动提升到新的高度，并为受众提供极具针对性的个性化体验。

通过配置条件内容字段，您可以根据收件人的用户档案创建高级动态个性化。 当满足特定条件时，替换消息内容中的文本块、链接、主题行和/或图像。 例如，您可以根据Adobe Campaign数据库中“性别”字段的值显示“先生”或“夫人”，也可以根据收件人的首选语言包含其他链接。

## 个性化语法{#perso-syntax}



## 使用个性化编辑器中的条件{#condition-perso-editor}

要为投放定义条件内容，请执行以下操作：

1. 打开投放并编辑内容。
1. 单击 **[!UICONTROL 打开个性化对话框]** 图标（例如，用于短信）。

   ![](assets/open-perso-editor-sms.png)

1. 在个性化编辑器中，浏览 **[!UICONTROL 辅助函数]**.
1. 单击“+”图标 **如果** 函数。 以下行将添加到中央屏幕中：
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Replace `<FIELD>` 按个性化字段。 例如，收件人的公司： `recipient.company`.
1. Replace `<VALUE>` 替换为要满足的值。 例如，`ADOBE`。




## 示例：条件短信主题行{#condition-subject-line}

要为短信消息创建条件主题行，请执行以下步骤：

1. 打开投放并编辑内容。
1. 单击主题行右侧的打开个性化对话框图标。
1. 在个性化编辑器中，浏览


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
