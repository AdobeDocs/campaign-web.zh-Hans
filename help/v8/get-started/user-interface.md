---
audience: end-user
title: 探索界面
description: Adobe Campaign Web 用户界面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: c2382359ee6777277fa9dd4f8fd4282fb2381b38
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 100%

---

# 探索界面 {#user-interface}

新的 Adobe Campaign Web 界面提供直观的现代用户体验，可简化营销活动的设计和投放。此新界面与 Adobe Experience Cloud 应用程序和解决方案集成。

[在本文中](connect-to-campaign.md)，了解如何连接到 Adobe Campaign 并探索有关 Experience Cloud 导航的基础知识。


>[!NOTE]
>
>此文档经常更新以反映产品用户界面中的最新更改。但是，某些屏幕快照可能与用户界面略有不同。

## Campaign 主页 {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="最近访问"
>abstract="**最近项目**&#x200B;列表提供了最近创建和修改的投放的快捷方式。此列表显示了它们的渠道、状态、所有者、创建日期和修改日期。"

通过 Campaign 主页，可快速轻松地浏览关键资源、指标和组件。

主页的上半部分详细介绍了产品中所提供的最新更新和新功能，以及发行说明和详细文档的链接。使用向左箭头滚动功能卡。

![](assets/home.png){zoomable=&quot;yes&quot;}

利用&#x200B;**关键绩效指标 (KPI)**，可以通过常见 KPI 检查平台有效性。可在[此页面](../reporting/kpis.md)中详细了解这些 KPI。

**最近**&#x200B;列表提供了最近创建和修改的投放的快捷方式。此列表显示了它们的渠道、状态、所有者、创建日期和修改日期。单击&#x200B;**显示更多**&#x200B;链接，加载更多投放。

此外，还可从页面的&#x200B;**学习**&#x200B;部分访问 Adobe Campaign Web 的关键帮助页面。

## 左侧导航菜单 {#user-interface-left-nav}

