---
audience: end-user
title: 将可视片段添加到电子邮件
description: 了解如何将可视化片段添加到您的电子邮件
badge: label="有限发布版"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 14%

---

# 将可视片段添加到电子邮件 {#use-visual-fragments}

>[!AVAILABILITY]
>
>此功能需要更新Campaign v8.6.4。请参阅[Campaign v8客户端控制台发行说明](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/releases/release-notes)以了解详情。

在Campaign Web界面中，**可视化片段**&#x200B;是预定义的可视化块，您可以在多个[电子邮件投放](../email/get-started-email-designer.md)或[内容模板](../email/use-email-templates.md)中重复使用。 在[本节](fragments.md)中了解如何创建和管理内容片段。

![](assets/do-not-localize/fragments.gif)

## 使用可视片段 {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="片段选项"
>abstract="此窗格提供与所选片段相关的选项。它允许您选择想要显示片段的设备，并打开该片段的内容。使用 **[!UICONTROL 样式]** 选项卡进一步自定义您的片段。您还可以打破与原始视觉片段的继承。"

<!-- pas vu dans l'UI-->

要在电子邮件内容中插入可视片段，请执行以下步骤：

1. 使用[电子邮件Designer](../email/get-started-email-designer.md)打开任何电子邮件或模板内容。

1. 从左边栏中选择&#x200B;**[!UICONTROL 片段]**&#x200B;图标。

   ![](assets/fragments-in-designer.png)

1. 此时将显示在当前沙盒中创建的所有可视化片段的列表。 您可以：

   * 通过开始键入特定片段的标签来搜索该片段。
   * 按升序或降序对片段排序。
   * 更改片段的显示方式（卡片视图或列表视图）。

   >[!NOTE]
   >
   >片段按创建日期排序：最近添加的片段首先显示在列表中。

   如果在编辑内容时修改或添加了某些可视化片段，请单击&#x200B;**刷新**&#x200B;图标以使用最新更改更新列表。

1. 将列表中的任何可视化片段拖放到要插入它的区域。 与任何其他组件一样，您可以在内容中移动片段。

1. 选择片段以在右侧窗格中显示其选项。

   ![](assets/fragment-right-pane.png)

   在&#x200B;**[!UICONTROL 设置]**&#x200B;选项卡中，您可以：

   * 选择您希望片段显示的设备。
   * 单击&#x200B;**编辑内容**&#x200B;按钮以打开此片段的内容。 [了解详情](../content/fragments.md#edit-fragments)

     您可以使用&#x200B;**[!UICONTROL 样式]**&#x200B;选项卡进一步自定义片段。

1. 如果需要，您可以使用原始可视片段中断继承。 [了解详情](#break-inheritance)

   您还可以从内容中删除或复制片段。 这些操作可以直接从片段顶部显示的上下文菜单执行。

1. 添加所需数量的可视化片段，并&#x200B;**[!UICONTROL 保存]**&#x200B;您的更改。

### 只读模式下的可视化片段 {#fragment-readonly}

访问权限可能会应用于可视化片段。

如果您没有特定可视化片段的编辑权限，则内容模板将以&#x200B;**只读模式**&#x200B;显示。 在这种情况下，**[!UICONTROL 编辑内容]**&#x200B;按钮将替换为&#x200B;**[!UICONTROL 查看内容]**&#x200B;按钮，从而允许您在不进行任何更改的情况下查看片段。

![](assets/fragment-readonly.png){zoomable="yes"}

如下所示，所有功能图标都已停用，将交互限制为仅查看。

![](assets/fragment-readonly-view.png){zoomable="yes"}

## 中断继承 {#break-inheritance}

编辑可视片段时，将同步更改。 它们会自动传播到包含该片段的所有电子邮件投放和内容模板。

添加到电子邮件或内容模板时，片段默认进行同步。

但是，您可以中断来自原始片段的继承。 在这种情况下，片段的内容将被复制到当前设计中，并且更改不再同步。

要中断继承，请执行以下步骤：

1. 选择可视片段。

1. 单击上下文工具栏中的解锁图标。

   ![](assets/fragment-break-inheritance.png)

1. 该片段将成为不再链接到原始片段的独立元素。 可将其编辑为内容中的任何其他内容组件。 [了解详情](../email/content-components.md)
