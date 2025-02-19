---
audience: end-user
title: 使用业务规则（类型）
description: 了解如何使用分类和分类规则来控制、筛选和监控投放的发送。
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 22%

---

# 使用业务规则（类型） {#typologies}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="业务规则"
>abstract="现在，您可以在Adobe Campaign Web用户界面中创建分类和分类规则。 通过分类，您可以控制、过滤投放投放并设置其优先级。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"


>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="类型和类型规则"
>abstract="使用类型，您可以将所有投放中的业务实践标准化。类型是类型规则集合，可让您控制和筛选投放的发送并确定其优先级。在准备阶段，将从投放受众中排除符合类型规则中的条件的轮廓。"

## 关于分类

使用类型，您可以将所有投放中的业务实践标准化。**分类**&#x200B;是&#x200B;**分类规则**&#x200B;的集合，可让您控制、筛选投放并为其设置优先级。 在准备阶段，将从投放受众中排除符合类型规则中的条件的轮廓。

类型可确保投放始终包含某些元素（如退订链接或主题行）或用于从预期目标中排除分组（如取消订阅者、竞争对手或不忠诚客户）的筛选规则。

可通过&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL 业务规则]**&#x200B;菜单访问分类。 在此屏幕中，您可以访问所有现有的分类和分类规则，或根据需要创建新分类和分类规则。

![](assets/business-rules-list.png)

>[!NOTE]
>
>**[!UICONTROL 类型规则]**&#x200B;列表显示了迄今为止在Web用户界面或客户端控制台中创建的所有现有规则。 但是，在Web用户界面中只能创建&#x200B;**控件**&#x200B;和&#x200B;**筛选**&#x200B;规则。 要创建其他类型的分类规则（如压力或容量规则），请使用Campaign v8客户端控制台。 [了解如何在客户端控制台中创建类型规则](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

将分类应用于消息的主要步骤如下：

