---
title: 过渡到Campaign v8后的检查和故障排除
description: 了解从Campaign Standard过渡到Campaign v8后要检查什么以及如何修复常见问题
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%
---
# 转换后的检查和故障排除 {#post-transition-checks}

从Campaign Standard过渡到Campaign v8后，某些投放、工作流和登陆页面的行为可能与您的预期不同。 下表列出了已转换的用户报告的症状、原因以及采取的措施。 有关差异的完整列表，请参阅[Campaign Standard与Campaign v8之间的差异](acs-v8-differences.md)。

| 症状 | 原因和要做什么 | 了解详情 |
|---|---|---|
| 投放中的链接是直接URL，不会收集任何点击数据。 | 在投放或其所基于的投放模板上禁用跟踪。 检查是否已启用&#x200B;**激活跟踪**，特别是针对定期投放的模板。 | [跟踪设置](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| 通过“mailto”List-Unsubscribe方法取消订阅的收件人不在隔离中。 | 这是正常情况。 这些收件人不会被隔离。 它们会取消订阅与投放关联的服务，或者在投放没有服务时添加到。 要跟踪这些取消订阅，请检查服务的订阅或配置文件的&#x200B;**不再联系**&#x200B;部分。 | [隔离](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| 登陆页面不会保存由脚本计算或存储在隐藏字段中的值。 | 在Campaign Web用户界面中创建的登陆页不支持隐藏的输入字段或自定义JavaScript。 改为在客户端控制台中将表单创建为Web应用程序。 | [登陆页面](../../v8/landing-pages/get-started-lp.md) |
| **文件传输**&#x200B;找不到直邮活动生成的文件。 | 直邮活动的出站过渡承载的是目标群体，而不是提取文件。 添加&#x200B;**数据提取**&#x200B;活动，然后添加&#x200B;**文件传输**&#x200B;活动。 | [直邮](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| 多个批次的投放会一起发送。 | 从投放联系日期开始安排批次。 如果投放在某些波次的计划时间后开始，则这些波次会一起发送，而不是相互隔开。 | [使用批次发送](../../v8/advanced-settings/send-using-waves.md) |
| 带有星号后字符的文件掩码在Azure Blob存储中找不到任何文件。 | Azure Blob存储按名称前缀过滤文件。 仅支持尾随星号。 | [转移外部帐户](../../v8/administration/transfer-external-account.md) |
| 在过渡之前发送的投放的镜像页面无法打开。 | 在过渡之前从Campaign Standard发送的投放的镜像页面不可用，没有解决方法。 从Campaign v8发送的投放的镜像页面可正常使用。 | [镜像页面](../../v8/email/mirror-page.md) |
| 使用自定义JavaScript的登陆页面或内容块的行为方式不同。 | 自定义JavaScript在迁移期间会进行转换，但会验证和调整它，尤其是当它使用`queryDef`、Campaign JavaScript API、会话写入、组织单位处理或自定义URL生成时。 | [登陆页面](../../v8/landing-pages/get-started-lp.md) |
