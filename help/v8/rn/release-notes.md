---
title: Campaign v8 Web 用户界面发行说明
description: 了解最新版 Campaign Web 用户界面的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: b8cf1d45b1a69efbe8e055d57b430d0fa04f8494
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 93%

---

# 发行说明 {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="发行说明"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，Campaign 发行说明每月更新数次，其中包含最新的功能、改进和修复。 我们建议您定期查看这些说明。"

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

## 2026 年 6 月版本 {#26-6-release}

_2026 年 6 月 16 日_

### 改进 {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* 您现在可以从任何列表界面（包括跟踪日志）导出数据。 找到您的列表，然后只需点击导出按钮即可。 导出包括当前加载的行，并会根据屏幕上显示的列以及任何正在进行的搜索或过滤器进行调整。 [了解详情](../get-started/list-filters.md)

* **重复数据删除**&#x200B;和&#x200B;**终止**&#x200B;工作流活动现在支持多个入站过渡。 当有多个集客过渡可用时，请使用活动中的&#x200B;**集加入**部分
属性，用于选择要连接的过渡。 请参阅以下页面了解更多信息：[重复数据删除](../workflows/activities/deduplication.md)、[终止](../workflows/activities/end.md)

* 高级参数现已显示在&#x200B;**扩充数据**&#x200B;部分，该部分在&#x200B;**构建受众**（查询类型）和&#x200B;**扩充**&#x200B;工作流活动中。 这些参数可让您对扩充数据的构建方式进行精细调整，包括分组、重复数据删除、主键处理以及入站事件数据。 [了解详情](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
