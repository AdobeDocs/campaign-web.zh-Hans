---
audience: end-user
title: 使用陷阱组
hide: true
hidefromtoc: true
description: 了解如何在Campaign Web用户界面中使用陷阱组进行投放
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# 使用 **[!UICONTROL 陷阱组]** {#trap-group}

A **[!UICONTROL 陷阱组]** 用于定位不符合所规定目标标准的收件人。 这样，超出投放范围的收件人可以像任何其他目标收件人一样接收投放。
A **[!UICONTROL 陷阱组]** 是一组 **[!UICONTROL 种子地址]**.

## 为何使用 **[!UICONTROL 陷阱组]**

您可以使用 **[!UICONTROL 陷阱组]** ：

1. **作为证明** ：每个成员 **[!UICONTROL 陷阱组]** 将接收投放，就像他们属于受众一样。


1. **保护您的邮件列表** ：通过接收受众将收到的内容，每个 **[!UICONTROL 种子地址]** 的 **[!UICONTROL 陷阱组]** 如果第三方使用邮件列表，则会引起注意。

## 关于 **[!UICONTROL 陷阱组]**

系统会自动从以下投放统计信息的报表中排除种子地址： **点击次数**， **打开次数**， **取消订阅**. 这些报表只涉及真实受众。

对于电子邮件投放，只需要电子邮件地址 **[!UICONTROL 陷阱组]**，Campaign将随机填充其他字段的个性化设置。

## 如何设置 **[!UICONTROL 陷阱组]** 在投放中

要设置 **[!UICONTROL 陷阱组]**，转到 **[!UICONTROL 受众]** 投放设置。 您将有2个选项：
- [选择测试配置文件](#select-test-profile)
- [创建条件](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### 选择测试配置文件 {#select-test-profiles}

选择“选择测试用户档案”时，您将具有如下窗口，邀请您访问 **[!UICONTROL 添加测试配置文件]** ：

![](assets/trap-no-test-profile.png){zoomable="yes"}

单击按钮后，您将有权访问可以添加 **[!UICONTROL 陷阱组]**. 选中要使用的项。
您可以创建新的种子地址。 [了解更多信息](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

确认陷阱地址后，请检查下方的号码是否正确 **[!UICONTROL 陷阱组]**.

![](assets/trap-check.png){zoomable="yes"}

### 创建条件 {#create-condition}

使用 **[!UICONTROL 创建条件]** 选项，您将获得一个新窗口，可以在其中自定义查询以定义要使用的种子地址：

![](assets/trap-create-condition.png){zoomable="yes"}

您的查询将显示在 **[!UICONTROL 陷阱组]**.

![](assets/trap-custom.png){zoomable="yes"}

## 如何新建 **[!UICONTROL 种子地址]** {#create-seed}

您可以创建新的 **[!UICONTROL 种子地址]** 在 **[!UICONTROL 资源管理器]** > **[!UICONTROL 资源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 种子成员]**

![](assets/trap-create.png){zoomable="yes"}

您可以填写有关种子成员的所有详细信息，就像它是一个受众配置文件一样：

![](assets/trap-create-contact.png){zoomable="yes"}