---
audience: end-user
title: 探索界面
description: Campaign v8 Web 用户界面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: a974221fa5b46ea9463c98724b1f49a7edb0adb7
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 98%

---

# 探索界面 {#user-interface}

新的 Campaign v8 Web 界面提供一种现代而直观的用户体验以简化营销活动的设计和投放。此新界面与 Adobe Experience Cloud 应用程序和解决方案集成。


>[!NOTE]
>
>此文档经常更新以反映产品用户界面中的最新更改。但是，某些屏幕快照可能与用户界面略有不同。


## 左侧导航菜单 {#user-interface-left-nav}

浏览左侧链接以访问 Campaign v8 Web 功能。多个链接显示了可排序和筛选的对象的列表。您还可以配置列以显示所需的所有信息。请参阅此[部分](#list-screens)。某些列表屏幕为只读。左侧导航菜单和列表中显示的项目取决于您的用户权限。可在[此部分](permissions.md)中详细了解权限。

![](assets/home.png)

### 主页 {#user-interface-home}

此屏幕包含用于快速访问主要 Campaign v8 Web 功能的关键链接和资源。

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="最近访问"
>abstract="**最近项目**&#x200B;列表提供了最近创建和修改的投放的快捷方式。此列表显示了它们的渠道、状态、所有者、创建日期和修改日期。"

**最近**&#x200B;列表提供了最近创建和修改的投放的快捷方式。此列表显示了它们的渠道、状态、所有者、创建日期和修改日期。单击&#x200B;**显示更多**&#x200B;链接，加载更多投放。

利用&#x200B;**关键绩效指标 (KPI)**，可以通过常见 KPI 检查平台有效性。可在[此页面](../reporting/kpis.md)中详细了解这些 KPI。


从主页的&#x200B;**学习**&#x200B;部分访问 Campaign v8 Web 关键帮助页面。

### 探索工具 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="**探索工具**&#x200B;菜单使用与客户端控制台中的文件夹层次结构相同的文件夹层次结构显示所有 Campaign 组件和对象。浏览您的所有 Campaign v8 组件、文件夹和架构，检查关联的权限，然后从此菜单创建文件夹和子文件夹。"

**资源管理器**&#x200B;菜单按照与客户端控制台中相同的文件夹层次结构显示所有 Campaign 资源和对象。浏览所有 Campaign v8 组件、文件夹和架构，并创建投放、工作流和营销活动。

**资源管理器**&#x200B;中显示的项目取决于您的用户权限。如果您具有适当的权限，也可以添加文件夹和子文件夹。可在[此部分](permissions.md)中详细了解权限。

可配置列以自定义显示，以便查看所需的所有信息。请参阅此[部分](#list-screens)。还可添加文件夹和子文件夹，如[此部分](permissions.md#folders)中所详述。

有关 Campaign 探索工具、文件夹层次结构和资源的更多信息，请参阅此 [Campaign v8（控制台）文档 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=zh-Hans#ac-explorer-ui){target="_blank"}。

### Campaign 管理 {#user-interface-campaign-management}

在“营销活动管理”部分中，可访问市场营销活动、投放情况和工作流。

* **营销活动** - 这是您的营销活动和营销活动模板的列表。默认情况下，可查看每个营销活动的开始/结束/创建/上次修改日期、当前状态以及创建它的 Campaign 操作员的姓名。可按状态、开始/结束日期和文件夹筛选该列表，也可创建高级筛选器以定义您自己的筛选条件。可[在此部分中](../campaigns/gs-campaigns.md)详细了解营销活动。

* **投放** - 浏览您的投放列表。默认情况下，您可以查看它们的状态、最后修改日期以及关键 KPI。您可以按状态、联系日期或渠道筛选列表。单击电子邮件投放以打开其仪表板来获取投放详细信息的概述。其他渠道上的投放是只读的。可[在此部分中](../msg/gs-messages.md)详细了解投放。

  使用&#x200B;**更多操作**&#x200B;按钮删除或重复投放。

  ![](assets/more-actions.png){width="70%" align="left"}

* **工作流** - 可在此屏幕中访问工作流和工作流模板的完整列表。可检查其状态、上次/下次执行日期，并可创建新的工作流或新的工作流模板。可用与筛选其他对象相同的条件筛选该列表。此外，还可筛选属于或不属于营销活动的工作流。可[在此部分中](../workflows/gs-workflows.md)详细了解工作流。


### 客户管理 {#user-interface-customer-management}

在“客户管理”部分中，您可以查看收件人、受众和订阅。这些列表为只读。

* **收件人** - 访问您的收件人数据库。默认情况下，您可以查看他们的电子邮件地址、名字和姓氏。可在[此部分](../audience/about-recipients.md)中详细了解收件人。
* **受众** - 这是您的受众列表。默认情况下，您可以查看它们的类型、来源、创建/最后修改日期和标签。您可以按来源筛选列表。可在[此部分](../audience/about-recipients.md)中详细了解受众和列表。
* **订阅** - 浏览您的订阅列表。默认情况下，您可以查看它们的类型、模式和标签。请参阅 [Adobe Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=zh-Hans){target="_blank"}，了解如何管理订阅和退订。

### 决策管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="优惠"
>abstract="浏览在控制台中使用&#x200B;**交互**&#x200B;模块创建的优惠和优惠模板的列表。这些列表为只读。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=zh-Hans" text="将优惠添加到投放"

在“决策管理”部分中，您可以查看优惠和优惠模板。这些列表为只读。

* **优惠** - 浏览在控制台中使用&#x200B;**交互**&#x200B;模块创建的优惠和优惠模板的列表。默认情况下，您可以查看它们的状态、开始/结束日期和环境。您可以按状态和开始/结束日期筛选列表。还有优惠模板可用。

可在[此部分](../content/offers.md)中了解如何在电子邮件和短信中创建和发送优惠。



## 上下文帮助 {#user-interface-help}

界面中提供了上下文帮助。当 `?` 图标可用时，单击该图标可显示帮助信息和相关文档链接。

![](assets/context-help.png){width="40%" align="left"}

通过新的 Beta 版本，嵌入在上下文帮助中的 **AI 支持的知识助手**&#x200B;彻底改变了文档搜索和解答操作方法疑问的方式，它可轻松地筛选大型文档存储库并立即找出所需的准确信息。

通过 Campaign 生成式 AI 的各项功能，此助手改变您的体验，使检索信息和解决问题变得轻而易举。无论您是在复杂的任务中寻求指导，还是在大量文档中导航，我们的 AI 支持的知识助手都是您的绝佳伙伴，每次互动的效率和准确性都无与伦比。

可在[此小节](using-ai.md)中了解详情。



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

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全球报告发送"
>abstract="跟踪报告量度在此屏幕中可见"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全球报告跟踪"
>abstract="跟踪报告量度在此屏幕中可见"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Campaign 中的工作流列表"
>abstract="Campaign 中的工作流列表"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="收件人创建"
>abstract="收件人创建"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="收件人详细信息"
>abstract="收件人详细信息"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="收件人联系信息"
>abstract="收件人联系信息"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="收件人地址"
>abstract="收件人地址"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="收件人帐户"
>abstract="收件人帐户"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="收件人自定义字段"
>abstract="收件人自定义字段"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="收件人不再联系"
>abstract="收件人不再联系"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="收件人其他"
>abstract="收件人其他"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="收件人信息卡概述"
>abstract="收件人信息卡概述"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="收件人接触点"
>abstract="收件人接触点"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="收件人订阅列表"
>abstract="收件人订阅列表"

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
>id="acw_recipients_readonlyprofile"
>title="收件人只读配置文件"
>abstract="收件人只读配置文件"





>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="测试用户档案附加数据"
>abstract="测试用户档案附加数据"




>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="订阅投放模板"
>abstract="订阅投放模板"





>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="登陆页面"
>abstract="登陆页面"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="登陆页面属性"
>abstract="登陆页面属性"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="登陆页面页"
>abstract="登陆页面页"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="登陆页面计划"
>abstract="登陆页面计划"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="登陆页面主页"
>abstract="登陆页面主页"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="登陆页面订阅"
>abstract="登陆页面订阅"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="登陆页面行动号召"
>abstract="登陆页面行动号召"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="登陆页面模拟"
>abstract="登陆页面模拟"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="活动不可编辑"
>abstract="活动不可编辑"




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
>id="acw_contenttemplate_menu"
>title="内容模板"
>abstract="内容模板"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="内容模板属性"
>abstract="内容模板属性"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="内容模板设计"
>abstract="内容模板设计"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="内容模板选择"
>abstract="内容模板选择"





>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="协调活动"
>abstract="使用&#x200B;**协调**&#x200B;活动将未识别的数据链接到现有资源。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="协调定位"
>abstract="协调定位"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="协调规则"
>abstract="协调规则"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="协调定位维度"
>abstract="协调定位维度"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="协调选择字段"
>abstract="协调选择字段"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="协调选择属性"
>abstract="协调选择属性"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="协调创建条件"
>abstract="协调创建条件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="协调生成补集"
>abstract="协调生成补集"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="协调将保留未协调的数据选项"
>abstract="协调将保留未协调的数据选项"



>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="合并生成补充"
>abstract="合并生成补充"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="拆分活动的区段"
>abstract="拆分活动的区段"




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
>id="acw_audiences_properties"
>title="受众属性"
>abstract="受众属性"

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="受众人数"
>abstract="受众人数"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="模拟测试配置文件"
>abstract="模拟测试配置文件"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="模拟测试配置文件选择"
>abstract="模拟测试配置文件选择"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="模拟测试配置文件发送"
>abstract="模拟测试配置文件发送"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="模拟电子邮件日志"
>abstract="模拟电子邮件日志"


>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="订阅总数"
>abstract="订阅总数"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="期间订阅量"
>abstract="期间订阅量"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="订阅整体演变"
>abstract="订阅整体演变"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="直邮内容"
>abstract="直邮内容"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="直邮的文件属性"
>abstract="直邮的文件属性"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="直邮的内容属性"
>abstract="直邮的内容属性"




>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="加载文件活动"
>abstract="加载文件活动"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="示例文件"
>abstract="示例文件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="文件名称"
>abstract="文件名称"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="目标数据库"
>abstract="目标数据库"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="加载文件活动的拒绝管理"
>abstract="加载文件活动的拒绝管理"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="拒绝管理出站过渡"
>abstract="拒绝管理出站过渡"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="针对拒绝的拒绝管理出站过渡"
>abstract="针对拒绝的拒绝管理出站过渡"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="加载文件活动的格式设置"
>abstract="加载文件活动的格式设置"
