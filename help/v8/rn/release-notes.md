---
audience: end-user
title: Campaign Web v8 发行说明
description: Campaign Web v8 发行说明
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: 0703b872bb8f452773e76f2524d47bf774c687e0
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 80%

---


# 发行说明 {#release-notes}

此页面列出了 Campaign Web v8 的所有最新功能和改进。

## Alpha 发行版{#alpha-release}

这个新的 Campaign Web 界面目前仅适用于 **Alpha 从业人员**，并具有以下功能：

**现代、直观且统一的体验**

Campaign 的新 Web UI 提供了新的用户体验，并与所有 Adobe Experience Cloud 解决方案和应用程序保持一致。它提供：

* 通过单个共享的Adobe会话访问新界面和您的其他用户解决方案
* 新的导航体验，可从左边栏访问所有菜单和文件夹
* 顶栏中的解决方案和组织切换器
* Unified Shell 集成，可直接访问社区、帮助中心和支持

**新的强大功能和无缝流程**

* 重新设计的工作流画布界面以设计和管理您的流程
* 动态内容，可为受众提供极具针对性和个性化的体验
* 与Adobe Experience Platform受众的本机集成
* 工作流、投放、活动和内容的模板管理

在[此页面](../get-started/user-interface.md)中详细了解新 UI。

**创建、启动和衡量您的营销活动**

利用新的 Campaign Web UI，可以：

* 使用电子邮件设计器设计个性化的电子邮件内容 - [了解详情](../content/edit-content.md)
* 发送跨渠道营销活动，包括短信和推送通知。
* 使用规则生成器定义目标受众 - [了解详情](../audience/about-audiences.md)
* 预览、测试和发送电子邮件 - [了解详情](../monitor/prepare-send.md)
* 使用内置报告监控发送和衡量结果 - [了解详情](../reporting/delivery-reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## 术语更新{#terminology-updates}

作为现有 Campaign 用户，请注意，已对一些概念进行重命名以符合最新的术语标准。这些更改仅适用于 Campaign Web UI，并且不会反映在客户端控制台中。下面对它们进行了汇总。

* 验证现在是&#x200B;**测试电子邮件**：要发送验证，请使用电子邮件投放 UI 中的&#x200B;**测试**&#x200B;按钮。验证目标的目标现在称为&#x200B;**测试配置文件**
* 种子地址现在用作&#x200B;**测试配置文件**：将测试电子邮件发送到种子地址，这些地址是数据库中的额外和虚构的收件人
* 投放分析现在是&#x200B;**投放准备**。在需要启动分析时，请单击&#x200B;**准备**&#x200B;按钮
* 电子邮件预览现在可通过&#x200B;**模拟内容**&#x200B;按钮使用
* 列表现在是&#x200B;**受众**

## 限制{#limitations-alpha}

以下限制适用于此 Alpha 版本：

* 可编辑的对象只有投放、营销策划、工作流、受众和模板。 其他对象是只读的。使用筛选器来浏览所有对象。
* 管理用户界面不可用。
* 报告量度（例如，打开次数和跟踪数据）每小时更新一次。
* 投放仪表板 KPI 每 5 分钟更新一次。- 但投放准备是实时的。
* 顶栏中可用的 Adobe Experience Cloud 通知和统一帮助尚未集成。

