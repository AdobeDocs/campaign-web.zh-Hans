---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 6581a2d6ab44b711ed6aea6736d60f932a7ce315
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 45%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。 我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

## ’26年6月版 {#26-6-release}

_2026年6月16日_

### 改进 {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* 您现在可以从任何列表屏幕（包括跟踪日志）导出数据。 找到您的列表，只需单击“导出”按钮即可。 导出包括当前加载的行，并考虑屏幕上显示的列以及任何活动的搜索或筛选条件。 [了解详情](../get-started/list-filters.md)

* **重复数据删除**&#x200B;和&#x200B;**结束**&#x200B;工作流活动现在支持多个集客过渡。 时间
有多个集客过渡可用，请使用活动中的&#x200B;**集加入**&#x200B;部分
属性以选择要连接的过渡。 在以下页面中了解详情： [重复数据删除](../workflows/activities/deduplication.md)，

<!--
[End](../workflows/activities/end.md)
-->

* 高级参数现在显示在&#x200B;**生成受众**（查询类型）和&#x200B;**扩充**&#x200B;工作流活动的&#x200B;**扩充数据**&#x200B;部分中。 利用这些参数，可优化扩充数据的构建方式，包括分组、重复数据删除、主键处理和入站事件数据。 [了解详情](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
