---
audience: end-user
title: 验证事务型消息
description: 了解如何在Campaign Web用户界面中验证事务型消息
source-git-commit: e0d87d22d9712837f085f94f9d9ba63e96f36b36
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# 验证事务型消息

在创建事务型消息期间或之后，您可能需要使用数据示例验证内容。

## 模拟内容 {#simulate-content}

按照以下步骤模拟消息的内容：

* 确保消息内容中的个性化路径与上下文示例匹配。 在以下示例中，为了显示测试配置文件的名字，我们使用路径&#x200B;*rtEvent.ctx.basicDetails.firstName*

  您可以更改消息内容或上下文示例以使它们保持一致。

  ![](assets/validate-verification.png){zoomable="yes"}

* 单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮，使用在上下文示例中输入的数据预览事务型消息。

  ![](assets/validate-simulate.png){zoomable="yes"}

  检查内容后，单击&#x200B;**[!UICONTROL 关闭]**&#x200B;按钮。

* 如果您对内容进行了任何更改，请不要忘记单击&#x200B;**[!UICONTROL 重新发布]**&#x200B;按钮。

## 发送校样

如果要测试和体验通过所选渠道（如电子邮件、短信或推送通知）投放的事务型消息，则可以使用验证功能。

在[模拟内容窗口](#simulate-content)中，单击&#x200B;**[!UICONTROL 发送校样]**&#x200B;按钮。

![](assets/transactional-proof.png){zoomable="yes"}

在出现的新窗口中，输入要接收校样的电子邮件地址（或电话号码，具体取决于渠道）。 输入所需地址后，单击&#x200B;**[!UICONTROL 发送校样]**&#x200B;和&#x200B;**[!UICONTROL 确认]**&#x200B;按钮。 此操作允许您发送事务型消息的示例，确保所有个性化、动态内容和格式正确显示，就像最终用户所做的那样。

![](assets/transactional-sendproof.png){zoomable="yes"}

这是在发布事务型消息之前识别任何潜在问题的关键步骤。
