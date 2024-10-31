---
audience: end-user
title: 事务性消息传递
description: 关于使用Adobe Campaign Web进行事务性消息传递
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 3%

---

# 关于事务型消息传递 {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="事务性消息传递"
>abstract="事务性消息传递是Adobe Campaign中用于处理触发消息的专用模块。"

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="事务性消息传递"
>abstract="事务性消息传递是Adobe Campaign中用于处理触发消息的专用模块。 这些消息是响应来自信息系统的事件自动生成的。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hans" text="请参阅发行说明"

<!-- >>[!CONTEXTUALHELP]
>id="acw_transacmessages_exclusionlogs"
>title="Transactional messaging exclusion logs"
>abstract="Transactional messaging exclusion logs" -->

事务性消息传递是Adobe Campaign中用于处理触发消息的专用模块。 这些消息是响应来自信息系统的事件自动生成的。 此类事件的常见示例包括单击按钮或链接、放弃购买、请求产品可用性警报、创建或修改帐户等。

事务型消息用于发送：

* 重要通知，例如订单确认或密码重置，
* 对客户操作（如帐户创建、购买完成）的实时响应，
* 对客户互动至关重要的非促销内容。

事务性消息传递模块与您的信息系统无缝集成。 事件（如客户操作）将推送到Adobe Campaign，以发送相应的个性化消息。 这些消息可以通过电子邮件、短信或推送通知等各种渠道单独或批量发送。

您可以在&#x200B;**[!UICONTROL 触发的消息]**&#x200B;部分找到&#x200B;**[!UICONTROL 事务型消息]**&#x200B;模块。

![](assets/transactional.png){zoomable="yes"}

**[!UICONTROL 事务型消息]**&#x200B;页面中有3个选项卡：

* **[!UICONTROL 浏览]**，您可在其中找到事务型消息的列表及其状态，
* **[!UICONTROL 模板]**，您可以在其中查找和创建事务性消息模板，
* **[!UICONTROL History]**，其中包含有关已执行的所有事务型消息的详细信息。

在本文档中了解如何：

* [在模板的帮助下创建事务性消息](create-transactional.md)，并了解所需的设置，
* [验证事务性消息的内容](validate-transactional.md)并模拟个性化，
* [监视事务性消息](monitor-transactional.md)。
