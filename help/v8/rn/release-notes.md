---
title: 最新发行说明
description: 发现 Campaign Web 用户界面附带的新功能
source-git-commit: 737a2ea3f3c5ecc41c692ada7927f5e60ecb256a
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 8%

---

# 发行说明 {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="新增功能"
>abstract="Adobe Campaign Web用户界面版本在持续交付模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 发行说明每月更新几次。 **3月版现已上线**，包括直邮渠道、新的更改数据源工作流活动和其他改进。"


<!--Last update: **March 19, 2024**-->

Adobe Campaign Web用户界面版本在持续交付模型上运行，通过该模型可采用更具可扩展性、分阶段的方法部署功能。 因此，这些发行说明每月更新几次。 请定期检查。

>[!AVAILABILITY]
>
>此版本对以下开始的所有用户都可用： [Campaign（控制台）版本8.6发布](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=zh-Hans). 在中详细了解Adobe Campaign客户端控制台的发布和升级 [Campaign v8（控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=zh-Hans){target="_blank"}.

## 3月版 {#24-3-release}

**发行日期**：2024年3月19日至20日

### 直邮渠道 {#24-3-dm}

**直邮** 渠道现在可用于工作流和独立投放。 直邮是一种线下渠道，允许您创建、个性化和生成提取文件，并与直邮提供商共享以向客户发送邮件。 [了解更多信息](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 新的更改数据源工作流活动 {#24-3-change-data-source}

此 **更改数据源** 利用定位活动，可更改工作流工作表使用的数据源。 本练习允许您跨不同的数据库管理数据并改进性能，从而提供了更大的灵活性。 [了解更多信息](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### 拆分工作流活动改进 {#24-3-split}

您现在可以使用 **在同一张表中生成所有子集** 中的选项 **Split** 工作流活动，用于将所有子集分组到单个输出转换中。 [了解更多信息](../workflows/activities/split.md)

### 查询建模器 {#24-3-query-modeler}

* 查询建模器现在可以在Email Designer中使用。 它允许您在创建条件内容时构建条件。 [了解更多信息](../personalization/conditions.md)
* 现在，创建自定义条件时，预定义值可用于日期类型属性。 [了解更多信息](../query/build-query.md)
* 不能再向图中的新过渡添加运算符。 它们只能在筛选组件以将它们分组到一起之前添加到现有过渡上。 [了解更多信息](../query/build-query.md)
