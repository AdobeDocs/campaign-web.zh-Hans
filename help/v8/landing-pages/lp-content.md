---
title: 定义特定于登陆页面的内容
description: 了解如何在Campaign Web中设计登陆页面特定内容
badge: label="有限发布版"
source-git-commit: 2a02015d9d7a7de67f0bcffd328d37080c0f50c4
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 13%

---

# 定义特定于登陆页面的内容 {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="使用内容组件"
>abstract="内容组件是空的内容占位符，您可用它来创建登陆页面的版面。要定义特定内容使得用户能够进行选择并提交其选择内容，请使用表单组件。"

编辑登陆页面中任何页面的内容时，该内容均已预填充。

主页面是在用户单击指向登陆页面的链接后立即向用户显示的页面，例如通过电子邮件或网站。 主页面已预填充了 [特定于登陆页面的表单组件](#use-form-component) 使用户能够选择并提交他们的选择。 您还可以定义 [登陆页面特定的样式](#lp-form-styles).

要进一步设计登陆页面内容，您可以使用与电子邮件相同的组件。 [了解详情](../email/content-components.md#add-content-components)

<!--
The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

Set the subscription form to the appropriate fields from the database to make sure it will work correctly.

The landing page default fields are already there for the selected template.

>[!NOTE]
>
>You can also create a click-through landing page without a **[!UICONTROL Form]** component. In that case, the landing page will be displayed to users, but they will not be required to submit any form. This can be useful if you only want to showcase a landing page without requiring any action from your recipients such as opt-in or opt out, or want to provide information that doesn't require user input.

Using the landing page content designer, you can also leverage contextual data coming from the primary page in a subpage. [Learn more](#use-primary-page-context)-->

## 使用表单组件 {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="设置表单组件字段"
>abstract="定义您的收件人如何从登陆页面查看和提交他们的选择。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="单击按钮时会出现的情况"
>abstract="定义在用户提交登陆页面表单时将会出现的情况。"

要定义特定内容，以允许用户从登陆页面选择并提交所做的选择，请使用 **[!UICONTROL 表单]** 组件。 为此，请执行以下步骤。

1. 登陆页面特定 **[!UICONTROL 表单]** 组件已显示在所选模板的画布中。

   >[!NOTE]
   >
   >此 **[!UICONTROL 表单]** 组件只能在同一页面上使用一次。

1. 选择它。 此 **[!UICONTROL 表单内容]** 选项卡显示在右侧面板中，允许您编辑表单的不同字段。

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >切换到 **[!UICONTROL 样式]** 选项卡，随时编辑表单组件内容的样式。 [了解详情](#lp-form-styles)

1. 展开第一个文本字段。 从 **[!UICONTROL 文本字段1]** 部分，您可以编辑字段类型、数据库中的字段、标签以及在用户填写字段之前显示在字段内的文本。

   ![](assets/lp-form-text-field.png)

1. 查看 **[!UICONTROL 将表单字段设为必填]** 选项（如果需要）。 在这种情况下，仅当用户填写此字段后才能提交登陆页面。

   >[!NOTE]
   >
   >如果未填写必填字段，则用户提交页面时会显示错误消息。

1. 添加复选框。 选择该复选框应更新数据库中的服务或字段。

   ![](assets/lp-form-checkbox.png)

   定义此复选框是使用户选择加入还是退出。 从以下两个选项中进行选择：

   * **[!UICONTROL 如果选中，则订阅]**：用户需要选中复选框才能同意（选择加入）。
   * **[!UICONTROL 如果选中，则取消订阅]**：用户需要选中复选框以取消同意（选择退出）。

1. 您可以根据需要删除和添加任意数量的文本字段和/或复选框。

1. 添加所有所需的复选框和/或文本字段后，单击 **[!UICONTROL 行动号召]** 以展开相应的部分。 它允许您在中定义按钮的行为 **[!UICONTROL 表单]** 组件。

   ![](assets/lp-call-to-action.png)

1. 定义单击按钮时将发生的操作：

   * **[!UICONTROL 确认页面]**：用户将被重定向到 **[!UICONTROL 确认]** 页面集。

   * **[!UICONTROL 重定向URL]**：输入用户将被重定向到的页面的URL。

1. 如果要在提交表单时进行其他更新，请选择 **[!UICONTROL 其他更新]**，选择 **[!UICONTROL 选择加入]** 或 **[!UICONTROL 选择禁用]**，并定义是要更新订阅列表、渠道还是只更新使用的电子邮件地址。

   ![](assets/lp-form-additionnal-updates.png)

1. 保存您的内容以返回至 [登陆页面属性](create-lp.md).

## 定义登陆页面表单样式 {#lp-form-styles}

1. 要修改表单组件内容的样式，请随时切换到 **[!UICONTROL 样式]** 选项卡。

   ![](assets/lp_designer-form-style.png)

1. 此 **[!UICONTROL 字段]** 默认情况下，部分处于扩展状态，允许您编辑文本字段的外观，如标签和占位符字体、标签位置、字段背景颜色或字段边框。

   ![](assets/lp_designer-form-style-fields.png)

1. 展开 **[!UICONTROL 复选框]** 部分定义复选框和相应文本的外观。 例如，您可以调整字体系列或大小，或复选框边框颜色。

   ![](assets/lp_designer-form-style-checkboxes.png)

1. 展开 **[!UICONTROL 按钮]** 部分，以修改组件窗体中按钮的外观。 例如，您可以更改字体、添加边框、在光标悬停时编辑标签颜色或调整按钮的对齐方式。

   ![](assets/lp_designer-form-style-buttons.png)

   您可以使用来预览某些设置，例如悬停时的按钮标签颜色 **[!UICONTROL 模拟内容]** 按钮。 了解有关测试登陆页面的更多信息 [此处](create-lp.md#test-landing-page).

1. 展开 **[!UICONTROL 表单布局]** 区域以编辑布局设置，如背景颜色、填充或边距。

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