1. [创建分类](#typology)。
1. [创建类型规则](#typology-rules)。
1. [在分类](#add-rules)中引用分类规则。
1. [将分类应用于消息](#message)。

## 创建一个类型 {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="类型属性"
>abstract="定义类型的属性，并展开&#x200B;**[!UICONTROL 附加选项]**&#x200B;部分以访问高级设置。使用 **[!UICONTROL IP 关联]**&#x200B;字段将 IP 关联与类型关联起来。通过定义可以为每个关联使用哪些特定的 IP 地址，您可以更好地控制出站 SMTP 流量。"

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="IP 关联"
>abstract="通过管理与 IP 地址的关联，可以根据投放操作的类型将不同的 IP 地址与每种类型的流量关联起来，从而更好地控制传出的 SMTP 流量"

要创建分类，请执行以下步骤：

1. 导航到&#x200B;**[!UICONTROL 业务规则]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 类型]**&#x200B;选项卡。

1. 单击&#x200B;**[!UICONTROL 创建分类]**&#x200B;按钮并输入该分类的&#x200B;**[!UICONTROL 标签]**。

1. 展开&#x200B;**[!UICONTROL 其他选项]**&#x200B;部分以定义高级设置，如分类的内部名称、存储文件夹和描述。

   ![](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >**[!UICONTROL IP相关性]**&#x200B;字段允许您将IP相关性与类型相关联。 这样，您可以通过定义每个关联可以使用哪些特定IP地址，更好地控制出站SMTP流量。  例如，您可以为每个国家/地区或子域使用一个关联。 然后，您可以为每个国家/地区创建一个分类，并将每个关联关联关联关联关联到相应的分类。

1. 单击&#x200B;**[!UICONTROL 创建]**&#x200B;以确认创建分类。

分类会打开详细信息。 在此屏幕中，您可以直接引用现有分类规则。 您还可以创建新的分类规则，并稍后在分类中引用它们：
* [了解如何创建分类规则](#add-rules)
* [了解如何在类型中引用规则](#add-rules)

## 创建一个类型规则 {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="类型规则属性"
>abstract="定义类型规则的属性。**控制** 规则用于在发送前验证消息的质量和有效性，而&#x200B;**筛选** 规则会根据特定标准排除某些目标受众区段。<br/><br/>您还可以更改规则的执行顺序，以管理在同一个消息处理阶段中执行同一类型的多条规则时执行类型规则的顺序。"

要创建分类规则，请导航到&#x200B;**[!UICONTROL 业务规则]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 分类规则]**&#x200B;选项卡。

单击&#x200B;**[!UICONTROL 创建分类规则]**&#x200B;按钮，然后执行下面详述的步骤。

### 定义分类规则的属性 {#properties}

定义分类规则的属性：

1. 输入规则的&#x200B;**[!UICONTROL 标签]**。

   ![](assets/business-rules-control-rule.png)

1. 选择分类规则的&#x200B;**[!UICONTROL 类型]**：

   * **控制**：确保消息质量和有效性以及预发送（例如，字符显示、SMS长度、地址格式、URL缩短）。 它们使用脚本界面创建，以便为内容检查和修改定义复杂的逻辑。

   * **筛选** 规则根据特定标准（例如年龄、地区、国家、电话号码）排除某些目标受众区段。这些规则链接到定向维度。

   >[!NOTE]
   >
   >目前，只能从Web用户界面创建&#x200B;**控件**&#x200B;和&#x200B;**筛选**&#x200B;分类规则。 要创建其他类型的规则，请使用客户端控制台。 [了解如何在客户端控制台中创建类型规则](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. 选择要与规则关联的&#x200B;**[!UICONTROL 渠道]**。

1. 如果您不希望规则在创建后立即处于活动状态，请关闭&#x200B;**[!UICONTROL 活动]**&#x200B;选项。

1. 定义规则&#x200B;**[!UICONTROL 执行顺序]**。

   默认情况下，分类规则顺序设置为50。 您可以调整此值，以便管理在同一消息处理阶段执行同一类型的多个规则时，执行分类规则的顺序。 例如，执行顺序为20的筛选规则在执行顺序为30的筛选规则之前执行。

1. 展开&#x200B;**[!UICONTROL 其他选项]**&#x200B;部分以访问高级设置，如规则的内部名称、文件夹存储和描述。

1. 对于控制规则，其他选项中还提供了两个其他规则。 它们允许您指定应用规则的时间及其警报级别：

   * **[!UICONTROL 阶段]**：此字段允许您指定在投放生命周期的哪个时间点应用规则。 选择要在&#x200B;**[!UICONTROL 阶段]**&#x200B;下拉列表中选择的值。 展开以下部分，了解有关可能值的更多详细信息。

   +++控制规则阶段：

   **[!UICONTROL 在定位开始时]**：若要防止在发生错误时执行个性化步骤，可以在此处应用控制规则。

   **[!UICONTROL 定位后]**：如果您需要知道目标的卷以应用控制规则，请选择此阶段。 例如，检查验证大小控制规则将在每个定位阶段后应用：如果验证收件人过多，此规则将阻止消息个性化。

   **[!UICONTROL 在个性化开始时]**：如果控件涉及审批消息个性化，则必须选择此阶段。 在分析阶段执行消息个性化。

   **[!UICONTROL 在分析结束时]**：如果某项检查要求完成邮件个性化，请选择此阶段。

+++

   * **[!UICONTROL 级别]**：此选项允许您指定规则的警报级别。 展开以下部分以获取更多信息。

   +++控制规则级别：

   **[!UICONTROL 错误]**：停止邮件准备。

   **[!UICONTROL 警告]**：在准备日志中显示警告。

   **[!UICONTROL 信息]**：在准备日志中显示信息。

   <!--**[!UICONTROL Status]**:-->

   **[!UICONTROL 详细]**：在服务器日志中显示信息。

+++

### 构建规则内容 {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="筛选"
>abstract="**筛选** 规则根据特定标准（例如年龄、地区、国家、电话号码）排除某些目标受众区段。选择类型规则的目标维度，然后点击&#x200B;**[!UICONTROL 添加规则]** 按钮，以访问查询建模器并构建规则。"

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="代码"
>abstract="**控制** 规则在消息发送前验证消息的质量和有效性（例如字符显示、SMS 长度、地址格式、URL 缩短情况）。它们使用 JavaScript 代码创建。"

定义分类规则的属性后，即可构建规则的内容。

* 对于&#x200B;**控制规则**，请单击&#x200B;**编辑代码**&#x200B;按钮，然后使用JavaScript输入规则的逻辑。 在以下示例中，我们将创建一个规则，以在目标为空时在日志中显示警告。

  ![](assets/business-rules-code.png)

* 对于&#x200B;**筛选规则**，选择定向维度并单击&#x200B;**[!UICONTROL 添加规则]**&#x200B;按钮以使用[查询建模器](../query/query-modeler-overview.md)定义筛选条件。

  ![](assets/business-rules-query.png)

规则就绪后，单击&#x200B;**[!UICONTROL 创建]**&#x200B;按钮以创建分类规则。 现在，您可以在分类中引用规则，以将其应用于消息。

## 引用分类中的分类规则 {#add-rules}

要在分类中引用一个或多个规则，请执行以下步骤：

1. 导航到&#x200B;**[!UICONTROL 分类]**&#x200B;选项卡，并打开要引用规则的分类。

1. 选择&#x200B;**[!UICONTROL 分类规则]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 添加分类规则]**&#x200B;按钮。

   ![](assets/business-rules-reference.png)

1. 选择要与分类关联的一个或多个分类规则并进行确认。

   ![](assets/business-rules-typology-save.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

您现在可以将分类应用于消息。 完成后，将执行所有选定的分类规则以执行定义的检查。

## 将类型应用于消息 {#message}

要将分类应用于消息或消息模板，您需要将分类选择到消息设置中。 [了解如何配置投放设置](../advanced-settings/delivery-settings.md#typology)

![](assets/business-rules-apply.png)

完成后，执行分类中包含的分类规则，以在消息准备期间检查投放的有效性。 然后，会从投放受众中排除与分类规则中标准匹配的用户档案。
