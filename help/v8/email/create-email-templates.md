---
audience: end-user
product: campaign
title: 使用内容模板
description: 了解如何创建模板以重复使用Adobe Campaign电子邮件中的内容
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 17%

---

# 使用内容模板 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="内容模板"
>abstract="为了加快并改进设计流程，您可以创建独立的电子邮件模板，从而轻松地在 Adobe Campaign 中重复使用自定义内容。这些内容模板可以从头开始设计，根据内置或自定义模板设计，从现有内容创建，也可以导入到内容模板编辑器中。"

为了加快并改进设计过程，您可以创建独立的模板，以轻松地在上下文中重复使用自定义内容 [!DNL Adobe Campaign]. 这些内容模板可以从头开始设计，根据内置或自定义模板设计，从现有内容创建，也可以导入到内容模板编辑器中。

此功能使面向内容的用户能够使用独立的模板，以便营销用户可以重复使用并在其自己的电子邮件促销活动中调整模板。

>[!NOTE]
>
>当前仅限 **电子邮件** 支持内容模板。

## 访问内容模板 {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="编辑您的模板内容"
>abstract="单击&#x200B;**编辑内容**&#x200B;按钮可使用电子邮件设计器更新您的内容。"

要访问内容模板列表，请浏览至 **[!UICONTROL 内容管理]** > **[!UICONTROL 内容模板]** 菜单。

![](assets/content-template-list.png){zoomable=&quot;yes&quot;}

此仪表板将所有可用的内容模板显示为列表。 您可以根据特定的 [文件夹](../get-started/permissions.md#folders) 使用下拉列表或使用添加规则 [查询建模器](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png){zoomable=&quot;yes&quot;}

从该列表中，您可以编辑、复制或删除现有内容模板。 使用上半部分的按钮可创建内容模板。


## 创建内容模板 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="内容模板设计"
>abstract="内容模板设计"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="内容模板选择"
>abstract="内容模板选择"

内容模板可以通过以下方式创建 [将现有电子邮件另存为模板](#save-as-template)，或从电子邮件模板列表中，通过 **创建内容模板** 按钮， [如下所述](#create-template-from-scratch).

保存后，您现在可以在构建任何 [电子邮件](../email/create-email.md) 范围 [!DNL Adobe Campaign]. [了解如何操作](use-email-templates.md)

>[!NOTE]
>
>* 对内容模板所做的更改不会传播到电子邮件。
>
>* 同样，在电子邮件中使用模板时，您对电子邮件内容所做的任何编辑都不会影响以前使用的内容模板。

### 创建新的内容模板 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="定义模板属性"
>abstract="定义您的电子邮件内容模板属性，以便在需要时轻松检索。"

要从内容模板仪表板中创建新内容模板，请执行以下步骤：

1. 从浏览内容模板列表 **[!UICONTROL 内容管理]** > **[!UICONTROL 内容模板]** 左边栏。

1. 选择 **[!UICONTROL 创建模板]**.

   ![](assets/content-template-create.png){zoomable=&quot;yes&quot;}

1. 输入模板标签和属性。 您可以选择要存储模板的文件夹。 默认情况下，内容模板存储在Adobe Campaign层次结构的专用文件夹中： **[!UICONTROL 资源管理器]** > **[!UICONTROL 资源]** > **[!UICONTROL 模板]** > **[!UICONTROL 内容模板]**. 了解有关文件夹的详细信息 [此页面](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png){zoomable=&quot;yes&quot;}

1. 单击 **[!UICONTROL 创建]** 并从不同的选项中选择所需的模板设计方式：

   * [从头开始设计内容](create-email-content.md) 通过Email Designer的界面。

   * [编码或复制粘贴原始HTML](code-content.md) 直接导入Email Designer。

   * [导入现有HTML内容](existing-content.md) 从文件或.zip文件夹中。

   * 使用内置或自定义模板列表中的现有内容。 有关在电子邮件中使用内容模板的步骤，请参阅 [本节](use-email-templates.md).

   ![](assets/email_designer-templates.png){zoomable=&quot;yes&quot;}

1. 此时将显示Email Designer。 根据所选选项，根据需要编辑内容，就像对任何电子邮件执行编辑操作一样。 了解如何在中使用电子邮件设计器 [本节](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. 模板准备就绪后，单击 **[!UICONTROL 保存]**.

   如果需要，单击模板名称旁边的箭头以返回 **[!UICONTROL 详细信息]** 屏幕并编辑您的模板。

   ![](assets/content-template-save-back.png){zoomable=&quot;yes&quot;}

该模板位于 **[!UICONTROL 内容模板]** 列表。 [了解详情](#access-templates)

您现在可以使用此模板来构建新内容：此模板位于 **[!UICONTROL 已保存模板]** 选项卡。 [了解如何操作](use-email-templates.md)

### 将电子邮件内容另存为模板 {#save-as-template}

一旦您 [设计了一封电子邮件](create-email-content.md)，您可以将此内容另存为模板以供将来重用。 保存的模板可供 Adobe Campaign 环境的所有用户使用。

要将电子邮件内容另存为模板，请执行以下步骤：

1. 在电子邮件设计器中，单击 **[!UICONTROL 更多]** 按钮。

1. 选择 **[!UICONTROL 另存为内容模板]** 从下拉菜单中。

   ![](assets/email_designer-save-template.png){zoomable=&quot;yes&quot;}

1. 输入此模板的名称，然后保存。

   ![](assets/email_designer-template-name.png){zoomable=&quot;yes&quot;}

模板将保存并显示在 **[!UICONTROL 内容模板]** 列表。 它会变成一个独立的内容模板，可以像该列表中的任何其他项目一样访问、编辑和删除该模板。 [了解详情](#access-manage-templates)

您现在可以使用此模板来构建新内容：此模板位于 **[!UICONTROL 已保存模板]** 选项卡。 [了解如何操作](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable=&quot;yes&quot;}


>[!NOTE]
>
>对该新模板所做的任何更改都不会传播到该模板所来自的电子邮件中。 同样，在该电子邮件中编辑原始内容时，不会修改新模板。

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## 修改内容模板 {#modify-delete}

要更新现有内容模板，请执行以下步骤：

1. 从内容模板列表中，单击要修改的模板的标签以对其进行编辑。

1. 单击 **[!UICONTROL 编辑内容]** 按钮以使用更新您的内容 [电子邮件设计工具](get-started-email-designer.md).

![](assets/content-template-edition.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>使用此内容模板时，对内容模板所做的更改不会传播到电子邮件。

## 删除内容模板 {#content-delete}

您可以通过两种方式删除内容模板：

* 从内容模板列表中，单击省略号按钮，然后选择 **删除**

  ![从功能板中删除内容模板](assets/content-template-list-delete.png)

* 从内容模板本身，单击 **更多** 按钮，然后选择 **删除**


>[!NOTE]
>
>删除内容模板不会影响使用此模板创建的投放。


## 复制内容模板 {#content-duplicate}

复制内容模板的方法有两种：

* 从内容模板列表中，单击省略号按钮，然后选择 **复制**

* 从内容模板本身，单击 **更多** 按钮，然后选择 **复制**

在这两种情况下，确认复制以创建新内容模板。 新内容模板的标签为 **副本`<label of the initial campaign`**. 浏览到模板设置以更新此标签。

