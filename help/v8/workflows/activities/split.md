---
audience: end-user
title: 使用“拆分工作流”活动
description: 了解如何使用“拆分工作流”活动
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 69%

---

# 拆分 {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="拆分活动"
>abstract="通过&#x200B;**拆分**&#x200B;活动，可根据不同的选择标准（如筛选规则或群体大小）将传入的群体分为多个子集。"

**拆分**&#x200B;活动是一个&#x200B;**定位**&#x200B;活动，它根据不同的选择条件（如筛选规则或群体大小）将传入的群体划分为多个子集。

## 配置拆分活动 {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="拆分活动的区段"
>abstract="添加所需数量的子集以划分传入的群体。执行&#x200B;**拆分**&#x200B;活动时，将群体按将其添加到活动的顺序划分为不同的子集。在开始工作流之前，请确保您已使用箭头按钮按照符合您需求的顺序为子集排序。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="“拆分”活动筛选条件"
>abstract="要将筛选条件应用于子集，请单击&#x200B;**[!UICONTROL 创建筛选条件]**&#x200B;并使用查询建模器配置所需的筛选规则。例如，包括其电子邮件地址位于数据库中的传入群体的轮廓。"
>additional-url="https://experienceleague.adobe.com/zh-hans/docs/campaign-web/v8/query-database/query-modeler-overview" text="使用查询建模器"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="拆分活动限制"
>abstract="要限制子集选择的轮廓数，请打开&#x200B;**[!UICONTROL 启用限制]**&#x200B;选项，并指定要包括的群体的数量或百分比。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="拆分活动排序"
>abstract="在为子集设置群体限制时，您可以根据特定的轮廓属性按升序或降序顺序对所选轮廓进行排名。为此，请打开&#x200B;**启用排序**&#x200B;选项。例如，您可以限制子集以仅包含购买金额最高的前 50 个轮廓。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="拆分生成补集"
>abstract="配置完所有子集后，您可以选择与任何子集均不匹配的剩余群体，并将其包含到附加出站过渡中。为此，请打开&#x200B;**生成补集**&#x200B;选项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="在同一个表中生成所有子集"
>abstract="切换该选项可将所有子集组合到单个输出过渡中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="跳过空过渡"
>abstract="如果传入的群体为空，则切换&#x200B;**[!UICONTROL 跳过空过渡]**&#x200B;选项，以禁用此子集的输出过渡。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="启用输出群体的重叠"
>abstract="**[!UICONTROL 启用输出群体重叠]**&#x200B;选项可让您管理属于多个子集的群体。如果不勾选该框，拆分活动将确保收件人即使满足多个子集的标准，也不会出现在多个输出过渡中。它们将位于符合条件的第一个选项卡的目标中。选中此框后，如果收件人符合筛选条件，则可以在多个子集中找到他们。Adobe Campaign 建议使用专属标准。"

请执行以下步骤来配置&#x200B;**拆分**&#x200B;活动：

1. 向您的工作流添加一个&#x200B;**拆分**&#x200B;活动。

1. 活动配置窗格随即打开，其中包含默认子集。单击&#x200B;**添加区段**&#x200B;按钮以添加所需数量的子集，对传入群体进行分段。

   ![显示子集的拆分活动配置窗格](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >执行&#x200B;**拆分**&#x200B;活动时，将群体按将其添加到活动的顺序划分为不同的子集。例如，如果第一个子集恢复初始群体的 70%，则下一个添加的子集仅将其选择标准应用于剩余的 30%，依此类推。
   >
   >在启动工作流之前，请确保已按照适合您需求的顺序对子集进行了排序。 使用箭头按钮更改子集的位置。

1. 添加子集后，活动将显示与子集一样多的输出转换。更改每个子集的标签以在工作流画布中轻松识别它们。

1. 配置每个子集如何过滤传入群体。 执行以下步骤：

   1. 打开子集以显示其属性。

   1. 要将筛选条件应用于子集，请单击&#x200B;**[!UICONTROL 创建筛选条件]**&#x200B;并使用查询建模器配置所需的筛选规则。例如，包含来自其电子邮件地址存在于数据库中的传入群体的用户档案。 [了解如何使用查询建模器](../../query/query-modeler-overview.md)。

   1. 要限制子集选择的轮廓数，请打开&#x200B;**[!UICONTROL 启用限制]**&#x200B;选项，并指定要包括的群体的数量或百分比。

   1. 要在传入群体为空时禁用过渡，请打开&#x200B;**[!UICONTROL 跳过空过渡]**&#x200B;选项。 如果没有与子集匹配的用户档案，则工作流将不会转换为下一个活动。

      ![子集配置窗格显示筛选和排序选项](../assets/workflow-split-subset.png)

      >[!NOTE]
      >
      >为子集设置群体限制时，您可以根据特定的[配置文件属性](../../get-started/attributes.md)，按升序或降序对选定的配置文件进行排名。 为此，请打开&#x200B;**[!UICONTROL 启用排序]**&#x200B;选项。例如，您可以限制子集以仅包含购买金额最高的前 50 个轮廓。

1. 配置完所有子集后，您可以选择与任何子集均不匹配的剩余群体，并将其包含到附加出站过渡中。为此，请打开&#x200B;**[!UICONTROL 生成补集]**&#x200B;选项。

   ![补充过渡配置窗格](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >**[!UICONTROL 在同一表]**&#x200B;中生成所有子集选项允许您将所有子集分组到单个输出转换中。

1. 通过&#x200B;**[!UICONTROL 启用输出群体的重叠]**&#x200B;选项，您可以管理属于多个子集的群体：

   * 如果不勾选该框，拆分活动将确保收件人即使满足多个子集的标准，也不会出现在多个输出过渡中。它们将位于第一个选项卡的目标中，并带有匹配条件。
   * 选中此框后，如果收件人符合筛选条件，则可以在多个子集中找到他们。Adobe Campaign 建议使用专属标准。

现已配置该活动。在执行工作流时，按照将群体区段添加到活动的顺序，将这些群体区段添加到不同的子集中。

## 示例 {#split-example}

在以下示例中，**[!UICONTROL 拆分]**&#x200B;活动根据要使用的通信渠道将受众分段为不同的子集：

* **子集1“推送”**：此子集包含已安装移动应用程序的所有配置文件。
* **子集2“短信”**：手机用户：对于未归入子集1的剩余群体，子集2应用筛选规则来选择数据库中包含手机的用户档案。
* **补集过渡**：此过渡捕获不符合子集 1 或子集 2 的条件的所有剩余轮廓。具体来说，它包括既没有安装移动应用程序也没有手机的轮廓，例如未安装移动应用程序或缺少注册的手机号码的用户。

![具有子集和补码转换的分割活动示例](../assets/workflow-split-example.png)