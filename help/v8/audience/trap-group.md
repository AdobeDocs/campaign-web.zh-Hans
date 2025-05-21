---
audience: end-user
title: 使用陷印组
description: 了解如何在Campaign Web用户界面中使用陷阱组进行投放
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 4%

---

# 使用陷印组 {#trap-group}

**[!UICONTROL 陷阱组]**（也称为&#x200B;**[!UICONTROL 种子列表]**）用于在投放中包含特定地址，以通过定向不符合定义的目标条件的用户档案来监视和验证分发过程。 这样，投放范围外的收件人可以像任何其他目标收件人一样接收投放。

**[!UICONTROL 陷阱组]**&#x200B;是Campaign Web用户界面上名为&#x200B;**[!UICONTROL 测试配置文件]**&#x200B;的一组&#x200B;**[!UICONTROL 种子地址]**。

## 为何使用陷阱组 {#why-trap-group}

您可以使用&#x200B;**[!UICONTROL 陷阱组]**：

1. **作为证明**： **[!UICONTROL 陷阱组]**&#x200B;的每个成员都像受众的一部分一样接收投放。

1. **为了保护您的邮件列表**：如果邮件列表由第三方使用，通过接收受众将收到的内容，将注意到&#x200B;**[!UICONTROL 陷阱组]**&#x200B;的每个&#x200B;**[!UICONTROL 测试配置文件]**。

>[!NOTE]
>
>除了在创建投放[&#128279;](../email/create-email.md#preview-test)期间和从[控制组](control-group.md)中发送验证外，添加陷阱组也是测试受众的好方法。

## 关于陷阱组 {#about-trap-group}

测试配置文件自动从有关以下投放统计信息的报告中排除：**点击次数**、**打开次数**、**取消订阅**。 报表仅关注真实受众。

对于电子邮件投放，**[!UICONTROL 陷阱组]**&#x200B;只需要电子邮件地址。 Campaign会随机填充其他字段的个性化设置。

## 在投放中添加陷阱组 {#trap-group-in-delivery}

要设置&#x200B;**[!UICONTROL 陷阱组]**，请转到投放的&#x200B;**[!UICONTROL 受众]**&#x200B;设置。 您将有两个选项：

* [选择测试轮廓](#select-test-profiles)
* [创建条件](#create-condition)

[陷阱组设置界面屏幕截图](assets/trap-group.png){zoomable="yes"}

### 选择测试轮廓 {#select-test-profiles}

选择&#x200B;**选择测试配置文件**&#x200B;时，请使用&#x200B;**添加测试配置文件**&#x200B;按钮，如下所示：

[添加测试配置文件按钮屏幕截图](assets/trap-no-test-profile.png){zoomable="yes"}

单击该按钮后，您可以访问要添加到&#x200B;**[!UICONTROL 陷阱组]**&#x200B;的测试配置文件。 选择您要使用的库。

您还可以创建新的测试用户档案。 [了解详情](#create-seed)

[选择测试配置文件界面截图](assets/trap-select-test-profiles.png){zoomable="yes"}

确认测试配置文件后，检查&#x200B;**[!UICONTROL 陷阱组]**&#x200B;下是否显示正确的编号。

[陷阱组确认屏幕快照](assets/trap-check.png){zoomable="yes"}

### 创建条件 {#create-condition}

使用&#x200B;**[!UICONTROL 创建条件]**&#x200B;选项，创建查询以定义要使用的测试用户档案：

[创建条件接口屏幕截图](assets/trap-create-condition.png){zoomable="yes"}

您的查询显示在&#x200B;**[!UICONTROL 陷阱组]**&#x200B;下。

[陷阱组查询显示屏幕截图](assets/trap-custom.png){zoomable="yes"}

## 创建新的测试配置文件 {#create-seed}

您可以从&#x200B;**[!UICONTROL 资源管理器]** > **[!UICONTROL 资源]** > **[!UICONTROL 促销活动管理]** > **[!UICONTROL 种子成员]**&#x200B;文件夹创建新的&#x200B;**[!UICONTROL 测试配置文件]**。

[创建测试配置文件导航屏幕截图](assets/trap-create.png){zoomable="yes"}

配置&#x200B;**[!UICONTROL 测试配置文件]**&#x200B;的所有设置，就像配置任何配置文件一样：

[测试配置文件配置屏幕截图](assets/trap-create-contact.png){zoomable="yes"}