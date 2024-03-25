---
title: 最新发行说明
description: 发现 Campaign Web 用户界面附带的新功能
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 99%

---

# 发行说明 {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="新增功能"
>abstract="Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。发行说明每月更新几次。**3 月版本已上线**，包括直邮渠道、全新更改数据源工作流活动以及其他改进。"


<!--Last update: **March 19, 2024**-->

Adobe Campaign Web 用户界面版本在持续投放模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。因此，这些发行说明每月更新几次。请定期检查。

>[!AVAILABILITY]
>
>此版本适用于所有 [Campaign（控制台）v8.6 及更高版本](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans)的用户。请参阅 [Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hans){target="_blank"}，了解有关 Adobe Campaign 客户端控制台版本和升级的更多信息。

## 3月发行说明 {#24-3-release}

**发布日期**：2024 年 3 月 19–20 日

### 直邮渠道 {#24-3-dm}

**直邮**&#x200B;渠道现在既可在工作流中使用，也可独立投放。直邮是一种离线渠道，允许您创建和生成提取文件、进行个性化设置，并与直邮提供商共享，向客户发送邮件。[了解更多信息](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 新的更改数据源工作流活动 {#24-3-change-data-source}

**更改数据源**&#x200B;定位活动允许您更改工作流工作表使用的数据源。这项活动提供了更大的灵活性，使您可以跨不同的数据库管理数据并提高性能。[了解更多信息](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### 拆分工作流活动改进 {#24-3-split}

现在，您可以使用“**拆分**”工作流活动中的“**在同一表中生成所有子集**”选项，将所有子集分组到单个输出过渡中。[了解更多信息](../workflows/activities/split.md)

### 查询建模器 {#24-3-query-modeler}

* 查询建模器现在可在电子邮件设计器中使用。它允许您在创建条件内容时构建条件。[了解更多信息](../personalization/conditions.md)
* 创建自定义条件时，预定义值现在可用于日期类型属性。[了解更多信息](../query/build-query.md)
* 无法再在图中的新过渡上添加运算符。运算符只能添加到现有的过渡中，然后再过滤组件将它们分组在一起。[了解更多信息](../query/build-query.md)
