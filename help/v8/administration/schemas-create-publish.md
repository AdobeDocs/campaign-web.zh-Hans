---
title: 创建和发布架构
description: 了解如何创建、扩展和发布架构。
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# 创建和发布架构 {#create-publish}

## 创建和管理架构 {#create-schemas}

您可以创建新架构、扩展现有架构以及访问外部数据库。

### 创建或扩展架构 {#create-new}

创建或扩展方案：

1. 导航到&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL 架构]**。
1. 单击&#x200B;**[!UICONTROL 创建架构]**。

   ![架构创建对话框](assets/schemas-create1.png)

1. 输入架构的命名空间（例如，`cus`用于自定义架构）。
1. 输入唯一的名称和标签，然后选择是要创建新架构还是扩展现有架构。

1. 单击&#x200B;**[!UICONTROL 创建]**。
   ![架构创建对话框](assets/schemas-create2.png)

将创建架构并显示生成的架构结构。

默认情况下，架构为空。 现在，您需要使用架构编辑器添加要包含在架构中的字段：

1. 在架构详细信息屏幕的&#x200B;**[!UICONTROL Content]**&#x200B;部分中单击铅笔图标。
2. 添加所需的元素并保存。 以下是自定义架构结构的示例：

   ![架构创建对话框](assets/schemas-create3.png)

系统自动验证XML结构并生成架构。

### 定义屏幕版本 {#define-attributes}

创建架构后，您需要定义屏幕版本。

有关屏幕定义屏幕以及如何对其进行访问的更多信息，请参阅[访问屏幕定义](schemas-browse-access.md#screen-def)部分。

在我们的示例中，我们只添加两个自定义字段：

1. 单击架构详细信息视图中的&#x200B;**[!UICONTROL 屏幕版本]**&#x200B;按钮以访问屏幕定义。

1. 单击&#x200B;**[!UICONTROL 自定义字段列表]**&#x200B;表上方的省略号图标，然后选择&#x200B;**[!UICONTROL 选择属性]**。
1. 选择要添加的自定义字段并进行确认。

   ![架构创建对话框](assets/schemas-create4.png)

## 发布并同步架构 {#publish}

创建或修改模式后，您需要发布该模式，以将逻辑模式与物理数据库结构同步。

### 发布架构更改 {#publish-changes}

>[!CAUTION]
>
>发布模式更改会修改数据库结构。 在确认发布之前，请确保您了解这些更改的影响。

要发布架构更改，请执行以下操作：

1. 导航到&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL 架构]**&#x200B;以访问架构列表。
1. 单击&#x200B;**[!UICONTROL 发布]**&#x200B;并确认。

   ![架构发布对话框，显示要应用的更改](assets/schemas-publish1.png)

1. 在列表中选择要同步的架构。

   ![架构发布对话框，显示要应用的更改](assets/schemas-publish2.png)

1. 查看将执行以更新数据库结构的SQL脚本。
1. 单击&#x200B;**[!UICONTROL 发布]**&#x200B;并确认继续发布。

>[!NOTE]
>
>此过程可能需要一些时间，具体取决于数据库的大小和更改的复杂性。

### 创建导航条目 {#navigation}

发布自定义架构后，您可以在资源管理器中创建导航条目以访问自定义数据：

1. 导航到&#x200B;**[!UICONTROL 资源管理器]**&#x200B;菜单，然后选择要放置自定义架构的文件夹。
1. 单击省略号图标，然后单击&#x200B;**[!UICONTROL 新建文件夹]**。
   为自定义架构创建![导航条目](assets/schemas-publish3.png)
1. 添加标签并在&#x200B;**[!UICONTROL 文件夹类型]**&#x200B;字段中选择您的架构。
   为自定义架构创建![导航条目](assets/schemas-publish5.png)
1. 自定义架构现在可以从&#x200B;**[!UICONTROL 资源管理器]**&#x200B;视图中访问。

从新文件夹中，您可以：

* 查看自定义架构中的记录列表。
* 创建新记录。
* 编辑和删除现有记录。
* 自定义在列表视图中默认显示的列。
