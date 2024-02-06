---
title: 创建登陆页面
description: 了解如何在Campaign Web中配置和发布登陆页面
badge: label="有限发布版"
source-git-commit: 7635ab284900c8a4cd5ceca5675e57dbedb39f3a
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 23%

---

# 创建和发布登陆页面 {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="创建和管理登陆页面"
>abstract="Adobe Campaign允许您创建、设计和共享登陆页面，以将用户定向到在线网页，在这里，您可以根据内置模板管理客户获取、订阅/退订和阻止列表用例。"

Adobe Campaign允许您创建、设计和共享登陆页面，以将用户定向到在线网页，在这里，您可以根据内置模板管理客户获取、订阅/退订和阻止列表用例。

## 访问登陆页面 {#access-landing-pages}

要访问登陆页面列表，请选择 **[!UICONTROL 营销活动管理]** > **[!UICONTROL 登陆页面]** 从左侧菜单。

![](assets/lp-inventory.png)

此 **[!UICONTROL 登陆页面]** 库存显示所有已创建的物料。 您可以使用以下代码筛选它们 **显示筛选器** 按钮。 您可以将结果限制为特定 [文件夹](../get-started/permissions.md#folders) 使用下拉列表，或者使用添加规则 [查询建模器](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>在Campaign Web中，您无法显示或编辑从客户端控制台创建的登陆页面。 在中了解详情 [Campaign控制台文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

您可以复制或删除登陆页面。 单击登陆页面旁边的三个圆点，以选择所需的操作。

## 创建登陆页面 {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="定义登陆页面属性"
>abstract="填写标签等属性字段并根据需要修改架构。此外，还可编辑内部名称、更改从中存储登陆页面的文件夹和提供描述。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="定义页面的内容"
>abstract="编辑属于此登陆页面的每个页面的内容。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="安排您的登陆页面"
>abstract="可定义登陆页面的开始日期和结束日期。在页面到期时，将显示&#x200B;**到期**&#x200B;页面。"


>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="定义主页面设置"
>abstract="当用户比如从电子邮件或网站单击您的登陆页面的链接后，将立即向用户显示主页面。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="设置您的订阅登陆页面"
>abstract="通过订阅页面，您的客户可订阅服务。"

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. 从 **[!UICONTROL 登陆页面]** 库存，单击 **[!UICONTROL 创建登陆页面]**.

   ![](assets/lp-create-button.png)

1. 选择模板：
   * **[!UICONTROL 客户获取]**：这是登陆页面的默认模板，用于捕获和更新用户档案数据。
   * **[!UICONTROL 订阅]**：使用此模板提供服务订阅。
   * **[!UICONTROL 退订]**：此模板可从发送给订阅者的电子邮件链接到服务，以便他们退订此服务。
   * **[!UICONTROL 阻止列表]**：当某个用户档案不再希望Campaign与其联系时，应使用此模板。 了解有关阻止列表管理的更多信息

   ![](assets/lp-templates.png)

1. 单击 **[!UICONTROL 创建]**.

1. 填写属性字段，如标签。 默认情况下，登陆页面存储在 **[!UICONTROL Web应用程序]** 文件夹。 您可以通过浏览到中所需的位置来更改它 **[!UICONTROL 其他选项]**. [了解如何使用文件夹](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. 在 **[!UICONTROL 数据预加载]** 部分，默认情况下会选中以下两个选项：

   * 此 **[!UICONTROL 使用表单中引用的数据预填充]** 选项允许您自动预加载与表单中的输入和合并字段匹配的数据。

   * 此 **[!UICONTROL 如果没有ID，则跳过预加载]** 如果不希望更新用户档案，则必须选择选项。 在这种情况下，输入的每个用户档案都将在批准表单后添加到数据库中。 例如，当表单在网站上发布时，将使用此选项。

1. 在 **[!UICONTROL 页面]** 部分，单击 **[!UICONTROL 编辑内容]** 按钮来指定您要为此登陆页面设计的每个页面。 每个页面的内容均已预填充。 根据需要编辑它们。 [了解详情](lp-content.md)

   ![](assets/lp-pages.png)

1. 此 **[!UICONTROL 更新预加载的记录]** 默认情况下选中该选项。 如果您希望通过登陆页更新存储在数据库中的用户档案，则可以使用预加载框。 通过预加载框，您可以指示如何在数据库中查找要更新的记录。 您还可以从登陆页面当前上下文中的字段中进行选择，这些字段将用于查找数据库中的相应用户档案。

   ![](assets/lp-storage-schedule.png)

1. 可定义登陆页面的开始日期和结束日期。选择 **[!UICONTROL 启用计划]** 并设置日期。 在页面到期时，将显示&#x200B;**[!UICONTROL 到期]**&#x200B;页面。

1. 单击 **[!UICONTROL 审阅并发布]**.

配置和设计所有页面后，您可以 [测试](#test-landing-page) 和 [发布](#publish-landing-page) 您的登陆页面。

## 测试登陆页面 {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="模拟您的登陆页面"
>abstract="可在 Campaign Web 用户界面中查看登陆页面的预览，或在新的 Web 浏览器标签页中打开它。"

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="预览和测试登陆页面"
>abstract="定义了登陆页面设置和内容之后，您可使用测试配置文件对其进行预览。"

定义登陆页面设置和内容后，您可以使用测试配置文件进行预览。 如果您已插入 [个性化内容](../personalization/gs-personalization.md)，您将能够使用测试用户档案数据检查此内容在登陆页面中的显示方式。

>[!CAUTION]
>
>您必须具有可用的测试用户档案，才能预览消息并发送校样。 了解如何 [创建测试用户档案](../audience/test-profiles.md).

1. 在登陆页面界面中，单击 **[!UICONTROL 模拟内容]** 按钮以访问选择的测试用户档案。

   ![](assets/lp-simulate-content.png)

1. 从 **[!UICONTROL 模拟]** 屏幕中，选择一个或多个测试用户档案。

   选择测试用户档案的步骤与测试消息时的步骤相同。 有关详情，请参见 [预览和测试](../preview-test/preview-test.md) 部分。

1. 选择 **[!UICONTROL 打开预览]** 以测试您的登陆页面。

   ![](assets/lp-open-preview.png)

1. 登陆页面的预览将在新选项卡中打开。 个性化的元素将由选定的测试配置文件数据替换。

   ![](assets/lp-preview.png)

1. 选择其他测试用户档案以预览登陆页面每个变体的渲染。

<!--Can you preview Confirmation/Error/Expiration pages?-->

## 发布登陆页面 {#publish-landing-page}

准备登陆页面后，即可发布该页面，以供在消息中使用。

发布登陆页面后，该页面将添加到登陆页面列表，其中包含 **[!UICONTROL 已发布]** 状态。 现在已上线并可供使用。

![](assets/lp-published.png)

发布后，您可以复制并粘贴 **[!UICONTROL 登陆页面URL]** 页面顶部显示的URL库文件会发送到Web浏览器。

您可以通过日志和特定报告监控登陆页面影响。
