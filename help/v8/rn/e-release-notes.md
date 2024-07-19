---
title: Campaign v8 Web 用户界面早期发行说明
description: 了解下一版 Campaign Web 用户界面的新功能
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: d4f9f3562f7dc2550bf9fea01f27456fdfdad43e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 46%

---

# 早期发行说明 {#e-release}

Adobe Campaign Web 用户界面不断地提供新功能、对现有功能进行增强和修复错误。所有更改会在每月的最后整合到[发行说明](release-notes.md)中。

**以下早期发行说明在发行可用日期之前如有更改，恕不另行通知**。链接、屏幕和更新的文档会于发布日期在[发行说明](release-notes.md)中发布。

## 7月发行说明 {#24-7-release}

**发行日期**： 2024年7月30日至31日

从7月版本开始，将提供以下功能和改进。

### 种子列表 {#24-7-2}

种子列表，又名&#x200B;**Trap 组**，是种子地址列表。它用于在您的投放中包含特定地址，然后定位不符合定义的目标标准的配置文件。这样，不在投放受众内的收件人就可以像其他目标收件人一样收到投放内容。您可以在发送校样时或保护您的邮件列表时使用种子地址。

### 富推送通知模板{#24-7.3}

您现在可以发送富推送通知。 富推送通知是移动通知的增强形式，它通过结合多媒体元素（例如图像、交互式按钮或其他富媒体内容）而超越简单的文本消息。 在此版本中，现在为您的iOS和Android应用程序提供了一组富推送通知模板。

>[!AVAILABILITY]
>
>此功能需要更新Campaign v8.6.3或v8.7.2。[请参阅Campaign客户端控制台发行说明以了解详情](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes)


### 改进 {#improvements-24-7}

**文件夹管理** — 您现在可以管理文件夹的权限和限制。

### 有限可用性版本中的新功能 {#acs-24-4}

>[!AVAILABILITY]
>
>以下功能处于“有限可用性” (LA) 状态。这些功能仅限于从 **Adobe Campaign Standard 迁移至 Adobe Campaign v8** 的客户使用，并且不能部署在任何其他环境中。
>
>请参阅以下文档页面：[从 Campaign Standard 过渡到 Campaign v8](../rn/acs-migration.md) 以及[面向 Campaign Standard 用户的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hans)。

#### 内容片段 {#LA-24-7}

您现在可以创建和使用内容片段。 内容片段是可在一条或多条消息中引用的可重用组件。 修改片段时，使用该片段的每个内容都会更新。 此功能允许预先构建多个自定义内容块，营销用户可以使用这些内容块在改进的设计过程中快速组合消息内容。

提供了两种类型的片段：

* **表达式片段**&#x200B;是预定义表达式，可从表达式编辑器的专用条目中使用。
* **可视化片段**&#x200B;是预定义的可视化块，您可以在多个电子邮件投放中或在内容模板中重复使用。 [了解详情](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >**可视化片段**&#x200B;处于有限可用性(LA)。 此功能仅限于将&#x200B;**从Adobe Campaign Standard迁移到Adobe Campaign v8**&#x200B;的客户，不能在任何其他环境中部署。
