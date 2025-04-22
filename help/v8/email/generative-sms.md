---
audience: end-user
title: 带有AI助理的短信
description: AI助手入门
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 2%

---

# 使用AI助手生成短信 {#generative-sms}

>[!IMPORTANT]
>
>在开始使用此功能之前，请阅读相关的[护栏和限制](generative-gs.md#generative-guardrails)。
></br>
>
>在Adobe Campaign Web中使用AI助手之前，必须同意[用户协议](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。 有关更多信息，请与您的 Adobe 代表联系。

一旦您制作并个性化短信消息以适合受众，即可借助创新的AI技术，提升Adobe Campaign Web中的AI助手与您的通信。

此工具提供了智能建议，可优化您的内容，确保您的消息有效地引起共鸣并最大限度地提高参与度。

>[!BEGINTABS]

>[!TAB 完整短信生成]

1. 创建和配置短信投放后，单击&#x200B;**[!UICONTROL 编辑内容]**。

   有关配置短信投放的详细信息，请参阅[此页面](../sms/create-sms.md)。

1. 填写投放的&#x200B;**[!UICONTROL 基本详细信息]**。 完成后，单击&#x200B;**[!UICONTROL 编辑内容]**。

1. 访问&#x200B;**[!UICONTROL 显示AI助手]**&#x200B;菜单。

   ![显示“显示AI助手”菜单的屏幕快照](assets/sms-genai-1.png){zoomable="yes"}

1. 通过描述您要在&#x200B;**[!UICONTROL 提示]**&#x200B;字段中生成的内容，微调内容。

   如果您在编写提示时需要帮助，请访问&#x200B;**[!UICONTROL 提示库]**，该库提供了多种提示想法以改进投放。

   ![显示提示库的屏幕截图](assets/sms-genai-2.png){zoomable="yes"}

1. 使用&#x200B;**[!UICONTROL 文本设置]**&#x200B;选项定制提示：

   * **[!UICONTROL 通信策略]**：为生成的文本选择最合适的通信样式。
   * **[!UICONTROL 音调]**：确保您的电子邮件音调可与您的受众引起共鸣。 无论您想听起信息性、娱乐性还是说服力，AI Assistant都会相应地调整消息。
   * **文本长度**：使用滑块选择所需文本长度。

   ![显示文本设置选项的屏幕快照](assets/sms-genai-3.png){zoomable="yes"}

1. 从&#x200B;**[!UICONTROL 品牌资产]**&#x200B;菜单中，单击&#x200B;**[!UICONTROL 上传品牌资产]**&#x200B;以添加任何包含向AI助手提供其他上下文的内容的品牌资产，或选择以前上传的品牌资产。

   以前上传的文件在&#x200B;**[!UICONTROL 已上传的品牌资产]**&#x200B;下拉菜单中可用。 切换要包含在生成中的资产。

1. 提示就绪后，单击&#x200B;**[!UICONTROL 生成]**。

1. 浏览生成的&#x200B;**[!UICONTROL 变体]**&#x200B;并单击&#x200B;**[!UICONTROL 预览]**&#x200B;以查看所选变体的全屏版本。

   ![显示生成的变体的屏幕截图](assets/sms-genai-4.png){zoomable="yes"}

1. 导航到&#x200B;**[!UICONTROL 预览]**&#x200B;窗口中的&#x200B;**[!UICONTROL 优化]**&#x200B;选项以访问其他自定义功能并微调您的首选项变量：

   * **[!UICONTROL 用作引用内容]**：所选变量用作用于生成其他结果的引用内容。
   * **[!UICONTROL 使用更简单的语言]**： AI Assistant可帮助您编写所有人都能理解的清晰、简洁的消息。
   * **[!UICONTROL 改写]**： AI Assistant将改写您的消息以使其可吸引不同受众。

   您还可以更改文本的&#x200B;**[!UICONTROL 音调]**&#x200B;和&#x200B;**[!UICONTROL 通信策略]**。

   ![显示细化选项的屏幕快照](assets/sms-genai-5.png){zoomable="yes"}

1. 找到相应的内容后，单击&#x200B;**[!UICONTROL 选择]**。

1. 插入个性化字段以根据用户档案数据自定义短信内容。 [了解有关内容个性化的更多信息](../personalization/personalize.md)。

   ![显示个性化字段的屏幕截图](assets/sms-genai-5.png){zoomable="yes"}

1. 定义消息内容后，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以控制渲染并使用测试用户档案检查个性化设置。 [了解详情](../preview-test/preview-content.md)。

   ![显示内容模拟的屏幕截图](assets/sms-genai-6.png){zoomable="yes"}

在定义内容、受众和计划时，准备短信投放。 [了解详情](../monitor/prepare-send.md)。

>[!TAB 纯文本生成]

1. 创建和配置短信投放后，单击&#x200B;**[!UICONTROL 编辑内容]**。

   有关配置短信投放的详细信息，请参阅[此页面](../sms/create-sms.md)。

1. 填写投放的&#x200B;**[!UICONTROL 基本详细信息]**。 完成后，单击&#x200B;**[!UICONTROL 编辑内容]**。

1. 根据需要个性化短信消息。 [了解详情](../sms/content-sms.md)。

1. 访问&#x200B;**[!UICONTROL 消息]**&#x200B;字段旁边的&#x200B;**[!UICONTROL AI助手]**&#x200B;菜单。

   ![显示AI助手菜单的屏幕截图](assets/sms-text-1.png){zoomable="yes"}

1. 为AI助手启用&#x200B;**[!UICONTROL 使用引用内容]**&#x200B;选项，以根据所选内容对新内容进行个性化设置。

1. 通过描述您要在&#x200B;**[!UICONTROL 提示]**&#x200B;字段中生成的内容，微调内容。

   如果您在创作提示时需要帮助，请访问&#x200B;**[!UICONTROL 提示库]**，该库提供了多种提示想法以改进您的营销活动。

   ![显示提示库的屏幕快照](assets/sms-text-2.png){zoomable="yes"}

1. 使用&#x200B;**[!UICONTROL 文本设置]**&#x200B;选项定制提示：

   * **[!UICONTROL 通信策略]**：为生成的文本选择所需的通信方法。
   * **[!UICONTROL 语言]**：选择变体内容的语言。
   * **[!UICONTROL 色调]**：确保文本适合您的受众和用途。
   * **[!UICONTROL 长度]**：使用范围滑块选择内容的长度。

   ![显示文本设置选项的屏幕快照](assets/sms-text-3.png){zoomable="yes"}

1. 从&#x200B;**[!UICONTROL 品牌资产]**&#x200B;菜单中，单击&#x200B;**[!UICONTROL 上传品牌资产]**&#x200B;以添加任何包含向AI助手提供其他上下文的内容的品牌资产，或选择以前上传的品牌资产。

   以前上传的文件在&#x200B;**[!UICONTROL 已上传的品牌资产]**&#x200B;下拉菜单中可用。 切换要包含在生成中的资产。

1. 提示就绪后，单击&#x200B;**[!UICONTROL 生成]**。

1. 浏览生成的&#x200B;**[!UICONTROL 变体]**&#x200B;并单击&#x200B;**[!UICONTROL 预览]**&#x200B;以查看所选变体的全屏版本。

1. 导航到&#x200B;**[!UICONTROL 预览]**&#x200B;窗口中的&#x200B;**[!UICONTROL 优化]**&#x200B;选项以访问其他自定义功能并微调您的首选项变量：

   * **[!UICONTROL 用作引用内容]**：所选变量用作用于生成其他结果的引用内容。
   * **[!UICONTROL 重述]**： AI助手可以通过不同方式重述您的消息，使您的写作保持新鲜，并吸引各种受众。
   * **[!UICONTROL 使用更简单的语言]**：利用AI Assistant简化您的语言，确保为更广泛的受众提供清晰易懂的语言。

   您还可以更改文本的&#x200B;**[!UICONTROL 音调]**&#x200B;和&#x200B;**[!UICONTROL 通信策略]**。

   ![显示细化选项的屏幕快照](assets/sms-text-4.png){zoomable="yes"}

1. 找到相应的内容后，单击&#x200B;**[!UICONTROL 选择]**。

1. 插入个性化字段以根据用户档案数据自定义短信内容。 [了解有关内容个性化的更多信息](../personalization/personalize.md)。

1. 定义消息内容后，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以控制渲染并使用测试用户档案检查个性化设置。 [了解详情](../preview-test/preview-content.md)。

   ![显示内容模拟的屏幕截图](assets/sms-text-5.png){zoomable="yes"}

在定义内容、受众和计划时，准备短信投放。 [了解详情](../monitor/prepare-send.md)。

>[!ENDTABS]