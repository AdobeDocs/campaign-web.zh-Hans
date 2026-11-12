---
title: Campaign Standard与Campaign v8之间的差异
description: 了解从Campaign Standard过渡到Campaign v8时发生了什么变化，以及在何处查找详细信息
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
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 2%
---
# Campaign Standard与Campaign v8之间的差异 {#acs-v8-differences}

Campaign Standard和Campaign v8中的大多数概念相同。 此页面汇总了过渡后影响您的差异，并链接到介绍每个差异的页面。 它补充了[营销人员](marketers.md)以及[管理员和开发人员](admin-developers.md)的指南。

* 有关术语的更改，请参阅[Campaign Standard与Campaign v8之间的主要差异](overview.md#experiences)。
* 有关转换后要运行的检查和报告的问题，请参阅[转换后的检查和疑难解答](post-transition-checks.md)。
* 有关只能在客户端控制台中使用的功能，请参阅[Campaign Web和Campaign客户端控制台](../../v8/get-started/capability-matrix.md)。

## 渠道和内容 {#channels}

创建和发送消息的步骤在这两个产品中都很相似，如营销人员指南[中所述](marketers.md)。 以下差异与渠道可用性、测试投放、登陆页面和直邮工作流有关。

| 更改内容 | 了解详情 |
|---|---|
| 应用程序内渠道在Campaign v8中不可用。 | [应用程序内频道](marketers.md#acs-gs-marketers-in-app) |
| 要过渡现有的推送工作流和投放，请联系您的Adobe Campaign过渡经理。 | [推送通知](marketers.md#acs-gs-marketers-push) |
| 在Campaign Standard中，可以将测试配置文件标记为&#x200B;**陷阱**&#x200B;以接收最终发送。 在Campaign v8中，启用选项以在投放的主要受众中包含测试用户档案。 | [测试投放](../../v8/preview-test/test-deliveries.md) |
| 在Campaign Web用户界面中创建的登陆页不支持隐藏的输入字段或自定义JavaScript。 | [登陆页面](../../v8/landing-pages/get-started-lp.md) |
| 在Campaign Standard中，直邮活动的叫客过渡也承载了生成的文件。 在Campaign v8中，它仅携带目标群体。 若要将文件发送到服务器，请添加&#x200B;**数据提取**&#x200B;活动，然后添加&#x200B;**文件传输**&#x200B;活动。 | [直邮](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## 受众、工作流和投放 {#data-and-workflows}

这些差异会影响从Campaign Standard迁移的受众和工作流、定期投放和&#x200B;**文件传输**&#x200B;活动的一些选项，以及动态报告的范围。

| 更改内容 | 了解详情 |
|---|---|
| 受众会在过渡期间发生转变。 例如，通过查询活动创建的受众会成为预定义过滤器，而文件类型受众会成为没有维度的列表类型受众。 | [管理受众](marketers.md#acs-gs-marketers-audiences) |
| 在Campaign Standard中执行的工作流的历史日志不会迁移。 | [创建工作流](marketers.md#acs-gs-marketers-wf) |
| 在Campaign Standard中，您可以选择定期电子邮件的聚合期。 此选项在Campaign v8中不可用。 | [渠道活动](../../v8/workflows/activities/channels.md) |
| 在Campaign Standard中，**文件传输**&#x200B;活动可以按字母数字对文件进行排序。 此选项在Campaign v8中不可用。 | [传输文件](../../v8/workflows/activities/transfer-file.md) |
| 动态报告涵盖电子邮件投放、包含电子邮件投放的营销活动和事务型消息。 | [报告](marketers.md#acs-gs-marketers-reporting) |

## 访问和安全性 {#access}

Campaign Standard安全组、角色和组织单位在过渡期间映射到操作员组、已命名权限和文件夹权限。 请仔细阅读以下要点，尤其是当某些用户的权限比以前更广泛或更窄时。

| 更改内容 | 了解详情 |
|---|---|
| 安全组、角色和组织单位映射到操作员组、已命名权限和文件夹权限。 自定义角色不会迁移。 | [用户访问管理](user-management-acs.md) |
| 具有&#x200B;**数据模型**&#x200B;角色但不具有&#x200B;**管理**&#x200B;角色的用户获得&#x200B;**管理**&#x200B;访问权限。 | [用户访问管理](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| 在Campaign v8中，分配给具有并行组织单位的安全组的用户可以拥有更广泛的访问权限。 | [并行组织单位分配](user-management-acs.md#parallel-assignments) |
| 从执行实例访问事务型API需要新的产品用户档案。 | [产品配置文件映射](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| 隐私请求可能会在Campaign Standard环境保持活动状态的时段内同时进入Campaign Standard和Campaign v8。 | [隐私和同意](admin-developers.md#privacy-and-consent) |

## 管理、跟踪和镜像页面 {#admin-tracking}

这些差异会影响在过渡之前从Campaign Standard发送的投放以及未转移到Campaign v8的管理信息。

| 更改内容 | 了解详情 |
|---|---|
| 在过渡之前从Campaign Standard发送的投放的镜像页面不可用。 从Campaign v8发送的投放的镜像页面可正常使用。 | [镜像页面](../../v8/email/mirror-page.md) |
| Campaign v8不会捕获在过渡之前从Campaign Standard发送的实时事务投放的跟踪数据。 这些消息的链接仍会重定向。 | [监视事务性消息](../../v8/transactional-messaging/monitor-transactional.md) |
| 不保留草稿投放的跟踪URL设置。 过渡后，跟踪、镜像页面和订阅链接将遵循Campaign v8标准，默认情况下会跟踪链接。 | [添加链接并跟踪消息](../../v8/email/message-tracking.md) |
| 没有地理单位。 基于地理单位的访问控制丢失。 | [访问控制](../../v8/get-started/connect-to-campaign.md#access-control) |
| 转换后，**创建者**&#x200B;和&#x200B;**修改者**&#x200B;实体信息不可用。 | [审核记录](admin-developers.md#acs-gs-admin-audit-trail) |
| 品牌化子域URL将调整为Campaign v8标准。 不迁移非标准品牌策略配置，而是通过默认品牌提供。 | [品牌](../../v8/administration/branding/branding-gs.md) |

## API和集成 {#apis-and-integrations}

这些差异会影响通过其REST API调用Campaign的集成，以及与其他Adobe解决方案和工具的集成。

| 更改内容 | 了解详情 |
|---|---|
| 迁移后，PKEY值会发生变化。 如果您将PKEY存储在Campaign之外，请改为遵循API返回的href。 | [REST API](admin-developers.md#acs-gs-admin-apis) |
| 某些已迁移的配置文件字段，如时区和`ccpaOptOut`，仅由`profileAndServicesExt/profile` API返回。 | [REST API](admin-developers.md#acs-gs-admin-apis) |
| Campaign Standard的Dreamweaver和Adobe Experience Platform Data Connector集成在Campaign v8中不可用。 | [使用Campaign和其他Adobe解决方案](../../v8/integrations/integration.md) |
| Adobe会迁移您的Adobe Analytics和Audience Manager配置。 您必须再次设置触发器和Adobe Target集成。 | [管理Adobe Campaign集成](admin-developers.md#acs-gs-integrations) |
