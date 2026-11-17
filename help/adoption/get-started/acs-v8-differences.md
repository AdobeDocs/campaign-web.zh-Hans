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
source-git-commit: 64a07e65b7e6d933288b10117aae99f48d13a8d8
workflow-type: tm+mt
source-wordcount: '1721'
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
| 在Campaign Standard中，可以将测试配置文件标记为&#x200B;**陷阱**&#x200B;以接收最终发送。 在Campaign v8中，在投放的受众设置中添加&#x200B;**陷阱组**。 | [陷阱组](../../v8/audience/trap-group.md) |
| 在Campaign Web用户界面中创建的登陆页不支持隐藏的输入字段或自定义JavaScript。 | [登陆页面](../../v8/landing-pages/get-started-lp.md) |
| 在Campaign Standard中，直邮活动的叫客过渡也承载了生成的文件。 在Campaign v8中，它仅携带目标群体。 若要将文件发送到服务器，请添加&#x200B;**数据提取**&#x200B;活动，然后添加&#x200B;**文件传输**&#x200B;活动。 | [直邮](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## 受众、工作流和投放 {#data-and-workflows}

这些差异会影响从Campaign Standard迁移的受众和工作流、定期投放和&#x200B;**文件传输**&#x200B;活动的一些选项，以及动态报告的范围。

