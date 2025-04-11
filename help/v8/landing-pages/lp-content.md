---
title: 定义特定于登陆页面的内容
description: 了解如何在Campaign Web中设计登陆页面特定内容
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 12%

---

# 定义特定于登陆页面的内容 {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="使用内容组件"
>abstract="内容组件是空的内容占位符，您可用它来创建登陆页面的版面。要定义允许用户选择和提交其选择的特定内容，请使用表单组件。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="定义主页面设置"
>abstract="用户单击指向登陆页面的链接后（例如通过电子邮件或网站），会立即向用户显示主页面。"

您可以编辑登陆页面中任何页面的内容。

第一个页面（在用户单击指向您的登陆页面的链接后立即向用户显示）已预填充了选定模板<!-- to enable users to select and submit their choices-->的[特定于登陆页面的表单组件](#use-form-component)。

**[!UICONTROL Confirmation]**、**[!UICONTROL Error]**&#x200B;和&#x200B;**[!UICONTROL Expiration]**&#x200B;页面的内容也已预填充。 根据需要编辑它们。

您还可以为登陆页面](#lp-form-styles)定义[样式。

要进一步设计登陆页面内容，请执行以下操作：

* 使用与设计电子邮件时使用的组件相同的组件。 [了解详情](../email/content-components.md#add-content-components)

* 以与电子邮件相同的方式向登陆页面添加条件内容。 [了解详情](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >此功能位于有限可用性(LA)中。 仅供&#x200B;**从 Adobe Campaign Standard 迁移到 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境上。

## 使用表单组件 {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="设置表单组件字段"
>abstract="定义您的收件人如何从登陆页面查看和提交他们的选择。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="单击按钮时会出现的情况"
>abstract="定义在用户提交登陆页面表单时将会出现的情况。"

要定义特定内容以允许用户从登陆页面选择并提交他们的选择，请编辑&#x200B;**[!UICONTROL 表单]**&#x200B;组件。 请按照以下步骤操作。

1. 登录页特定的&#x200B;**[!UICONTROL 表单]**&#x200B;组件已显示在所选模板的画布中。

   >[!NOTE]
   >
   >**[!UICONTROL Form]**&#x200B;组件只能在同一页面上使用一次。

1. 选择它。 **[!UICONTROL 表单内容]**&#x200B;选项卡显示在右侧面板中，允许您编辑表单的不同字段。

   ![表单组件显示在画布中](assets/lp-form-component.png){zoomable="yes"}

   >[!NOTE]
   >
   >随时切换到&#x200B;**[!UICONTROL 样式]**&#x200B;选项卡以编辑表单组件内容的样式。 [了解详情](#lp-form-styles)

1. 展开第一个文本字段（如果有），或使用&#x200B;**[!UICONTROL 添加]**&#x200B;按钮添加一个文本字段。 从&#x200B;**[!UICONTROL 文本字段1]**&#x200B;部分，编辑字段类型、要更新的数据库字段、标签以及显示在字段中的文本，然后用户输入值。

   ![表单组件中的文本字段设置](assets/lp-form-text-field.png){zoomable="yes"}

1. 根据需要选中&#x200B;**[!UICONTROL 将表单字段设为必填]**&#x200B;选项。 在这种情况下，仅当用户填写此字段后才能提交登陆页面。

   >[!NOTE]
   >
   >如果未填写必填字段，则用户提交页面时会显示错误消息。

1. 展开此复选框（如果有），或使用&#x200B;**[!UICONTROL 添加]**&#x200B;按钮添加此复选框。 选择该复选框应更新数据库中的服务或字段。

   ![表单组件中的复选框设置](assets/lp-form-checkbox.png){zoomable="yes"}

   如果您选择&#x200B;**[!UICONTROL 订阅和服务]**，请从列表中选择[服务](../audience/manage-services.md)，然后在以下两个选项之间进行选择：

   * **[!UICONTROL 如果选中，则订阅]**：用户需要选中复选框才能同意（选择加入）。
   * **[!UICONTROL 如果选中，则取消订阅]**：用户需要选中此框以移除其同意（选择退出）。

   如果选择&#x200B;**[!UICONTROL 字段]**，请从[属性列表](../get-started/attributes.md)中选择一个字段，然后在以下两个选项之间进行选择：

   * 如果选中&#x200B;**[!UICONTROL 是]**。
   * 如果选中&#x200B;**[!UICONTROL 否]**。

1. 根据需要删除和添加任意数量的字段（例如文本字段、单选按钮、复选框、下拉列表等）。

1. 添加或更新所有字段后，单击&#x200B;**[!UICONTROL 行动号召]**&#x200B;展开相应的部分。 它允许您定义&#x200B;**[!UICONTROL 表单]**&#x200B;组件中按钮的行为。 [了解如何操作](#define-actions-on-form-submission)

   ![表单组件中的行动号召设置](assets/lp-call-to-action.png){zoomable="yes"}

1. 保存您的内容以返回[登陆页面属性](create-lp.md#create-landing-page)。

### 定义针对表单提交的操作 {#define-actions-on-form-submission}

1. 定义单击按钮后执行的操作：

   * **[!UICONTROL 确认页面]**：默认情况下，用户将被重定向到为当前登陆页设置的&#x200B;**[!UICONTROL 确认]**&#x200B;页面。

   * **[!UICONTROL 重定向URL]**：输入用户被重定向到的页面的URL。

   * **[!UICONTROL 登陆页面]**：选择用户要重定向到的其他登陆页面。 确保相应地配置选定的登陆页面。

1. 要在提交表单时进行其他更新，请选择&#x200B;**[!UICONTROL 其他更新]**，然后选择要更新的项目：
   * 订阅[服务](../audience/manage-services.md) — 定义您要在提交表单时选择加入还是选择退出用户。 在设计电子邮件时，如果您定义指向此登陆页面的&#x200B;**[!UICONTROL 登陆页面]**&#x200B;类型的链接，则将自动使用选定的服务。 [了解有关插入链接的更多信息](../email/message-tracking.md)

     >[!NOTE]
     >
     >如果要在此登陆页中使用多个服务，请使用如下所述的&#x200B;**[!UICONTROL 来自URL的服务]**&#x200B;选项。

   * 渠道 — 填写表单时使用的电子邮件地址。
   * 所有渠道 — 提交表单时，用户将选择加入或退出（取决于所选模板），以进入或退出所有渠道上来自您品牌的所有通信。
   * 数据库中的字段 — 从属性列表中选择一个字段，并定义在提交表单时该字段应设置为True还是False。

   ![表单组件中的其他更新设置](assets/lp-form-additionnal-updates.png){zoomable="yes"}

1. 选择“**[!UICONTROL 服务来自URL]**”选项，以允许将登陆页用于多个服务，使其成为动态页面。 定义在提交表单时要选择加入还是选择退出用户。

   >[!AVAILABILITY]
   >
   >此功能位于有限可用性(LA)中。 仅供&#x200B;**从 Adobe Campaign Standard 迁移到 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境上。

   来自表单组件](assets/lp-form-service-from-url.png){zoomable="yes"}中的URL设置的![服务

   在设计电子邮件时，如果您定义指向此登陆页面的&#x200B;**[!UICONTROL 登陆页面]**&#x200B;类型的链接，则可以从列表中选择任何服务。 然后，在定义指向此登陆页面的其他链接时，您可以选择其他服务。 [了解有关插入链接的更多信息](../email/message-tracking.md)

   ![电子邮件链接至登陆页面设置](assets/email-link-to-landing-page.png){zoomable="yes"}

1. 发送登陆页面提交消息。 [在此处了解详情](#lp-message)

### 提交后发送消息 {#lp-message}

>[!AVAILABILITY]
>
>此功能位于有限可用性(LA)中。 仅供&#x200B;**从 Adobe Campaign Standard 迁移到 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境上。

要在提交登陆页面后自动发送确认消息，请执行以下步骤：

1. 在&#x200B;**[!UICONTROL 行动号召]**&#x200B;部分中，选中&#x200B;**[!UICONTROL 发送确认电子邮件]**&#x200B;选项。

1. 在关联的下拉列表中，选择需要发送的事务型消息模板。

![表单组件中的确认电子邮件设置](assets/lp-confirmation.png){zoomable="yes"}

## 定义登陆页面表单样式 {#lp-form-styles}

1. 要修改表单组件内容的样式，请随时切换到&#x200B;**[!UICONTROL 样式]**&#x200B;选项卡。

1. 默认情况下，**[!UICONTROL 文本字段]**&#x200B;部分处于扩展状态。 它允许您编辑文本字段的外观，如标签字体、标签位置、字段背景颜色或字段边框。

   ![文本字段样式设置](assets/lp-text-styles.png){zoomable="yes"}

1. 展开&#x200B;**[!UICONTROL 复选框]**&#x200B;部分以定义复选框和相应文本的外观。 例如，调整字体系列和大小，或复选框边框颜色。

   ![复选框样式设置](assets/lp-checkbox-style.png){zoomable="yes"}

1. 展开并编辑与您可能已添加到表单的其他字段（单选按钮、下拉列表、日期和时间等）对应的任何其他部分。

1. 展开&#x200B;**[!UICONTROL 行动号召]**&#x200B;部分以修改组件表单中按钮的外观。 例如，更改字体、添加边框、在光标悬停时编辑标签颜色或调整按钮的对齐方式。

   ![行动号召样式设置](assets/lp-call-to-action-style.png){zoomable="yes"}

   使用&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮预览某些设置，例如悬停时的按钮标签颜色。 [了解详情](create-lp.md#test-landing-page)

1. 保存您的更改。