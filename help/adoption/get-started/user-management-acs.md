---
title: 将技术用户迁移到Adobe Developer控制台
description: 了解如何将用户访问管理从Campaign Standard迁移到Campaign v8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 9354c07f173f67c23ce64e591f869bdd374c3334
workflow-type: tm+mt
source-wordcount: '1403'
ht-degree: 2%

---

# 从Campaign Standard到Campaign v8的用户访问管理 {#user-management-acs}

通过Adobe Campaign Standard和Adobe Campaign v8，用户可以定义和管理不同用户/操作员的权限。 这些权限包括授予用户访问产品各种功能的特定权限。 但是，这两种产品使用不同的方法和实施来管理用户访问权限。

Adobe Campaign Standard和Campaign v8中使用了以下概念来实现用户访问管理：

| Campaign Standard | Campaign v8 |
|---------|----------|
| 用户 | 操作员 |
| 角色 | 已命名权限 |
| 安全组 | 操作员组 |
| 组织实体 | 文件夹权限 |

## 从安全组到操作员组的迁移方法

>[!IMPORTANT]
>
>这些角色/已命名权限的功能在实施中可能有所不同，这可能会导致授权问题（例如，权限提升或功能中断）。 我们建议用户在转换后查看这些映射，以确保进行正确的访问控制。 [了解有关权限的详细信息](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

下表概述了从Adobe Campaign Standard过渡到Campaign v8时用户角色组的迁移方法。 在Campaign Standard中，**安全组**（在Campaign v8中称为&#x200B;**操作员组**）用于将一组角色分配给用户。 虽然某些安全组/操作员组是现成可用的，但如果需要，用户可以创建新组或修改现有组。

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **术语**  | 安全组 | 操作员组 |

在Adobe Campaign Standard和Campaign v8中，**安全组**&#x200B;和&#x200B;**操作员组**&#x200B;都映射到管理控制台中的产品配置文件。 如果要向用户分配&#x200B;**安全组**&#x200B;或&#x200B;**操作员组**，您可以在管理控制台中链接相应的&#x200B;**产品配置文件**。 此关联在用户登录时同步。 [了解有关产品配置文件的更多信息](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Campaign Standard安全组** | **Campaign v8操作员组** |
|----------|---------|
| 管理员 | 管理员 |
| 投放主管 | 管理员 |
| 工作流监督者 | 工作流监督者  |

## 从用户角色到已命名权限的迁移方法

>[!IMPORTANT]
>
>从Adobe Campaign Standard迁移到Campaign v8期间，具有&#x200B;**数据模型**&#x200B;角色但不具有&#x200B;**管理**&#x200B;角色的用户将自动获得&#x200B;**管理**&#x200B;访问权限，因为Campaign v8中的架构创建需要管理权限。 要防止出现这种情况，请在迁移之前删除其&#x200B;**数据模型**&#x200B;角色。

在Adobe Campaign Standard中，术语&#x200B;**用户角色**&#x200B;在Campaign v8中称为&#x200B;**Named right**。 下表概述了在Campaign v8中用于与Campaign Standard中的&#x200B;**用户角色**&#x200B;对应的&#x200B;**已命名权限**&#x200B;的术语。

| **Campaign Standard用户角色** | **Campaign v8命名权限** | **描述**  |
|----------|---------|---------|
| 管理 | 管理 | 具有管理权限的用户具有实例的完全访问权限。 |
| 数据模型  | 管理 | 有权运行发布和创建自定义资源。 管理员可以在Campaign v8中使用与架构创建相关的功能。  |
| 可投放性  | 管理  | 有权批准以前分析的投放。  |
| 导出 | 导出 | 导出数据的权限。  |
| 文件访问  | 文件访问  | 有权批准以前分析的投放。  |
| 一般导入  | 导入  | 通用数据导入权限 |
| 准备投放 | 准备投放 | 有权创建、修改、准备和删除投放。  |
| SQL脚本执行 | SQL脚本执行 | 有权直接在数据库上执行任何SQL命令。 |
| 开始投放  | 开始投放  | 有权批准以前分析的投放。  |
| 系统命令执行 | 项目执行 | 有权在服务器上执行系统命令。 |
| 工作流 | 工作流 | 有权管理工作流开始、停止、暂停等的执行。 |

## 组织单位的迁移方法

>[!IMPORTANT]
>
>Adobe Campaign Standard中没有作为直接或间接父项的&#x200B;**所有（所有）**的组织单位将不会迁移到Campaign v8。
>></br>
>>为多个安全组中的用户分配了最高级别安全组的组织单位。 如果多个组具有平行的顶级单位，则系统会为Campaign Standard中的用户选择组织单位，并且该用户只能访问系统选择的组织单位及其子级。 在迁移后的Campaign v8中，用户将有权访问&#x200B;**所有分配的组织单位及其子单位**，权限可能会不断提升。 要防止出现这种情况，请避免将用户分配给具有并行组织单位的安全组。 了解有关[并行组织单位分配](#parallel-assignments)的更多信息。


在Adobe Campaign Standard中，**组织单位**&#x200B;映射到Campaign v8中的现有&#x200B;**文件夹**&#x200B;层次结构模型，以维护类似的访问控制。 [了解有关文件夹管理的更多信息](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **术语**  | 组织实体 | 文件夹 |


### 关于并行组织单位分配 {#parallel-assignments}

当用户有权访问层次结构中单独分支中存在的多个单位（通过安全组分配）而没有权限访问公共父组织单位时，会发生并行组织单位分配。 这会在迁移期间造成安全风险。

例如，请考虑以下组织单位层次结构：

![并行组织单位分配示例图表](assets/do-not-localize/parallel-org-units-sample.png){width="50%" zoomable="yes"}

如果没有并行组织单位，任务将如下所示：

![没有并行组织单元示例图表](assets/do-not-localize/without-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

在此，用户有权访问组织单位A、A1和A2-1，所有这些都连接在父组织单位A下。用户可以访问A下的所有内容。

以下任务包含并行组织单位：

![使用并行组织单元示例图表](assets/do-not-localize/with-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

用户有权访问A1-1、A2和A2-1，它们存在于没有公共分配父项的单独分支中。


**安全影响**

* 在Campaign Standard中，系统会为用户选择一个顶级组织单位（A1-1或A2），并将访问权限限制为该单位及其子级。
* 迁移到Campaign V8后，用户将获得对所有已分配组织单位及其子单位的资源的访问权限。

**分辨率**

通过确保分配给用户的所有组织单位都归属于也分配给用户的单个、公共的父单位，可以解决并行组织单位分配问题。

下面列出了一些实现此目标的方法：

1. 删除对多个分支的访问权限：撤销对多个并行分支的访问权限，并确保所有访问权限都位于单个父级下。
1. 分配公共父项：授予包含所有所需访问点的相应公共父项组织单位的访问权限。
1. 重新构建层次结构：修改组织单元结构，将所有需要的访问权限置于单个分支下。

对于以上用户有权访问A1-1、A2和A2-1的示例，具体的分辨率步骤如下：

1. 删除对多个分支的访问权限：

   1. 撤销对A1-1的访问权限，仅保留对A2（包括A2-1）的访问权限，或者
   1. 撤销对A2和A2-1的访问权限，仅保留对A1-1的访问权限

1. 分配公共父级：

   1. 授予对组织单元A（A1-1和A2的共同父级）的访问权限，或者
   1. 授予对“全部”的访问权限，这将覆盖整个层次结构

1. 重新构建层次结构：

   1. 将A1-1移到A2下，或
   1. 将A2和A2-1移到A1-1下


## 从计划迁移方法

在Campaign v8中，**程序**&#x200B;表示为&#x200B;**文件夹**。 Campaign v8允许创建文件夹并允许限制对文件夹的访问。

通过使用&#x200B;**组**&#x200B;和&#x200B;**已命名的权限**，**操作员**&#x200B;可以被授予访问导航层次结构中的特定&#x200B;**文件夹**&#x200B;的权限，并且有权分配读取、写入和删除权限。 [了解有关文件夹管理的更多信息](https://experienceleague.adobe.com/zh-hans/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

由于&#x200B;**项目**&#x200B;在Campaign v8中视为&#x200B;**文件夹**，因此可以采用与任何其他文件夹相同的方式管理其访问权限。 迁移后，Campaign Standard管理员可以执行以下步骤：

1. 在资源管理器中，右键单击任意文件夹并选择&#x200B;**[!UICONTROL 属性……]**。

1. 导航到&#x200B;**[!UICONTROL 安全]**&#x200B;选项卡。

1. 根据所需的访问模型修改操作员组权限。 

## 用于访问REST API的产品配置文件映射 

要从Campaign v8中的执行实例访问事务性API，除&#x200B;**管理员**&#x200B;和&#x200B;**消息中心**&#x200B;产品配置文件之外，还需要新的&#x200B;**产品配置文件**。 此新&#x200B;**产品配置文件**&#x200B;将添加到Campaign Standard中的现有或预创建的技术帐户中。

迁移后，如果Campaign Standard用户不希望将其&#x200B;**技术帐户**&#x200B;关联到&#x200B;**管理员**&#x200B;产品配置文件，则应审查其&#x200B;**产品配置文件映射**&#x200B;并分配相应的&#x200B;**产品配置文件**。 对于未来的集成，我们建议在&#x200B;**REST URL**&#x200B;中使用Campaign v8 **租户ID**，而不是使用以前的Campaign Standard **租户ID**。

## 向Campaign Standard操作员迁移对内置Campaign资源的访问权限

从Campaign Standard迁移的操作员将拥有对Campaign v8中特定内置资源的读取权限。

## 未迁移的安全组和角色 {#non-migrated-groups-roles}

以下是尚未过渡的Campaign Standard角色列表：

* 默认中继帐户 

* 消息中心推送 

以下是尚未转换的Campaign Standard安全组映射列表。

* 消息中心代理

* 消息中心推送代理

* Adobe Experience Manager应用程序管理器

* 中继帐户

>[!NOTE]
>
>在Adobe Campaign Standard中创建并分配给用户的自定义角色将不会迁移到Adobe Campaign v8。
