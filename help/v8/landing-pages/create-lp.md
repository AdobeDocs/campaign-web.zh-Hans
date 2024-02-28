---
title: 创建登陆页面
description: 了解如何在Campaign Web中配置和发布登陆页面
feature: Landing Pages
source-git-commit: 2afb8c03305262c5695121fb03936c6d738833b5
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 22%

---

# 创建和发布登陆页面 {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="创建和管理登陆页面"
>abstract="借助 Adobe Campaign，您可以创建、设计和共享登陆页面，从而将用户引导至在线网页，您可以在其中根据内置模板管理客户获取、订阅/取消订阅和阻止列表用例。"

Campaign Web用户界面允许您创建、设计和发布登陆页面。 发布后，您可以在投放中插入指向表单的链接。 收件人单击该链接后，会被定向到相应的登陆页面。

[!DNL Adobe Campaign] 随附四个模板，用于管理以下用例： **acquisition**， **订阅**， **退订**、和 **阻止列表**. [了解详情](lp-use-cases.md)

## 访问登陆页面 {#access-landing-pages}

要访问登陆页面列表，请选择 **[!UICONTROL 营销活动管理]** > **[!UICONTROL 登陆页面]** 从左侧菜单。

![](assets/lp-inventory.png){zoomable=&quot;yes&quot;}

