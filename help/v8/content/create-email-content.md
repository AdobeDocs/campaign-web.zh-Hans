---
audience: end-user
title: 在电子邮件设计器中设计电子邮件
description: 了解如何从头开始设计电子邮件内容
exl-id: 23e71da3-434d-4619-a48a-334281592d85
badge: label="Alpha" type="Positive"
source-git-commit: d7e19b2d8730cacbbff1ad42f1956b32c84a309a
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 100%

---

# 从头开始设计电子邮件内容 {#create-email-content}

>[!CONTEXTUALHELP]
>id="ac_structure_components_email"
>title="关于结构组件"
>abstract="结构组件定义电子邮件的版面。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_landing_page"
>title="关于结构组件"
>abstract="结构组件定义登陆页面的版面。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_fragment"
>title="关于结构组件"
>abstract="结构组件定义片段的版面。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_template"
>title="关于结构组件"
>abstract="结构组件定义模板的版面。"


>[!CONTEXTUALHELP]
>id="ac_edition_columns_email"
>title="定义电子邮件列"
>abstract="使用电子邮件设计器，您可以通过定义列结构来轻松定义电子邮件的版面。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_landing_page"
>title="定义登陆页面列"
>abstract="使用电子邮件设计器，您可以通过定义列结构来轻松定义登陆页面的版面。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_fragment"
>title="定义片段列"
>abstract="使用电子邮件设计器，您可以通过定义列结构来轻松定义片段的版面。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_template"
>title="定义模板列"
>abstract="使用电子邮件设计器，您可以通过定义列结构来轻松定义模板的版面。"

使用电子邮件设计器，您可以轻松定义电子邮件的结构。通过使用简单的拖放操作来添加和移动结构元素，可以在几秒钟内设计出电子邮件正文。

要开始生成电子邮件内容，请执行以下步骤：

1. 从电子邮件设计器主页中，选择&#x200B;**[!UICONTROL 从头开始设计]**&#x200B;选项。

   ![](assets/email_designer.png)

1. 通过将&#x200B;**[!UICONTROL 结构组件]**&#x200B;拖放到画布中来定义电子邮件版面，从而开始设计电子邮件内容。

   >[!NOTE]
   >
   >堆叠列并非与所有电子邮件程序都兼容。在不受支持时，不会堆叠列。

   <!--Once placed in the email, you cannot move nor remove your components unless there is already a content component or a fragment placed inside. This is not true in AJO - TBC?-->

   ![](assets/email_designer_2.png)

1. 添加所需数量的&#x200B;**[!UICONTROL 结构组件]**，并在右侧的专用窗格中编辑其设置。

   选择 **[!UICONTROL n:n 列]**&#x200B;组件来定义所选列数（3 和 10 之间）。还可以通过移动每个列底部的箭头来定义该列的宽度。

   >[!NOTE]
   >
   >每个列的大小不能小于结构组件的总宽度的 10%。不能删除非空列。

1. 展开&#x200B;**[!UICONTROL 内容组件]**&#x200B;部分，并将所需数量的元素添加到一个或多个结构组件中。[详细了解内容组件](content-components.md)

1. 可以使用右侧的&#x200B;**[!UICONTROL 组件设置]**&#x200B;窗格进一步自定义每个组件。例如，您可以更改每个组件的文本样式、内边距或边距。[了解有关对齐方式和内边距的更多信息](alignment-and-padding.md)

   ![](assets/email_designer_5.png)

1. 插入个性化字段以从配置文件数据自定义电子邮件内容。[详细了解内容个性化](../personalization/personalize.md)

1. 单击左侧窗格中的&#x200B;**[!UICONTROL 链接]**&#x200B;选项卡以显示必须跟踪的内容的所有 URL。可以修改其&#x200B;**[!UICONTROL 跟踪类型]**&#x200B;或&#x200B;**[!UICONTROL 标签]**，并添加&#x200B;**[!UICONTROL 类别]**（如果需要）。[详细了解链接和邮件跟踪](message-tracking.md)

   ![](assets/email_designer_7.png)

1. 如果需要，可以通过单击高级菜单中的&#x200B;**[!UICONTROL 切换到代码编辑器]**&#x200B;来进一步个性化电子邮件。例如，这允许您编辑电子邮件源代码以添加跟踪或自定义 HTML 标记。[详细了解代码编辑器](code-content.md)

   >[!CAUTION]
   >
   >切换到代码编辑器后，无法恢复到此电子邮件的可视设计器。

1. 在内容准备就绪后，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;以检查电子邮件渲染。可以选择桌面或移动视图。[详细了解预览电子邮件](../preview-test/preview-test.md)

   ![](assets/email_designer_28.png)

1. 在电子邮件就绪后，单击&#x200B;**[!UICONTROL 保存]**。