| 更改内容 | 了解详情 |
|---|---|
| 受众会在过渡期间发生转变。 例如，通过查询活动创建的受众会成为预定义过滤器，而文件类型受众会成为没有维度的列表类型受众。 | [管理受众](marketers.md#acs-gs-marketers-audiences) |
| 在Campaign Standard中执行的工作流的历史日志不会迁移。 | [创建工作流](marketers.md#acs-gs-marketers-wf) |
| 在Campaign Standard中，您可以选择定期电子邮件的聚合期。 此选项在Campaign v8中不可用。 | [渠道活动](../../v8/workflows/activities/channels.md) |
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

## API和集成 {#apis-and-integrations}

这些差异会影响通过其REST API调用Campaign的集成，以及与其他Adobe解决方案和工具的集成。

| 更改内容 | 了解详情 |
|---|---|
| 迁移后，PKEY值会发生变化。 如果您将PKEY存储在Campaign之外，请改为遵循API返回的href。 | [密钥用法](#key-usage) |
| 某些已迁移的配置文件字段，如时区和`ccpaOptOut`，仅由`profileAndServicesExt/profile` API返回。 | [配置文件时区](#profile-timezone) |
| Adobe会迁移您的Adobe Analytics和Audience Manager配置。 您必须再次设置触发器和Adobe Target集成。 | [管理Adobe Campaign集成](admin-developers.md#acs-gs-integrations) |

## REST API建议和限制 {#rest-api-limitations}

从Campaign Standard过渡到Campaign v8时，以下建议和限制适用于REST API。

### 权限和安全性 {#permissions}

#### 产品配置文件映射 {#rest-product-profiles}

在Campaign Standard中，无论您分配了什么产品配置文件，都向您授予了更高的API管理员角色访问权限。 Campaign v8引入了一组不同的产品配置文件，需要从Campaign Standard映射到Campaign v8产品配置文件。

通过迁移，可将两个产品配置文件添加到您现有或预先创建的技术帐户：管理员和消息中心（用于访问事务型API）。 如果您不希望将管理员产品配置文件映射到您的技术帐户，请查看产品配置文件映射，并分配所需的产品配置文件。

#### 租户 ID

迁移后，对于任何未来的集成，建议在REST URL中使用您的&#x200B;**Campaign v8租户ID**，替换您之前的Campaign Standard租户ID。

#### 密钥用法

对PKey值的管理在Campaign Standard和Campaign v8之间有所不同。 如果您使用Campaign Standard存储PKeys，请确保您的实施使用从以前的API调用中获取的PKeys或href动态形成后续API调用。

### 可用API {#available-apis}

目前，下面列出的REST API可供使用：

* **配置文件**
* **服务和订阅**
* **自定义资源**
* **工作流**
* **事务性消息**

>[!AVAILABILITY]
>
>目前，**事务性消息** REST API不可用。
>
>下面列出的REST API已弃用，无法使用：
>* 营销历史记录
>* 组织实体
>* 隐私管理

### 筛选 {#rest-filtering}

* 要在REST API负载中使用筛选器，您需要在Campaign v8中编辑这些筛选器，并提供要在负载中使用的名称。 为此，请从&#x200B;**[!UICONTROL 参数]**&#x200B;选项卡访问筛选器的其他参数，并在REST API的&#x200B;**[!UICONTROL 筛选器名称]**&#x200B;字段中提供所需的名称。

  ![](assets/api-filtering.png)


* 不再需要使用自定义筛选器所需的“by”前缀。 过滤器名称应按照原样在请求中使用。

  示例：

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### 删除的数据库字段 {#dropped-fields}

迁移期间将删除数据库中的某些字段。 使用放置的字段时，REST API将返回空白值。 将来，弃用和删除所有已删除的字段。

### 使用链接的资源发布 {#post-linked}

使用以下请求正文格式时，“vehicleOwner”表示指向“nms:recipient”的链接：

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

链接信息将被忽略。 因此，在“cusVehicle”下生成了一个仅包含“vehicleNumber”和“vehicleName”值的新记录。 但是，链接仍然为空，导致“vehicleOwner”被设置为null。

在Campaign v8中，当使用相同的请求正文结构并且“vehicle”链接到用户档案时，会发生错误。 出现此错误是因为“firstName”属性未被识别为“cusVehicle”有效。 但是，请求正文仅包含属性而没有链接功能，没有任何问题。

### PATCH操作 {#patch}

* Campaign v8不支持请求正文为空的PATCH：它返回“204无内容”状态。
* 虽然Campaign Standard在架构内的元素/属性上支持PATCH，但请注意，Campaign v8不支持在位置上执行PATCH操作。 尝试在位置上使用PATCH会导致500内部服务器错误，并显示一条错误消息，指示“zipCode”属性对于“profile”资源无效。

### REST响应 {#rest-responses}

以下部分列出了Campaign Standard与v8 REST响应之间的细微差异。

* 对于单个GET记录，响应中包含href。
* 在使用属性进行查询时，Campaign v8在响应中提供计数和分页。
* POST操作后，响应中会返回链接资源的值。

### 错误代码和消息 {#rest-errors}

以下部分列出了Campaign Standard与Campaign v8错误代码和消息之间的差异。

| 场景 | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| 在请求正文中使用无效的PKey | 500 — “O5iRp40EGA”属性未知(请参阅“配置文件(nms:recipient)”架构的定义)。 XTK-170036无法解析表达式“@id = @O5iRp40EGA”。 | 404 — 无法解密PKey。 (PKey=@jksad) |
| 在URI中使用无效的PKey | 500 — “O5iRp40EGA”属性未知(请参阅“配置文件(nms:recipient)”架构的定义)。 XTK-170036无法解析表达式“@id = @O5iRp40EGA”。 | 404 — 无法解密PKey。 (PKey=@jksad)不支持的端点。 (endpoint=rest/profileAndServices/profile/@jksad) |
| 在URI和请求正文中使用两个不同的原始Pkey | 500 - RST-360011发生错误 — 请联系您的管理员。 RST-360012对资源“服务”的操作不一致 — 无法将键“SVC3”更新为“SVC4”。 | 500 — 发生错误 — 请联系您的管理员。 |
| 在URI中使用PKey，并在请求正文中使用其他原始PKey | 500 — 具有相同键“SVC4”的“服务”已存在。 PGS-220000 PostgreSQL错误：错误：重复的键值将违反唯一约束“nmsservice_name”。详细信息：键(sname)=(SVC4)已存在。 | 500 — 发生错误 — 请联系您的管理员。 |
| 在URI中使用不存在的原始ID | 404 - RST-360011发生错误 — 请联系您的管理员。 无法从键“adobe_nl：0”（模式为“service”且名称为“adobe_nl”的文档）找到路径为“Service”的文档 | 404 — 无法从键“adobe_nl”（模式为“service”且名称为“adobe_nl”的文档）找到路径为“Service”的文档 |
| 在请求正文中使用不存在的原始ID | 404 - RST-360011发生错误 — 请联系您的管理员。 无法从键“adobe_nl”中找到路径为“Service”的文档（架构为“service”且名称为“adobe_nl”的文档） | 404 — 无法从键“adobe_nl”（模式为“service”且名称为“adobe_nl”的文档）找到路径为“Service”的文档 |
| - | 500 - RST-360011发生错误 — 请联系您的管理员。 | 500 — 发生错误 — 请联系您的管理员。 |
| 插入具有无效性别（或任何）枚举值的配置文件/服务 | 500 - RST-360011发生错误 — 请联系您的管理员。 值“invalid”对于“@gender”字段的“nms:recipient:gender”枚举无效 | 500 — 发生错误 — 请联系您的管理员。 |

### 轮廓时区 {#profile-timezone}

使用Campaign Standard时，时区显示为&#x200B;**profileAndServices/profile** REST API调用的JSON响应的一部分。

使用Campaign v8时，时区仅作为&#x200B;**profileAndServicesExt/profile** REST API调用的一部分显示给用户。 它不是&#x200B;**profileAndServices/profile** REST API调用的一部分，因为它被添加到扩展架构中。

### 工作流外部信号 {#workflow-signals}

Campaign Standard Workflow GET API返回参数名称，例如工作流实例变量及其数据类型（布尔值、字符串等）。 当通过POST API调用触发信号时，可用于创建格式适当的JSON请求正文。

Campaign v8不支持广告工作流实例变量，但希望开发人员了解这些变量。 因此，在迁移后，需要构造POST请求正文中的参数信息，而没有GET API响应中的参数信息。