浏览左侧链接以访问 Adobe Campaign Web 功能。多个链接显示了可排序和筛选的对象的列表。您还可以配置列以显示所需的所有信息。请参阅此[部分](#list-screens)。某些列表屏幕为只读。左侧导航菜单和列表中显示的项目取决于您的用户权限。可在[此部分](permissions.md)中详细了解权限。


### 探索工具 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="**探索工具**&#x200B;菜单使用与客户端控制台中的文件夹层次结构相同的文件夹层次结构显示所有 Campaign 组件和对象。浏览您的所有 Campaign v8 组件、文件夹和架构，检查关联的权限，然后从此菜单创建文件夹和子文件夹。"

**资源管理器**&#x200B;菜单按照与客户端控制台中相同的文件夹层次结构显示所有 Campaign 资源和对象。浏览所有 Campaign v8 组件、文件夹和架构，并创建投放、工作流和营销活动。

**资源管理器**&#x200B;中显示的项目取决于您的用户权限。如果您具有适当的权限，也可以添加文件夹和子文件夹。可在[此部分](permissions.md)中详细了解权限。

可配置列以自定义显示，以便查看所需的所有信息。请参阅此[部分](#list-screens)。还可添加文件夹和子文件夹，如[此部分](permissions.md#folders)中所详述。

有关 Campaign 探索工具、文件夹层次结构和资源的更多信息，请参阅此 [Campaign v8（控制台）文档 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=zh-Hans#ac-explorer-ui){target="_blank"}。

### 营销活动管理 {#user-interface-campaign-management}

在“营销活动管理”部分中，可访问市场营销活动、投放情况和工作流。

* **营销活动** - 这是您的营销活动和营销活动模板的列表。默认情况下，可查看每个营销活动的开始/结束/创建/上次修改日期、当前状态以及创建它的 Campaign 操作员的姓名。可按状态、开始/结束日期和文件夹筛选该列表，也可创建高级筛选器以定义您自己的筛选条件。可[在此部分中](../campaigns/gs-campaigns.md)详细了解营销活动。

* **投放** - 浏览您的投放列表。默认情况下，您可以查看它们的状态、最后修改日期以及关键 KPI。您可以按状态、联系日期或渠道筛选列表。单击电子邮件投放以打开其仪表板来获取投放详细信息的概述。其他渠道上的投放是只读的。可[在此部分中](../msg/gs-messages.md)详细了解投放。

  使用&#x200B;**更多操作**&#x200B;按钮删除或重复投放。

  ![](assets/more-actions.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

* **工作流** - 可在此屏幕中访问工作流和工作流模板的完整列表。可检查其状态、上次/下次执行日期，并可创建新的工作流或新的工作流模板。可用与筛选其他对象相同的条件筛选该列表。此外，还可筛选属于或不属于营销活动的工作流。可[在此部分中](../workflows/gs-workflows.md)详细了解工作流。


### 内容管理 {#user-interface-content-management}

在“内容管理”部分中，您可以查看内容模板和片段。

* **内容模板** - 为了加快并改进设计流程，您可以创建独立的模板，从而轻松地在 [!DNL Adobe Campaign] 中重复使用自定义内容。此功能仅适用于电子邮件，它使以内容为导向的用户能够使用独立的模板，这样营销用户可以在自己的电子邮件营销活动中重复使用和调整模板。可在[此部分](../email/create-email-templates.md)中了解详情。

<!--
* **Fragments** -
-->

### 客户管理 {#user-interface-customer-management}

在“客户管理”部分，您可以查看用户档案、受众和订阅。这些列表为只读。

* **用户档案** - 创建和管理用户档案，并访问收件人数据库。默认情况下，您可以查看他们的电子邮件地址、名字和姓氏。可在[此部分](../audience/about-recipients.md)中详细了解用户档案。
* **受众** - 这是您的受众列表。默认情况下，您可以查看它们的类型、来源、创建/最后修改日期和标签。您可以按来源筛选列表。可在[此部分](../audience/about-recipients.md)中详细了解受众和列表。
* **订阅服务** - 浏览您的订阅列表。默认情况下，您可以查看它们的类型、模式和标签。请参阅 [Adobe Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=zh-Hans){target="_blank"}，了解如何管理订阅和退订。
* **预定义筛选器** - 预定义筛选器是创建并保存以供将来使用的自定义筛选器。在使用查询建模器进行任何过滤操作时，例如在过滤数据列表或创建投放受众时，可将预定义过滤器用作快捷方式。可在[此部分](predefined-filters.md)中了解详情。


### 决策管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="优惠"
>abstract="浏览在控制台中使用&#x200B;**交互**&#x200B;模块创建的优惠和优惠模板的列表。这些列表为只读。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=zh-Hans" text="将优惠添加到投放"

在“决策管理”部分中，您可以查看优惠和优惠模板。这些列表为只读。

* **优惠** - 浏览在控制台中使用&#x200B;**交互**&#x200B;模块创建的优惠和优惠模板的列表。默认情况下，您可以查看它们的状态、开始/结束日期和环境。您可以按状态和开始/结束日期筛选列表。还有优惠模板可用。

可在[此部分](../msg/offers.md)中了解如何在电子邮件和短信中创建和发送优惠。

### 报告 {#left-nav-reporting}

* **报告** - **报告**&#x200B;条目可提供 Campaign 环境中每个渠道的流量和参与量度的整体摘要。这些报告由各种构件组成，每个构件都提供您的营销活动或投放效果的一个独特视角。可在[此部分](../reporting/global-reports.md)中了解详情。


## 上下文帮助 {#user-interface-help}

界面中提供了上下文帮助。当 `?` 图标可用时，单击该图标可显示帮助信息和相关文档链接。

![](assets/do-not-localize/context-help.png){zoomable=&quot;yes&quot;}{width="40%" align="left"}

目前，**AI 支持的知识助手**&#x200B;在新 Campaign Web 用户界面中作为 Beta 版发布，嵌入在上下文帮助中，彻底改变了文档搜索和解答操作方法疑问的方式，可轻松地筛选大型文档存储库并立即找出所需的准确信息。

通过 Campaign 生成式 AI 的各项功能，此助手改变您的体验，使检索信息和解决问题变得轻而易举。无论您是在复杂的任务中寻求指导，还是在大量文档中导航，我们的基于 AI 的知识助手都是您的绝佳伙伴，每次互动的效率和准确性都无与伦比。

可在[此部分](using-ai.md)中了解详情。


## 了解详情 {#learn-more}

参阅[此页面](list-filters.md)，了解如何浏览、搜索和筛选 Campaign 环境中可用的列表。



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建区段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建区段。"

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全球报告发送"
>abstract="跟踪报告量度在此屏幕中可见"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全球报告跟踪"
>abstract="跟踪报告量度在此屏幕中可见"


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="收件人创建"
>abstract="收件人创建"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="收件人信息卡概述"
>abstract="收件人信息卡概述"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="收件人接触点"
>abstract="收件人接触点"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="收件人订阅选择"
>abstract="收件人订阅选择"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="收件人合格优惠列表"
>abstract="收件人合格优惠列表"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="收件人优惠预览"
>abstract="收件人优惠预览"

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="片段"
>abstract="片段"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="片段保存"
>abstract="片段保存"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="片段创建"
>abstract="片段创建"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="片段属性"
>abstract="片段属性"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="片段类型"
>abstract="片段类型"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="片段列表"
>abstract="片段列表"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="片段详情"
>abstract="片段详情"




>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="条件内容保存过滤器"
>abstract="条件内容保存过滤器"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="条件内容选择过滤器"
>abstract="条件内容选择过滤器"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="条件主题行上的内容"
>abstract="条件主题行上的内容"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="条件内容主题行条件"
>abstract="条件内容主题行条件"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="模拟测试配置文件"
>abstract="模拟测试配置文件"

<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="模拟测试配置文件选择"
>abstract="模拟测试配置文件选择"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="模拟测试配置文件发送"
>abstract="模拟测试配置文件发送"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="模拟电子邮件日志"
>abstract="模拟电子邮件日志"

<!-- ML: beta wiki page - not visible in UI-->

<!-- FOR POST-GA -->



<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="显示高级属性"
>abstract="默认情况下，属性列表中仅显示最常见属性。激活&#x200B;**显示高级属性**&#x200B;切换开关可看到对于规则生成器左侧调色板中当前列表可用的所有属性，如节点、分组、1 对 1 链接、1 对多链接。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="规则生成器高级字段"
>abstract="默认情况下，属性列表中仅显示最常见属性。激活&#x200B;**显示高级属性**&#x200B;切换开关可看到对于规则生成器左侧调色板中当前列表可用的所有属性，如节点、分组、1 对 1 链接、1 对多链接。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="规则生成器高级属性"
>abstract="默认情况下，属性列表中仅显示最常见属性。激活&#x200B;**显示高级属性**&#x200B;切换开关可看到对于规则生成器左侧调色板中当前列表可用的所有属性，如节点、分组、1 对 1 链接、1 对多链接。"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="此模板处于“仅就绪”状态"
>abstract="您无权编辑此模板。如果需要，请联系您的管理员以向您授予访问权限。"

<!-- Subscription activity-->

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="默认登陆页面"
>abstract="选择与此订阅服务相关的默认登陆页面。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="订阅服务活动"
>abstract="使用 Adobe Campaign 创建和监测您的服务（如新闻稿）以及检查这些服务的订阅或取消订阅情况。订阅仅适用于电子邮件和短信投放。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="订阅服务参数"
>abstract="选择并确认订阅服务的设置。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="订阅服务出站过渡"
>abstract="切换&#x200B;**“生成出站过渡”**&#x200B;选项，可在活动后添加过渡。"


<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="更新数据"
>abstract="**更新数据**&#x200B;活动会对数据库中的字段执行批量更新。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="选择如何更新数据"
>abstract="通过&#x200B;**操作类型**&#x200B;字段，您可以选择对数据库中的数据执行的处理过程。选择第一个选项来添加数据或更新（如果已经添加）。您还可以仅添加数据、仅更新数据或删除数据。选择&#x200B;**“更新和合并收藏集”**，即可选择要链接重复项的主要记录，然后安全地删除这些重复项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="记录标识"
>abstract="指定如何识别数据库中的记录：如果数据与现有定位维度相关，请选择&#x200B;**“使用定位维度”**&#x200B;选项，然后选择要更新的定位维度和字段。否则，请指定一个或多个自定义链接来识别数据库中的数据，或直接使用协调键。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="选择要更新的字段"
>abstract="选择要更新的字段和协调键设置。您可以使用&#x200B;**“自动映射”**&#x200B;选项来自动识别要更新的字段。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="更新数据的高级选项"
>abstract="通过&#x200B;**“高级选项”**&#x200B;分区，您可以指定其他设置以管理数据和重复项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="生成出站过渡"
>abstract="切换&#x200B;**“生成出站过渡”**&#x200B;选项即可添加出站过渡，该过渡会在&#x200B;**更新数据**&#x200B;活动执行结束时激活。更新通常标志着定位工作流的结束，因此默认情况下不会激活该选项。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="为拒绝内容生成出站过渡。"
>abstract="切换&#x200B;**“为拒绝内容生成出站过渡”**&#x200B;选项，可添加包含更新后未正确处理记录的出站过渡（例如，存在重复记录）。更新通常标志着定位工作流的结束，因此默认情况下不会激活该选项。"



<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="外部信号"
>abstract="借助&#x200B;**外部信号**&#x200B;活动，您可以从 API 或另一个工作流触发工作流中一组任务的执行。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="外部信号参数"
>abstract="外部信号参数"


>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="结束触发器"
>abstract="结束触发器"


<!--JavaScript-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript 代码"
>abstract="**JavaScript 代码**&#x200B;活动在工作流上下文中执行 JavaScript 代码。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript 代码片段"
>abstract="配置要执行的代码。"
>additional-url="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/api" text="请参阅 Campaign v8（控制台）文档了解详情。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript 执行"
>abstract="默认情况下，执行阶段不能超过 1 小时。延迟之后，该进程将会中止并会显示错误消息，并且活动执行会失败。切换&#x200B;**“停止执行于”**&#x200B;选项来定义自定义延迟。若要忽略此限制，请将该值设置为 0。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="流程错误"
>abstract="切换&#x200B;**“处理错误”**&#x200B;选项，可添加包含错误的出站过渡。"



<!--ExtractFile-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="提取文件"
>abstract="提取文件活动"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="要提取的文件"
>abstract="选择要提取的文件。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="目标格式"
>abstract="选择格式。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="后处理"
>abstract="定义后处理步骤"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="出站过渡"
>abstract="切换&#x200B;**“生成出站过渡”**&#x200B;选项，可在当前活动后添加出站过渡。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="流程错误"
>abstract="切换&#x200B;**“处理错误”**&#x200B;选项，可添加包含错误的出站过渡。"

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="初始化脚本"
>abstract="初始化脚本"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="执行属性"
>abstract="执行属性"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="执行错误"
>abstract="执行错误"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="执行初始化脚本"
>abstract="执行初始化脚本"


<!--incremental querry -->

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="增量查询"
>abstract="增量查询"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="增量查询历史记录"
>abstract="增量查询历史记录"


<!-- Transfer file activity -->

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="传输文件"
>abstract="传输文件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="传输文件选项"
>abstract="传输文件选项"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="传输文件活动"
>abstract="传输文件活动"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="传输文件远程服务器"
>abstract="传输文件远程服务器"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="传输文件源"
>abstract="传输文件源"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="传输后删除源文件"
>abstract="传输后删除源文件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="显示会话日志"
>abstract="显示会话日志"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="列出所有文件"
>abstract="列出所有文件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="文件历史记录"
>abstract="文件历史记录"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="处理缺失的文件"
>abstract="处理缺失的文件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="流程错误"
>abstract="流程错误"

>[!CONTEXTUALHELP]
>id="acw_deliveries_alerting"
>title="投放提醒"
>abstract="投放提醒"
