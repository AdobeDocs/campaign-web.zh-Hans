---
audience: end-user
title: 使用Campaign中的AI助手推送通知
description: Campaign中的AI助手入门
badge: label="Beta 版"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 8%

---

# 使用 AI 助手生成推送通知 {#generative-push}

>[!BEGINSHADEBOX]

**目录**

* [开始使用 AI 助手](generative-gs.md)
* [使用 AI 助手生成电子邮件](generative-content.md)
* [使用 AI 助手生成短信](generative-sms.md)
* 使用 AI 助手生成推送通知

>[!ENDSHADEBOX]

AI Assistant可以通过建议更可能引起受众共鸣的不同内容来帮助您优化投放的影响。

>[!NOTE]
>
>在开始使用此功能之前，请阅读相关的[护栏和限制](generative-gs.md#generative-guardrails)。

在以下示例中，我们将利用AI助手制作引人入胜的消息来打造更引人入胜的客户体验。

1. 创建和配置推送通知投放后，单击&#x200B;**[!UICONTROL 编辑内容]**。

   有关如何配置推送投放的详细信息，请参阅[此页面](../push/create-push.md)。

1. 填写投放的&#x200B;**[!UICONTROL 基本详细信息]**。 完成后，单击&#x200B;**[!UICONTROL 编辑内容]**。

1. 根据需要个性化您的推送通知。 [了解详情](../push/content-push.md)

1. 访问&#x200B;**[!UICONTROL 显示AI助手]**&#x200B;菜单。

   ![](assets/push-genai-1.png){zoomable="yes"}

1. 为AI助手启用&#x200B;**[!UICONTROL 使用原始内容]**&#x200B;选项，以根据您的投放、投放名称和所选受众来个性化新内容。

   >[!IMPORTANT]
   >
   > 您的提示必须始终与当前内容绑定。

   ![](assets/push-genai-3.png){zoomable="yes"}

1. 通过描述要在&#x200B;**[!UICONTROL 提示]**&#x200B;字段中生成的内容，优化内容。

   如果您在制作提示时寻求帮助，请访问&#x200B;**[!UICONTROL 提示库]**，该库提供各种提示想法以改进投放。

   ![](assets/push-genai-2.png){zoomable="yes"}

1. 选择&#x200B;**[!UICONTROL 上载品牌资产]**&#x200B;可添加任何包含可为AI助手提供其他上下文的内容的品牌资产。

1. 选择要生成的字段：**[!UICONTROL 标题]**、**[!UICONTROL 子标题]**&#x200B;或&#x200B;**[!UICONTROL 消息]**。

1. 使用不同的选项定制提示：

   * **[!UICONTROL 通信策略]**：为生成的文本选择最合适的通信样式。
   * **[!UICONTROL 语言]**：选择您希望生成内容的语言。
   * **[!UICONTROL 音调]**：您电子邮件的音调应该引起您的听众的共鸣。 无论您是要提供信息、好玩还是具有说服力，AI Assistant都可以相应地调整消息。

   ![](assets/push-genai-4.png){zoomable="yes"}

1. 提示就绪后，单击&#x200B;**[!UICONTROL 生成]**。

1. 浏览生成的&#x200B;**[!UICONTROL 变体]**&#x200B;并单击&#x200B;**[!UICONTROL 预览]**&#x200B;以查看所选变体的全屏版本。

1. 导航到&#x200B;**[!UICONTROL 预览]**&#x200B;窗口中的&#x200B;**[!UICONTROL 优化]**&#x200B;选项以访问其他自定义功能：

   * **[!UICONTROL 用作引用内容]**：所选变量将用作用于生成其他结果的引用内容。

   * **[!UICONTROL 改写]**： AI助手可以通过不同方式改写您的消息，使您的写作保持新鲜，并吸引各种受众。

   * **[!UICONTROL 使用更简单的语言]**：利用AI Assistant简化您的语言，确保更广大的受众拥有清晰易懂的语言。

   ![](assets/push-genai-5.png){zoomable="yes"}

1. 找到相应的内容后，单击&#x200B;**[!UICONTROL 选择]**。

1. 插入个性化字段，以根据用户档案数据自定义电子邮件内容。 然后，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以控制渲染，并使用测试配置文件检查个性化设置。 [了解详情](../preview-test/preview-content.md)

   ![](assets/push-genai-6.png){zoomable="yes"}

定义内容、受众和计划后，便可以准备推送投放。 [了解详情](../monitor/prepare-send.md)

