---
audience: end-user
title: 使用提取文件工作流活动
description: 了解如何使用提取文件工作流活动
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 7%

---

# 提取文件 {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="提取文件"
>abstract="此 **提取文件** 利用活动，可将数据以外部文件的形式从Adobe Campaign中导出。 然后，可以使用传输文件活动将数据导出到服务器位置，如SFTP、云存储或您的Campaign服务器。"

此 **提取文件** 活动是 **数据管理** 活动。 使用此活动以外部文件的形式从Adobe Campaign导出数据。 然后，可以使用传输文件活动将数据导出到服务器位置，如SFTP、云存储或您的Campaign服务器。

配置 **提取文件** 活动，添加 **提取文件** 将活动添加到工作流中，然后执行以下步骤。

## 配置要提取的文件 {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="要提取的文件"
>abstract="选择要提取的文件。"

此 **[!UICONTROL 要提取的文件]** 部分允许您配置要包含的文件属性和数据。

![](../assets/extract-file-file.png)

1. 在 **[!UICONTROL 文件名]** 字段中，为要提取的文件输入所需的名称。

   您可以使用事件变量、条件和日期/时间函数将文件名个性化。 要执行此操作，请单击 **[!UICONTROL 打开个性化对话框]** 图标以打开表达式编辑器。 [了解如何使用事件变量和表达式编辑器](../event-variables.md)

1. 指定要显示在提取文件中的列。 为此，请执行以下步骤：

   1. 单击 **[!UICONTROL 添加输出列]**.
   1. 选择要显示在列中的属性，然后进行确认。 可用属性取决于工作流的定向维度。
   1. 添加列后，您可以更改其 **[!UICONTROL 标签]** 并修改关联的 **[!UICONTROL 属性]**.
   1. 如果要将转换应用于列的值，请从下拉列表中选择它。 例如，可以将选定列中的所有值全部转换为大写。

1. 重复这些步骤以在提取文件中添加所需数量的列。 要更改列的位置，请使用向上箭头和向下箭头。

1. 要从提取的文件中删除所有重复行，请打开 **[!UICONTROL 删除重复行（列表）]** 选项。

1. 要根据属性对提取的文件进行排序，请打开 **[!UICONTROL 启用排序]** 选项，然后选择要对文件进行排序的属性，以及所需的排序方法（升序或降序）。 您可以对当前定向维度的任何属性进行排序，无论其是否已添加到文件的列中。

## 配置提取的文件格式 {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="目标格式"
>abstract="选择格式。"

此 **[!UICONTROL 目标]** 格式部分允许您配置提取文件的格式。

1. 选择 **[!UICONTROL 输出格式]** 对于提取的文件： **文本**， **文本使用fixed with columns**， **CSV (Excel)** 或 **XML**.

1. 单击 **[!UICONTROL 提取格式]** 按钮访问与所选格式相关的特定选项。 展开以下部分以获取更多信息。

+++ 可用的提取格式选项

   * **[!UICONTROL 使用第一行作为列标题]** (文本/CSV (Excel)格式)：打开此选项可将第一列用作标题。
   * **[!UICONTROL 列分隔符]** （文本格式）：指定在输出文件中用作列分隔符的字符。
   * **[!UICONTROL 字符串分隔符]** （文本格式）：指定如何在输出文件中分隔字符串。
   * **[!UICONTROL 行尾]** （文本格式）：指定输出文件中行尾的分隔方式。
   * **[!UICONTROL 编码]**：选择输出文件的编码。
   * **[!UICONTROL 日期格式和分隔符]**：指定日期在输出文件中的格式。
   * **[!UICONTROL 数字格式]**：指定数字在输出文件中的格式。
   * **[!UICONTROL 导出标签而不是枚举的内部值]**：如果导出枚举值并且希望检索列标签（而非内部ID），请打开此选项，这样更易于理解。

+++

   ![](../assets/extract-file-format.png)

## 添加后处理阶段 {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="后处理"
>abstract="定义后处理步骤"

此 **[!UICONTROL 导出修改脚本]** 允许您应用处理阶段以在数据提取期间执行，如压缩或加密。 要执行此操作，请单击 **[!UICONTROL 编辑脚本]** 按钮。

表达式编辑器将打开，允许您输入要应用于文件的命令。 左侧窗格提供了预定义的语法，您可以利用它来构建脚本。 [了解如何使用事件变量和表达式编辑器](../event-variables.md)

![](../assets/extract-file-script.png)

## 其他选项 {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="出站过渡"
>abstract="切换&#x200B;**“生成出站过渡”**&#x200B;选项，可在当前活动后添加出站过渡。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="流程错误"
>abstract="切换&#x200B;**“处理错误”**&#x200B;选项，可添加包含错误的出站过渡。"

配置输出文件提取后，可以使用与过渡和错误管理相关的其他选项：

* **[!UICONTROL 生成叫客过渡]**：启用此选项以添加叫客过渡并配置其标签。
* **[!UICONTROL 如果集客过渡为空，则不生成文件]**：启用此选项后，如果集客过渡不包含任何数据，则跳过文件提取。
* **[!UICONTROL 进程错误]**：启用此选项可在文件提取期间遇到任何错误时添加叫客过渡。

## 示例 {#example}

在以下示例中，我们使用 **构建受众** 活动后跟 **提取文件** 活动，将所有定向的用户档案提取到CSV文件中。

![](../assets/extract-file-example.png)

* 此 **[!UICONTROL 文件名]** 字段配置为包含提取日期。

  ![](../assets/extract-file-example-name.png)

* 将添加列以显示用户档案的名字和姓氏、其客户ID以及数据库中的创建日期。

  ![](../assets/extract-file-example-columns.png)
