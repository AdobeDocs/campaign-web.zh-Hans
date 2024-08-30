---
audience: end-user
title: 投放警报
description: 了解如何使用投放警报。
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 39dcf11797339ee9800da6c5a32b1a1c3470529a
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 19%

---

# 开始使用投放警报 {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="投放警报"
>abstract="投放警报现已在 Campaign 中推出。此功能是一个警报管理系统，利用该系统可让用户组自动接收包含其投放执行信息的电子邮件通知。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

投放警报功能是一个警报管理系统，利用该系统可让用户组自动接收包含其投放执行信息的电子邮件通知。收件人可以监控Adobe Campaign处理的持续投放，并在出现问题时采取适当措施。

可根据Adobe Campaign Web用户界面定义的特定警报条件自定义通知。

有关如何管理投放失败的更多信息，请参阅[Adobe Campaign v8 （控制台）文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## 电子邮件通知内容 {#content}

电子邮件通知包含以下部分：

* **摘要**：显示符合您定义的条件的投放数量，以及每个条件的标签和颜色。
* **详细信息**：列出仪表板的所有已定义投放标准以及每个标准的相应投放。

![](assets/alerting-email.png)

## 设置投放警报 {#set-up}

为帮助您设置这些警报，Campaign Web用户界面允许您创建和管理：

* **投放警报仪表板**：指定收件人，设置要包含在仪表板中的警报条件，并访问已发送警报的历史记录。 [了解如何使用仪表板](../msg/delivery-alerting-dashboards.md)
* **投放警报标准**： Campaign Web用户界面提供了预定义警报标准（吞吐量低的投放，准备失败的投放……），您可以将这些标准添加到仪表板。 您也可以根据自己的需求创建自己的标准。 [了解如何使用标准](../msg/delivery-alerting-criteria.md)

假设您只想将失败的投放通知给具有管理权限的用户，并将软退回错误率较高的投放通知给营销用户。 要实现此目的，请为每个收件人组创建两个包含相应标准的单独功能板。

>[!NOTE]
>
>要访问和配置功能板和警报条件，您必须具有&#x200B;**管理权限**&#x200B;或是&#x200B;**投放主管**&#x200B;安全组的成员。 标准用户无法访问Adobe Campaign界面中的仪表板，但会收到警报通知。 [了解有关访问和权限的更多信息](../get-started/permissions.md)
