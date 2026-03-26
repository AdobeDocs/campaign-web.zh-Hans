---
title: 关于架构
description: 了解如何使用架构。
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 22%

---

# 关于架构 {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="架构创作"
>abstract="您现在可以直接从Campaign Web用户界面创建和管理架构。 您可以创建新表、扩展现有模式以及创建自定义表单。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="架构"
>abstract="Adobe Campaign 使用基于 XML 的架构来定义应用程序中数据的物理结构和逻辑结构。在此界面中，您可以查看所有现有架构、访问架构详细信息、配置自定义表单，并直接通过 Web 用户界面创建或扩展架构。"

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
