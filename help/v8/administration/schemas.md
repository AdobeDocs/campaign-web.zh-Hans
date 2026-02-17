---
title: 关于架构
description: 了解如何使用架构。
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 6%

---

# 关于架构 {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="架构"
>abstract="Adobe Campaign使用基于XML的架构来定义应用程序中数据的物理和逻辑结构。 在此屏幕中，您可以直接从Web用户界面查看所有现有架构、访问架构详细信息、配置自定义表单以及创建或扩展架构。"

**[!DNL Adobe Campaign]** 使用基于 XML 的架构定义应用程序内数据的物理和逻辑结构。架构是链接到数据库表的XML文档，该数据库表定义：

* SQL表结构，包括表名、字段和关系。
* XML数据结构，包括元素、属性、层次结构、类型、默认值和标签。

架构在以下方面发挥着关键作用：

* 将应用程序数据映射到数据库表。
* 定义数据对象之间的关系。
* 指定每个字段的结构和属性。

Adobe Campaign中的每个实体都有一个专用架构，确保数据一致性和组织性。

利用模式界面，您可以：

* [访问和自定义架构](schemas-browse-access.md) — 查看可用的架构，浏览其详细信息并自定义屏幕显示
* [配置列表列](schemas-list-columns.md) — 配置在列表视图中默认显示的列。
* [编辑自定义字段](schemas-custom-fields.md) — 配置哪些自定义字段在详细信息屏幕中显示并将它们整理到多个部分中。
* [添加收藏集列表](schemas-collection-lists.md) — 添加收藏集列表以在配置文件屏幕中显示相关数据。
* [创建和管理架构](schemas-create-publish.md#create-schemas) — 创建新架构并扩展现有架构
* [发布并同步架构](schemas-create-publish.md#publish) — 同步架构更改与数据库结构。
* [使用自定义表单](schemas-custom-forms.md) — 使用数据输入表单在自定义架构中创建、编辑和管理记录。

>[!NOTE]
>
>您需要具有管理员权限才能管理架构。

有关架构的详细信息，请参阅[Campaign控制台文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}。
