---
audience: end-user
title: 使用陷阱组
hide: true
hidefromtoc: true
description: 了解如何在Campaign Web用户界面中使用陷阱组进行投放
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# 使用&#x200B;**[!UICONTROL 陷阱组]** {#trap-group}

**[!UICONTROL 陷阱组]**（也称为&#x200B;**[!UICONTROL 种子列表]**）用于在投放中包含特定地址，以通过定向不符合定义的目标条件的用户档案来监视和验证分发过程。 这样，超出投放范围的收件人可以像任何其他目标收件人一样接收投放。
**[!UICONTROL 陷阱组]**&#x200B;是AC Web UI上名为&#x200B;**[!UICONTROL 测试配置文件]**&#x200B;的一组&#x200B;**[!UICONTROL 种子地址]**。

## 为何使用&#x200B;**[!UICONTROL 陷阱组]**

您可以使用&#x200B;**[!UICONTROL 陷阱组]** ：

1. **作为证明** ： **[!UICONTROL 陷阱组]**&#x200B;的每个成员都将收到投放，就像他们属于受众一样。


1. **为了保护您的邮件列表** ：通过接收受众将收到的内容，如果邮件列表由第三方使用，将注意到&#x200B;**[!UICONTROL 陷阱组]**&#x200B;的每个&#x200B;**[!UICONTROL 测试配置文件]**。

>[!NOTE]
>
>陷阱组与创建投放](../email/create-email.md#preview-test)期间发送验证的[不同，并且与[控制组](control-group.md)不同。


## 关于&#x200B;**[!UICONTROL 陷阱组]**

测试配置文件自动从有关以下投放统计信息的报告中排除：**点击次数**、**打开次数**、**取消订阅**。 这些报表只涉及真实受众。

对于电子邮件投放，**[!UICONTROL 陷阱组]**&#x200B;只需要电子邮件地址，Campaign将随机填充其他字段的个性化设置。

## 如何在投放中设置&#x200B;**[!UICONTROL 陷阱组]**

要设置&#x200B;**[!UICONTROL 陷阱组]**，请转到投放的&#x200B;**[!UICONTROL 受众]**&#x200B;设置。 您将有2个选项：
- [选择测试配置文件](#select-test-profile)
- [创建条件](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### 选择测试配置文件 {#select-test-profiles}

选择“选择测试配置文件”时，您将具有如下窗口，邀请您&#x200B;**[!UICONTROL 添加测试配置文件]** ：

![](assets/trap-no-test-profile.png){zoomable="yes"}

单击该按钮后，您将有权访问可添加&#x200B;**[!UICONTROL 陷阱组]**的测试配置文件。 选中要使用的项。
您可以创建新的测试用户档案。 [了解详情](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

当您确认测试配置文件时，请检查您在&#x200B;**[!UICONTROL 陷阱组]**&#x200B;下是否具有正确的编号。

![](assets/trap-check.png){zoomable="yes"}

### 创建条件 {#create-condition}

通过&#x200B;**[!UICONTROL 创建条件]**&#x200B;选项，您将获得一个新窗口，您可以在其中自定义查询以定义要使用的测试用户档案：

![](assets/trap-create-condition.png){zoomable="yes"}

您的查询将显示在&#x200B;**[!UICONTROL 陷阱组]**&#x200B;下。

![](assets/trap-custom.png){zoomable="yes"}

## 如何创建新的&#x200B;**[!UICONTROL 测试配置文件]** {#create-seed}

您可以在&#x200B;**[!UICONTROL 资源管理器]** > **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子成员]**&#x200B;中创建新的&#x200B;**[!UICONTROL 测试配置文件]**

![](assets/trap-create.png){zoomable="yes"}

您可以填写有关&#x200B;**[!UICONTROL 测试配置文件]**&#x200B;的所有详细信息，就像它是一个受众配置文件一样：

![](assets/trap-create-contact.png){zoomable="yes"}