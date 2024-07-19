---
audience: end-user
title: 创建内容片段
description: 了解如何使用内容片段创建
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: 2d6b885642fbb6e1545f899219db05c156b069c4
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 24%

---

# 创建内容片段 {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="定义您自已的片段"
>abstract="片段是一个可重复使用的组件，可以在各种营销活动中的一封或多封电子邮件中引用。此功能用于预构建多个自定义内容块，营销用户可以使用这些块在改进的设计过程中快速组装电子邮件内容。"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="片段保存"
>abstract="片段保存"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="定义您自已的片段"
>abstract="片段是一个可重复使用的组件，可以在各种营销活动中的一封或多封电子邮件中引用。"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="片段属性"
>abstract="片段属性"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="片段类型"
>abstract="选择片段类型。目前，仅提供适用于电子邮件的视觉片段。"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="定义您自已的片段"
>abstract="片段是一个可重复使用的组件，可以在各种营销活动中的一封或多封电子邮件中引用。您还可以在电子邮件模板中使用片段。目前，只有视觉片段可用。"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="片段详情"
>abstract="片段详情"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="定义您自已的片段"
>abstract="片段是一个可重复使用的组件，可以在各种营销活动中的一封或多封电子邮件中引用。"

片段是一个可重复使用的组件，可以在各种营销活动中的一封或多封电子邮件中引用。修改片段时，使用该片段的每个内容都会更新。

此功能允许预先构建多个自定义内容块，营销用户可以使用这些内容块在改进的设计过程中快速组合电子邮件内容。

![](assets/fragments.gif)

要充分利用片段，请执行以下操作：

* 创建您自己的可视化片段，如下所述。
* 您可以根据需要通过Email Designer在内容中多次使用它们。 请参阅[将可视化片段添加到您的电子邮件](../email/use-visual-fragments.md)。

>[!AVAILABILITY]
>
>此功能位于有限可用性(LA)中。 仅供&#x200B;**从 Adobe Campaign Standard 迁移到 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境上。

## 创建可视片段 {#create-fragments}

创建片段的方法有两种：

* 使用&#x200B;**[!UICONTROL 片段]**&#x200B;专用菜单从头开始创建片段。 [了解如何操作](#create-from-scratch)

* 设计内容时，将部分内容另存为片段。 [了解如何操作](#save-as-fragment)

保存后，您的片段即可用于电子邮件或电子邮件模板。 无论是从头开始还是从现有内容创建，您现在都可以在在Campaign中构建任何内容时使用此片段。 请参阅[添加可视化片段](../email/use-visual-fragments.md)。

### 从头开始创建片段 {#create-from-scratch}

要从头开始创建片段，请执行以下步骤。

1. [通过&#x200B;**[!UICONTROL 内容管理]** > **[!UICONTROL 片段]**&#x200B;左侧菜单访问片段列表](#access-manage-fragments)。

   ![](assets/fragments-list.png)

1. 选择&#x200B;**[!UICONTROL 创建片段]**。

1. 输入片段的标签。

   ![](assets/fragment-create.png)

1. 如果需要，您可以定义其他选项，如片段内部名称、其文件夹和描述。

   >[!NOTE]
   >
   >目前，您只能创建可视化片段。

1. 单击&#x200B;**创建**&#x200B;按钮配置片段的内容。

1. 显示[电子邮件Designer](../email/get-started-email-designer.md)。 根据需要编辑内容，就像处理营销活动中的任何电子邮件一样。 您可以添加图像、链接、个性化字段和动态内容。

   ![](assets/fragment-designer.png)

1. 片段准备就绪后，单击&#x200B;**[!UICONTROL 保存并关闭]**。 已将其添加到[片段列表](#access-manage-fragments)。

现在，在Campaign中构建任何[电子邮件](../email/get-started-email-designer.md)或[内容模板](use-email-templates.md)时，可使用此片段。 [了解如何操作](../email/use-visual-fragments.md)


### 将内容另存为片段 {#save-as-fragment}

任何电子邮件内容都可以另存为片段以供将来重用。 在设计[内容模板](use-email-templates.md)或[电子邮件](../email/get-started-email-designer.md)投放时，您可以将部分内容另存为可视片段。 为此请执行以下操作步骤：

1. 在[电子邮件Designer](../email/get-started-email-designer.md)中，单击屏幕右上角的&#x200B;**更多**&#x200B;按钮。

1. 从下拉菜单中选择&#x200B;**[!UICONTROL 另存为片段]**。

   ![](assets/fragment-save-as.png)

1. 将显示&#x200B;**[!UICONTROL 另存为片段]**&#x200B;屏幕。 其中选择要包含在片段中的元素，包括个性化字段和动态内容。

   >[!CAUTION]
   >
   >只能选取彼此相邻的部分。 您不能选择空的结构或其他片段。

   ![](assets/fragment-save-as-screen.png)

1. 单击&#x200B;**[!UICONTROL 创建]**。填写片段名称并保存。

   ![](assets/fragment-save-confirm.png)

   此内容现在是独立的片段，添加到[片段列表](#manage-fragments)中，可从专用菜单访问。 现在，在Campaign中构建任何[电子邮件](../email/get-started-email-designer.md)或[内容模板](use-email-templates.md)时，可以使用此片段。 [了解如何操作](../email/use-visual-fragments.md)

>[!NOTE]
>
>对该新片段所做的任何更改都不会传播到它来自的电子邮件或模板。 同样，在该电子邮件或模板中编辑原始内容时，不会修改新片段。

## 管理您的片段 {#manage-fragments}

您可以从片段列表中编辑、更新、复制或删除片段。

### 编辑和更新片段 {#edit-fragments}

要编辑片段，请执行以下步骤。

1. 从&#x200B;**[!UICONTROL 片段]**&#x200B;列表中单击要编辑的片段的名称。
1. 单击&#x200B;**编辑内容**&#x200B;按钮以打开此片段的内容。

   ![](assets/fragment-edit-content.png)

1. 进行必要的更改并保存修改。

>[!CAUTION]
>
>对片段所做的任何更改都会传播到使用该片段的电子邮件投放或模板中。


### 删除片段 {#delete-fragments}

要删除片段，请执行以下步骤：

1. 浏览到片段列表，然后单击要删除的片段旁边的&#x200B;**[!UICONTROL 更多操作]**&#x200B;按钮。
1. 单击&#x200B;**删除**&#x200B;并确认。

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>删除内容片段时，会更新电子邮件投放和使用它的模板：片段将从电子邮件内容中删除，但仍被引用。 要将片段内容保留在这些投放和模板中，必须在删除片段之前中断继承，[如本节](use-visual-fragments.md#break-inheritance)所述。
>

### 复制片段 {#duplicate-fragments}

您可以轻松复制片段以创建新片段。 要复制现有片段，请执行以下步骤：

1. 浏览到片段列表，然后单击要删除的片段旁边的&#x200B;**[!UICONTROL 更多操作]**&#x200B;按钮。
1. 单击&#x200B;**复制**&#x200B;并确认。
1. 输入新片段的标签并保存更改。

   片段将添加到片段列表。 您可以根据需要对其进行编辑和配置。
