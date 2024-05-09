---
audience: end-user
title: 使用Campaign中的AI助手发送短信
description: Campaign中的AI助手入门
badge: label="Beta 版"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 11%

---

# 使用 AI 助手生成短信 {#generative-sms}

>[!BEGINSHADEBOX]

**目录**

* [开始使用 AI 助手](generative-gs.md)
* [使用 AI 助手生成电子邮件](generative-content.md)
* 使用 AI 助手生成短信
* [使用 AI 助手生成推送通知](generative-push.md)

>[!ENDSHADEBOX]

一旦您根据受众定制和个性化短信消息后，借助Campaign中由创新的AI技术提供支持的AI助手，将您的通信提升到新的水平。

这款方便易用的工具提供了智能建议，可优化您的内容，确保您的消息有效地引起共鸣并最大限度地提高参与度。

>[!NOTE]
>
>在开始使用此功能之前，请阅读相关内容 [护栏和限制](generative-gs.md#generative-guardrails).

1. 创建和配置短信投放后，单击 **[!UICONTROL 编辑内容]**.

   有关如何配置短信投放的更多信息，请参阅 [此页面](../sms/create-sms.md).

1. 填写 **[!UICONTROL 基本详细信息]** 用于您的投放。 完成后，单击 **[!UICONTROL 编辑内容]**.

1. 根据需要个性化短信消息。 [了解详情](../sms/content-sms.md)

1. 访问 **[!UICONTROL 显示AI助手]** 菜单。

   ![](assets/sms-genai-1.png){zoomable=&quot;yes&quot;}

1. 启用 **[!UICONTROL 使用原始内容]** AI助手选项，用于根据投放、投放名称和所选受众来个性化新内容。

   >[!IMPORTANT]
   >
   > 您的提示必须始终与当前内容绑定。

1. 通过描述您要在 **[!UICONTROL 提示]** 字段。

   如果您在制作提示时需要帮助，请访问 **[!UICONTROL 提示库]** 其中提供了多种旨在改进交付的即时想法。

   ![](assets/sms-genai-2.png){zoomable=&quot;yes&quot;}

1. 选择 **[!UICONTROL 上传品牌资产]** 添加任何品牌资产，其中包含可为AI助手提供其他上下文的内容。

1. 使用不同的选项定制提示：

   * **[!UICONTROL 沟通策略]**：为生成的文本选择所需的通信方法。
   * **[!UICONTROL 语言]**：选择变体内容的语言。
   * **[!UICONTROL 色调]**：确保文本适合您的受众和用途。
   * **[!UICONTROL 长度]**：使用范围滑块选择内容的长度。

   ![](assets/sms-genai-3.png){zoomable=&quot;yes&quot;}

1. 提示就绪后，单击 **[!UICONTROL 生成]**.

1. 浏览生成的页面 **[!UICONTROL 变体]** 并单击 **[!UICONTROL 预览]** 以查看所选变体的全屏版本。

1. 导航至 **[!UICONTROL 优化]** 内的选项 **[!UICONTROL 预览]** 窗口访问其他自定义功能并微调变体到您的首选项：

   * **[!UICONTROL 用作参考内容]**：所选变量将用作生成其他结果的参考内容。

   * **[!UICONTROL 使用更简单的语言]**：AI助手帮助您编写每个人都能理解的清晰、简洁的消息。

   * **[!UICONTROL 重新短语]**：AI Assistant会重述您的消息，以使内容可吸引不同受众。

   ![](assets/sms-genai-4.png){zoomable=&quot;yes&quot;}

1. 单击 **[!UICONTROL 选择]** 找到相应的内容后。

1. 插入个性化字段，以根据用户档案数据自定义短信内容。 [详细了解内容个性化](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable=&quot;yes&quot;}

1. 定义消息内容后，单击 **[!UICONTROL 模拟内容]** 按钮来控制渲染，并使用测试用户档案检查个性化设置。 [了解详情](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable=&quot;yes&quot;}

定义内容、受众和计划后，便可以准备短信投放。 [了解详情](../monitor/prepare-send.md)
