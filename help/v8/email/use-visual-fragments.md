---
audience: end-user
title: 将可视片段添加到电子邮件
description: 了解如何将可视化片段添加到您的电子邮件
hide: true
hidefromtoc: true
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: f96c807c2ee094ad4775b6bf56f5f02822da8d28
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 4%

---

# 将可视片段添加到电子邮件 {#use-visual-fragments}

您可以在以下位置使用可视化片段： [电子邮件投放](get-started-email-designer.md)，或在 [内容模板](use-email-templates.md). 步骤详见下文。


>[!NOTE]
>
>了解如何在中创建和管理片段 [本节](fragments.md).


## 使用片段 {#use-fragment}

要在电子邮件内容中插入片段，请执行以下步骤：

1. 使用打开任何电子邮件或模板内容 [电子邮件设计工具](get-started-email-designer.md).

1. 选择 **[!UICONTROL 片段]** 图标。

   ![](assets/fragments-in-designer.png)

1. 此时将显示在当前沙盒中创建的所有可视化片段的列表。 您可以：

   * 通过开始键入特定片段的标签来搜索该片段。
   * 按升序或降序对片段排序。
   * 更改片段的显示方式（卡片视图或列表视图）。

   >[!NOTE]
   >
   >片段按创建日期排序：最近添加的可视化片段首先显示在列表中。

   如果在编辑内容时修改或添加了某些片段，请单击 **刷新** 图标以使用最新更改更新列表。

1. 将列表中的任何片段拖放到要插入它的区域。 与任何其他组件一样，您可以在内容中移动片段。

1. 选择片段以在右侧窗格中显示其选项。

   ![](assets/fragment-right-pane.png)

   从 **[!UICONTROL 设置]** 选项卡，您可以：

   * 选择您希望片段显示的设备。
   * 
      1. 单击 **编辑内容** 按钮以打开此片段的内容。 [了解详情](../email/fragments.md#edit-fragments)

     您可以使用进一步自定义片段 **[!UICONTROL 样式]** 选项卡。

1. 如果需要，您可以使用原始片段中断继承。 [了解详情](#break-inheritance)
您还可以从内容中删除或复制片段。 这些操作可以直接从片段顶部显示的上下文菜单执行。

1. 添加所需数量的片段并 **[!UICONTROL 保存]** 您所做的更改。

## 中断继承 {#break-inheritance}

编辑可视片段时，将同步更改。 它们会自动传播到包含该片段的所有电子邮件投放和内容模板。

添加到电子邮件或内容模板时，片段默认进行同步。

但是，您可以中断来自原始片段的继承。 在这种情况下，片段的内容将被复制到当前设计中，并且更改不再同步。

要中断继承，请执行以下步骤：

1. 选择片段。

1. 单击上下文工具栏中的解锁图标。

   ![](assets/fragment-break-inheritance.png)

1. 该片段将成为不再链接到原始片段的独立元素。 可将其编辑为内容中的任何其他内容组件。 [了解详情](content-components.md)
