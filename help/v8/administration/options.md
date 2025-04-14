---
title: 配置 [!DNL Campaign] 选项
description: 了解如何配置Campaign选项和创建自己的自定义选项。
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 4%

---

# 配置[!DNL Campaign]选项 {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Options"
>abstract="Options"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Create option"
>abstract="Create option"

Adobe Campaign Web包括技术选项，可让您更具体地配置应用程序。 其中有些选项是内置的，而其他选项可以根据需要手动添加。

>[!IMPORTANT]\
内置选项已预配置，只应由高级用户修改。 如果您有任何问题或请求，请联系您的Adobe代表。

## 访问Campaign选项 {#access}

选项可从&#x200B;**[!UICONTROL 管理]** / **[!UICONTROL 选项]**&#x200B;菜单使用。 使用筛选器窗格缩小列表范围并快速找到所需的选项。

![](assets/options-list.png)\
[在“管理”/“选项”菜单中显示的选项列表]

>[!NOTE]\
尽管选项菜单在Adobe Campaign控制台和Web用户界面中的位置不同，但该列表是相同的，其操作方式与镜像类似。 有关可用选项的更多详细信息，请参阅[Campaign v7文档](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}中的选项列表。

从选项列表中，您可以：

* **复制或删除选项**：单击省略号按钮并选择所需的操作。
* **修改选项**：单击该选项名称以打开其属性。 进行更改并保存。
* **创建自定义选项**：单击&#x200B;**[!UICONTROL 创建选项]**&#x200B;按钮。

## 创建选项 {#create}

Adobe Campaign Web用户界面允许您创建自定义选项以满足要求。 在使用 **[!UICONTROL JavaScript 代码]**&#x200B;工作流活动存储中间数据时，这一点特别有用。

要创建选项，请执行以下操作：

1. 访问选项列表，然后单击&#x200B;**[!UICONTROL 创建选项]**。
1. 输入选项的名称，选择其类型，然后设置所需的值。
1. 单击&#x200B;**[!UICONTROL 创建]**&#x200B;以创建该选项。

![创建选项界面，显示名称、类型和值的字段](assets/options-create.png)

选项可以充当数据的临时存储，具有以下优势：

* 键入的值：选项支持特定数据类型，例如日期、整数、字符串等。
* 灵活性：利用选项，用户可以高效地存储和检索数据，而不会产生管理数据库表的开销。

在下面的示例中，创建了名为`sampleOption`的自定义选项，其初始值为“a”。 工作流中的&#x200B;**[!UICONTROL JavaScript代码]**&#x200B;活动修改此选项的值并将其存储在变量中。 更新的值将显示在工作流日志中，并反映在&#x200B;**[!UICONTROL 选项]**&#x200B;菜单中。

1. 创建选项。

   ![自定义选项创建界面，显示名称`sampleOption`和初始值“a”](assets/options-sample-create.png)

1. 配置&#x200B;**[!UICONTROL JavaScript代码]**&#x200B;活动并启动工作流。

   ![JavaScript代码活动配置界面](assets/options-sample-javascript.png)

1. 运行工作流以在工作流日志中查看更新的值。

   ![显示自定义选项更新值的工作流日志](assets/options-sample-logs.png)

1. 更新后的值现在显示在&#x200B;**[!UICONTROL 选项]**&#x200B;菜单中。

   ![显示自定义选项更新值的选项菜单](assets/options-sample-updated.png)