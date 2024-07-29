---
title: Campaign v8 Web 用户界面早期发行说明
description: 了解下一版 Campaign Web 用户界面的新功能
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: f8bdb15151774b33a0bcf16e86347dae6ab417a2
workflow-type: ht
source-wordcount: '401'
ht-degree: 100%

---

# 早期发行说明 {#e-release}

Adobe Campaign Web 用户界面不断地提供新功能、对现有功能进行增强和修复错误。所有更改会在每月的最后整合到[发行说明](release-notes.md)中。

**以下早期发行说明在发行可用日期之前如有更改，恕不另行通知**。链接、屏幕和更新的文档会于发布日期在[发行说明](release-notes.md)中发布。

## 7 月份发行说明 {#24-7-release}

**发布日期**：2024 年 7 月 30-31 日

自 7 月版本开始可以使用以下功能和改进。

### 内容片段 {#24-7-1}

您现在可以创建和使用内容片段。内容片段是可重复使用的组件，可以在一条或多条消息中引用。当修改片段时，使用它的每个内容都会被更新。此功能用于预构建多个自定义内容块，营销用户可以使用这些块在改进的设计过程中快速组装消息内容。

有两种类型的片段可用：

* **表达式片段** 是预定义表达式，可从表达式编辑器中的专用条目中获取。
* **视觉片段** 是预定义的视觉块，您可以在多个电子邮件传递或内容模板中重复使用。[了解详情](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >**视觉片段** 处于有限可用性（LA）。该功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。

### 种子列表 {#24-7-2}

种子列表，又名&#x200B;**Trap 组**，是种子地址列表。它用于在您的投放中包含特定地址，然后定位不符合定义的目标标准的配置文件。这样，不在投放受众内的收件人就可以像其他目标收件人一样收到投放内容。您可以在发送校样时或保护您的邮件列表时使用种子地址。

### 富推送通知模板 {#24-7-3}

您现在可以发送富推送通知。富推送通知是移动通知的一种增强形式，它不局限于简单的文本消息，而是融合了图像、交互式按钮或其他富媒体内容等多媒体元素。在此版本中，您可以为您的 iOS 和 Android 应用程序提供一组丰富的推送通知模板。

>[!AVAILABILITY]
>
>此功能需要更新至 Campaign v8.6.3 或 v8.7.2。详情请参阅 [Campaign v8 客户端控制台发行说明](https://experienceleague.adobe.com/zh-Hans/docs/campaign/campaign-v8/releases/release-notes)

### 改进 {#improvements-24-7}

**文件夹管理** - 您现在可以管理文件夹的权限和限制。
