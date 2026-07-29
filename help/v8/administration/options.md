---
title: 配置 [!DNL Campaign] 选项
description: 了解如何配置Campaign选项和创建自己的自定义选项。
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
TQID: https://experienceleague.adobe.com/a3MU21qEI7ggDv-gUT4--glIkWdU05mz14v3U9Q2wnM
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0638cc11f533521f7c8f3df3a80361b040a05b0c
workflow-type: tm+mt
source-wordcount: 592
ht-degree: 4%

---

# 配置[!DNL Campaign]选项 {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="选项"
>abstract="选项"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="创建选项"
>abstract="创建选项"

Adobe Campaign Web包括技术选项，可让您更具体地配置应用程序。 其中有些选项是内置的，而其他选项可以根据需要手动添加。

>[!IMPORTANT]
>内置选项已预配置，只应由高级用户修改。 如果您有任何问题或请求，请联系您的Adobe代表。

## 访问Campaign选项 {#access}

选项可从&#x200B;**[!UICONTROL 管理]** / **[!UICONTROL 选项]**&#x200B;菜单使用。 使用筛选器窗格缩小列表范围并快速找到所需的选项。

![](assets/options-list.png)\
[在“管理”/“选项”菜单中显示的选项列表]

>[!NOTE]
>尽管选项菜单在Adobe Campaign控制台和Web用户界面中的位置不同，但该列表是相同的，其操作方式与镜像类似。 有关可用选项的更多详细信息，请参阅[Campaign v7文档](https://experienceleague.adobe.com/zh-hans/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}中的选项列表。

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

## 限制投放的发件人电子邮件地址 {#restrict-sender-address}

默认情况下，营销人员可以在电子邮件投放的&#x200B;**[!UICONTROL 发件人电子邮件]**&#x200B;字段中键入任意地址。 若要将此字段限制为预定义的地址列表，请创建或编辑内置`NmsDelivery_senderAddressMask`选项，并将其值设置为允许的发件人地址逗号分隔列表，例如`abc@adobe.com,bcd@adobe.com`。

![在“从”菜单中限制值的选项](assets/option-restrict-from.png)

一旦此选项具有值，**[!UICONTROL 来自电子邮件]**&#x200B;字段就会成为仅包含这些地址的下拉列表，而不是自由文本字段。 如果选项不存在或其值为空，则字段将像之前一样保留自由文本。

电子邮件中的![可用值](assets/option-restrict-from2.png)

此限制是全局的。 它适用于每个品牌和投放模板，并且不支持个性化字段，仅支持静态地址。

有关&#x200B;**[!UICONTROL 来自电子邮件]**&#x200B;字段的更多信息，请参阅[配置电子邮件内容](../email/edit-content.md#edit-content)。
