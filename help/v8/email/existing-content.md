---
audience: end-user
title: 导入电子邮件内容
description: 了解如何导入电子邮件内容
exl-id: ef9c8e6f-f422-404e-9ebb-a89d1bd45e7f
badge: label="有限发布版"
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 48%

---

# 导入电子邮件内容 {#existing-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_import_content"
>title="使用现有的电子邮件内容"
>abstract="通过电子邮件设计器，可导入现有的 HTML 内容。此内容可以是内含样式表的 HTML 文件，也可以是具有 HTML 文件、样式表 (.css) 和图像的 .zip 文件夹。"

您可以在Email Designer中导入现有HTML内容。 相关的内容可以是：

* 一个带合并的样式表的 **HTML 文件**，
* 一个 **.zip 文件夹**，其中包含 HTML 文件、样式表 (.css) 和图像。

  >[!NOTE]
  >
  >具体的 .zip 文件结构没有任何限制。但是，引用必须是相对的，并且适合.zip文件夹的树结构。

要导入包含 HTML 内容的文件，请执行以下步骤：

1. 在 [电子邮件设计工具](get-started-email-designer.md) 主页，选择 **[!UICONTROL 导入HTML]**.

   ![](assets/html-import.png)

1. 拖放包含 HTML 内容的 HTML 或 .zip 文件，然后单击&#x200B;**[!UICONTROL 导入]**。

1. 上传HTML内容后，您的内容将位于 **[!UICONTROL 兼容模式]**.

   在此模式下，您只能对文本进行个性化，向内容添加链接或包含资源。

   ![](assets/html-imported.png)

1. 为了能够利用Email Designer内容组件，请访问 **[!UICONTROL HTML转换器]** 选项卡，然后单击 **[!UICONTROL 转换]**.

   ![](assets/html-imported-2.png)

   >[!NOTE]
   >
   > 使用 `<table>` 将标签作为HTML文件中的第一层可能会导致样式丢失，包括顶层标签中的背景和宽度设置。

1. 现在，您可以根据需要使用Email Designer功能个性化导入的文件 [了解详情](content-components.md).
