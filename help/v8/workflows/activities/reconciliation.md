---
audience: end-user
title: 使用协调工作流活动
description: 了解如何使用协调工作流活动
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 43%

---

# 协调 {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="协调活动"
>abstract="**协调**&#x200B;活动是一项&#x200B;**定位**&#x200B;活动，通过它可定义 Adobe Campaign 数据库中的数据与工作表中的数据之间的联系。例如，可将&#x200B;**协调**&#x200B;活动放在&#x200B;**加载文件**&#x200B;活动之后以将非标准数据导入到数据库中。在本例中，**协调**&#x200B;活动允许您定义 Adobe Campaign 数据库中的数据与外部表中的数据之间的关联。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="协调选择字段"
>abstract="协调选择字段"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="协调创建条件"
>abstract="协调创建条件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="协调生成补集"
>abstract="协调生成补集"

此 **调解** 活动是 **定位** 活动，用于定义Adobe Campaign数据库中的数据与工作表中的数据（例如从外部文件加载的数据）之间的链接。

例如，可将&#x200B;**协调**&#x200B;活动放在&#x200B;**加载文件**&#x200B;活动之后以将非标准数据导入到数据库中。在本例中， **调解** 利用活动，可定义Adobe Campaign数据库中的数据与工作表中的数据之间的链接。

## 最佳实践 {#reconciliation-best-practices}

而 **扩充** 利用活动，可定义要在工作流中处理的附加数据(您可以使用 **扩充** 活动以组合来自多个集的数据，或创建指向临时资源的链接)， **调解** 利用活动，可将未识别的数据链接到现有资源。

>[!NOTE]
>协调操作意味着链接维度的数据已在数据库中。  例如，如果导入一个购买文件，其中显示了购买哪个产品、购买时间、购买客户等，则数据库中必然已经存在该产品和客户。

## 配置协调活动 {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="定位维度"
>abstract="选择新的定位维度。通过维度可以定义目标群体：收件人、应用程序订阅者、运营商、订阅者等。默认情况下会选择当前的定位维度。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="协调规则"
>abstract="选择用于删除重复项的协调字段。您可以使用一个或多个协调标准。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="选择定位维度"
>abstract="选择要协调的入站数据的定位维度。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=zh-Hans#targeting-dimensions" text="定位维度"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="保留未协调数据"
>abstract="默认情况下，未调节的数据保留在出站过渡中，并可在工作表中使用。要删除未协调的数据，请停用&#x200B;**保留未协调的数据**&#x200B;选项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="协调属性"
>abstract="选择用于协调数据的属性，然后单击“确认”。"

按照以下步骤配置 **调解** 活动：

1. 拖放 **调解** 活动添加到工作流中。 应在包含定向维度并非直接来自Adobe Campaign的群体的过渡之后添加此活动。

1. 选择新的定位维度。通过维度可以定义目标群体：收件人、应用程序订阅者、运营商、订阅者等。[了解有关定位维度的更多信息](../../audience/about-recipients.md#targeting-dimensions).

1. 选择要用于协调的字段。 您可以使用一个或多个协调标准。

   1. 要使用属性协调数据，请选择 **简单属性** 选项。 此 **来源** 字段列出了输入过渡中可用的要协调的字段。 此 **目标** 字段对应于所选定向维度的字段。 当源和目标相等时，将协调数据。 例如，选择 **电子邮件** 用于根据用户档案的电子邮件地址删除重复用户档案的字段。

      要添加其他协调条件，请单击 **添加规则** 按钮。 如果指定了多个连接条件，则必须对所有连接条件进行验证，以便将数据链接在一起。

      ![](../assets/workflow-reconciliation-criteria.png)

   1. 要使用其他属性协调数据，请选择 **高级协调条件** 选项。 然后，您可以使用查询建模器创建自己的协调条件。 了解如何在中使用查询建模器 [本节](../../query/query-modeler-overview.md).

1. 您可以使用来筛选要协调的数据 **创建过滤器** 按钮。 这让您能够使用创建自定义条件 [查询建模器](../../query/query-modeler-overview.md).

默认情况下，未协调的数据将保留在叫客过渡中，并可在工作表中供将来使用。 要删除未协调的数据，请停用&#x200B;**保留未协调的数据**&#x200B;选项。

## 示例 {#reconciliation-example}

下方的示例演示了直接从包含新客户的导入文件创建受众用户档案的工作流。该工作流由以下活动组成：

工作流的设计如下所示：

![](../assets/workflow-reconciliation-sample-1.0.png)


它是通过以下活动构建的：

* [加载文件](load-file.md)活动，上传包含从外部工具提取之用户档案数据的文件。

  例如：

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* A **调解** 使用将传入数据标识为用户档案的活动 **电子邮件** 和 **出生日期** 字段作为协调条件。

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* A [保存受众](save-audience.md) 活动，以根据这些更新创建新受众。 您也可以替换 **保存受众** 活动依据 **结束** 活动。 无论在何种情况下，运行工作流都会更新收件人用户档案。


## 兼容性 {#reconciliation-compat}

此 **调解** 客户端控制台中不存在活动。 全部 **扩充功能** 在启用了协调选项的客户端控制台中创建的活动显示为 **调解** Campaign Web用户界面中的活动。