此 **[!UICONTROL 登陆页面]** 库存显示所有已创建的物料。 您可以使用以下代码筛选它们 **显示筛选器** 按钮。 您可以将结果限制为特定 [文件夹](../get-started/permissions.md#folders) 使用下拉列表，或者使用添加规则 [查询建模器](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png){zoomable=&quot;yes&quot;}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>在Campaign Web用户界面中，无法显示或编辑从客户端控制台（Web窗体）创建的登陆页面。 在中了解详情 [Campaign控制台文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=zh-Hans){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

您可以复制或删除登陆页面。 单击登陆页面旁边的省略号以选择所需的操作。

## 创建登陆页面 {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="定义登陆页面属性"
>abstract="填写标签等属性字段并根据需要修改架构。此外，还可编辑内部名称、更改从中存储登陆页面的文件夹和提供描述。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="定义每个页面的内容"
>abstract="调整作为该登陆页面一部分的每个页面的内容，例如表单本身、提交表单时显示的确认页面或发生错误时将用户定向到的页面。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="安排您的登陆页面"
>abstract="可定义登陆页面的开始日期和结束日期。当页面的有效期结束时，该表单将不再可用。而将显示&#x200B;**过期**&#x200B;页面。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_preload"
>title="定义预加载选项"
>abstract="当 **使用表单中引用的数据预填充** 选项，如果登陆页面的访客与数据库中的某个配置文件匹配，则该配置文件的信息会自动预加载到表单中。 使用 **如果没有ID，则跳过预加载** 选中此选项后，输入的每个用户档案都将在批准表单后添加到数据库中。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_storage"
>title="定义存储选项"
>abstract="通过预加载部分，可指示如何在数据库中查找要更新的记录。"

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

要创建登陆页面，请执行以下步骤：

1. 从 **[!UICONTROL 登陆页面]** 库存，单击 **[!UICONTROL 创建登陆页面]**.

   ![](assets/lp-create-button.png){zoomable=&quot;yes&quot;}

1. 选择模板：
   * **[!UICONTROL 客户获取]**：这是登陆页面的默认模板，允许您捕获和更新用户档案数据。
   * **[!UICONTROL 订阅]**：使用此模板可让用户订阅特定的 [服务](../audience/manage-services.md).
   * **[!UICONTROL 退订]**：此模板可用于发送给服务订阅者的投放，以便他们取消订阅 [服务](../audience/manage-services.md).
   * **[!UICONTROL 阻止列表]**：当用户档案单击投放中的选择退出链接时，并且不想再被联系时，应使用此模板。

   ![](assets/lp-templates.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >了解如何在中实施与每个模板对应的不同用例 [此页面](lp-use-cases.md).

1. 单击 **[!UICONTROL 创建]**.

1. 填写 **[!UICONTROL 属性]** 字段，例如标签。

   默认情况下，登陆页面存储在 **[!UICONTROL Web应用程序]** 文件夹。 您可以通过浏览到中所需的位置来更改它 **[!UICONTROL 其他选项]**. [了解如何使用文件夹](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png){zoomable=&quot;yes&quot;}

1. 在 **[!UICONTROL 数据预加载]** 部分，默认情况下会选中以下两个选项：

   * 当 **[!UICONTROL 使用表单中引用的数据预填充]** 选项，如果登陆页面的访客与数据库中的某个配置文件匹配，则该配置文件的信息会自动预加载到表单中。 用户只需填写缺少的字段，并在需要时更新现有值。 这允许合并现有用户档案的数据，而不是创建重复项。

   * 此 **[!UICONTROL 如果没有ID，则跳过预加载]** 如果不希望更新用户档案，则必须选择选项。 在这种情况下，输入的每个用户档案都将在批准表单后添加到数据库中。 例如，当表单在网站上发布时，将使用此选项。

1. 登陆页面可以具有后续页面。 要添加页面，请浏览 **[!UICONTROL 页面]** 部分，然后单击 **[!UICONTROL 编辑内容]** 按钮来指定您要为此登陆页面设计的每个页面。 每个页面的内容均已预填充。 根据需要编辑它们。 [了解详情](lp-content.md)

   ![](assets/lp-pages.png){zoomable=&quot;yes&quot;}

1. 此 **[!UICONTROL 更新预加载的记录]** 默认情况下选中该选项。 它允许通过登陆页面更新存储在数据库中的用户档案。 通过预加载框，您可以指示如何在数据库中查找要更新的记录。

   您还可以从登陆页面当前上下文中的字段中进行选择，这些字段将用于查找数据库中的相应用户档案。 要执行此操作，请取消选择 **[!UICONTROL 更新预加载的记录]** 选项并选中下的所需字段 **[!UICONTROL 对帐选项]**.

   ![](assets/lp-storage.png){zoomable=&quot;yes&quot;}

1. 可定义登陆页面的开始日期和结束日期。选择 **[!UICONTROL 启用计划]** 并设置日期。

   ![](assets/lp-schedule.png){zoomable=&quot;yes&quot;}

   * 登陆页面会在指定的开始日期/时间自动发布。

     >[!NOTE]
     >
     >如果未定义开始日期，则登陆页面在发布后立即处于活动状态。

   * 当页面到达结束日期时， <!--the landing page is automatically unpublished and -->该表单不再可用。 而将显示&#x200B;**[!UICONTROL 过期]**&#x200B;页面。

     >[!NOTE]
     >
     >出于安全原因和平台性能的考虑，Adobe建议您设置结束日期。

1. 单击 **[!UICONTROL 审阅并发布]**.

定义所有设置和 [设计](lp-content.md) 您可以 [测试](#test-landing-page) 和 [发布](#publish-landing-page) 您的登陆页面，如下所述。

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
>您必须具有可用的测试用户档案，才能预览消息并发送校样。 [了解有关测试用户档案的更多信息](../audience/test-profiles.md)

要测试登陆页面，请执行以下步骤：

1. 单击之后 **[!UICONTROL 审阅并发布]**，选择 **[!UICONTROL 模拟内容]** 登录页面仪表板中用于访问测试用户档案选择的按钮。

   ![](assets/lp-simulate-content.png){zoomable=&quot;yes&quot;}

1. 从 **[!UICONTROL 模拟]** 屏幕中，选择一个或多个测试用户档案。

   选择测试用户档案的步骤与测试消息时的步骤相同。 有关详情，请参见 [预览和测试](../preview-test/preview-test.md) 部分。

1. 选择 **[!UICONTROL 打开预览]** 以测试您的登陆页面。

   ![](assets/lp-open-preview.png){zoomable=&quot;yes&quot;}

1. 登陆页面的预览将在新选项卡中打开。 个性化的元素将由选定的测试配置文件数据替换。

   如果您选择了 **[!UICONTROL 使用表单中引用的数据预填充]** 选项，则表单字段会自动预填相应的测试配置文件数据。<!--TBC-->

   ![](assets/lp-preview.png){zoomable=&quot;yes&quot;}

1. 选择其他测试用户档案以预览登陆页面每个变体的渲染。

<!--Can you preview Confirmation/Error/Expiration pages?-->

## 发布登陆页面 {#publish-landing-page}

准备就绪并验证登陆页面后，将其发布，以便使用相应的按钮将其用于投放。

发布后：

* 登陆页面将添加到登陆页面列表中， **[!UICONTROL 已发布]** 状态。 它现已上线，并准备好在您的内容中引用。

* 您可以复制并粘贴 **[!UICONTROL 登陆页面URL]** ，该页面顶部显示的内容将置于Web浏览器中，以预览您的登陆页面。

>[!CAUTION]
>
>要全面测试或利用您的登陆页面，您无法将此链接直接复制并粘贴到 Web 浏览器或您的投放中。请改用 [模拟内容](#test-landing-page) 函数进行测试，并遵循中所述的步骤 [本节](lp-use-cases.md) 以正确使用登陆页面。

![](assets/lp-published.png){zoomable=&quot;yes&quot;}

您可以通过日志监控登陆页面影响<!--and specific reports-->. 单击 **[!UICONTROL 日志]** 按钮。
