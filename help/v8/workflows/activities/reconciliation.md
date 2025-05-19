---
audience: end-user
title: 使用协调工作流活动
description: 了解如何使用协调工作流活动
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 40%

---

# 协调 {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="协调活动"
>abstract="**协调**&#x200B;活动是一项&#x200B;**定位**&#x200B;活动，通过它可定义 Adobe Campaign 数据库中的数据与工作表中的数据之间的联系。例如，可将&#x200B;**协调**&#x200B;活动放在&#x200B;**加载文件**&#x200B;活动之后以将非标准数据导入到数据库中。在本例中，**协调**&#x200B;活动定义了 Adobe Campaign 数据库中的数据与外部表中的数据之间的关联。"

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

**协调**&#x200B;活动是一个&#x200B;**定位**&#x200B;活动，它定义了Adobe Campaign数据库中的数据与工作表中的数据（如从外部文件加载的数据）之间的链接。

例如，可将&#x200B;**协调**&#x200B;活动放在&#x200B;**加载文件**&#x200B;活动之后以将非标准数据导入到数据库中。在这种情况下，**协调**&#x200B;活动定义Adobe Campaign数据库中的数据与工作表中的数据之间的链接。

## 最佳实践 {#reconciliation-best-practices}

当&#x200B;**扩充**&#x200B;活动定义要在工作流中处理的附加数据（例如，组合来自多个集的数据或创建指向临时资源的链接）时，**协调**&#x200B;活动将未识别的数据链接到现有资源。

>[!NOTE]
>协调操作要求链接维度的数据已存在于数据库中。 例如，如果导入一个购买文件，其中显示了购买哪个产品、购买时间以及购买客户，则数据库中必须已存在该产品和该客户。

## 配置协调活动 {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="定位维度"
>abstract="选择新的定位维度。维度定义了目标群体：收件人、应用程序订阅者、运营商、订阅者等。默认情况下会选择当前的定位维度。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="协调规则"
>abstract="选择用于删除重复项的协调规则。若要使用属性，请选择&#x200B;**简单属性**&#x200B;选项，然后选择源字段和目标字段。若要使用查询建模器创建您自己的协调条件，请选择&#x200B;**高级协调条件**&#x200B;选项。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/query-database/query-modeler-overview" text="使用查询建模器"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="选择定位维度"
>abstract="选择要协调的入站数据的定位维度。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?#targeting-dimensions" text="目标选择维度"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="保留未协调数据"
>abstract="默认情况下，未协调的数据保留在出站过渡中，并可在工作表中使用。要删除未协调的数据，请停用&#x200B;**保留未协调的数据**&#x200B;选项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="协调属性"
>abstract="选择用于协调数据的属性，然后单击“确认”。"

按照以下步骤配置&#x200B;**协调**&#x200B;活动：

1. 将&#x200B;**协调**&#x200B;活动添加到您的工作流。 此活动应紧跟在包含定向维度并非直接来自Adobe Campaign的群体的过渡之后。

1. 选择新的定位维度。维度定义了目标群体：收件人、应用程序订阅者、运营商、订阅者等。[了解有关定向维度的更多信息](../../audience/about-recipients.md#targeting-dimensions)。

1. 选择要用于协调的字段。 您可以使用一个或多个协调标准。

   1. 要使用属性协调数据，请选择&#x200B;**简单属性**&#x200B;选项。 **Source**&#x200B;字段列出了输入转换中要协调的可用字段。 **目标**&#x200B;字段对应于所选定向维度的字段。 当源和目标相等时，将协调数据。 例如，选择&#x200B;**电子邮件**&#x200B;字段，以根据用户档案的电子邮件地址删除重复的用户档案。

      要添加另一个协调条件，请单击&#x200B;**添加规则**&#x200B;按钮。 如果指定了多个连接条件，则必须对所有连接条件进行验证，才能将数据链接在一起。

      ![协调条件示例](../assets/workflow-reconciliation-criteria.png)

   1. 要使用其他属性协调数据，请选择&#x200B;**高级协调条件**&#x200B;选项。 然后，您可以使用查询建模器创建自己的协调条件。 [了解如何使用查询建模器](../../query/query-modeler-overview.md)。

1. 使用&#x200B;**创建筛选器**&#x200B;按钮筛选要协调的数据。 这使您可以使用查询建模器创建自定义条件。 [了解如何使用查询建模器](../../query/query-modeler-overview.md)。

默认情况下，未协调的数据保留在出站过渡中，并可在工作表中使用。要删除未协调的数据，请停用&#x200B;**保留未协调的数据**&#x200B;选项。

## 示例 {#reconciliation-example}

下方的示例演示了直接从包含新客户的导入文件创建受众轮廓的工作流。包括以下活动：

工作流的设计如下所示：

![工作流示例](../assets/workflow-reconciliation-sample-1.0.png)

它是通过以下活动构建的：

* [加载文件](load-file.md)活动上传包含从外部工具提取的配置文件数据的文件。

  例如：

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* **协调**&#x200B;活动使用&#x200B;**电子邮件**&#x200B;和&#x200B;**出生日期**&#x200B;字段作为协调条件，将传入数据标识为用户档案。

  ![协调活动示例](../assets/workflow-reconciliation-sample-1.1.png)

* [保存受众](save-audience.md)活动根据这些更新创建新的受众。 如果不需要创建或更新特定受众，您还可以将&#x200B;**保存受众**&#x200B;活动替换为&#x200B;**结束**&#x200B;活动。 无论在何种情况下，运行工作流都会更新收件人用户档案。

## 兼容性 {#reconciliation-compat}

客户端控制台中不存在&#x200B;**协调**&#x200B;活动。 在启用了协调选项的客户端控制台中创建的所有&#x200B;**扩充**&#x200B;活动在Campaign Web用户界面中显示为&#x200B;**协调**&#x200B;活动。