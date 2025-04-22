---
audience: end-user
title: 使用AI助手推送通知
description: AI助手入门
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# 使用AI助手生成推送通知 {#generative-push}

>[!IMPORTANT]
>
>在开始使用此功能之前，请阅读相关的[护栏和限制](generative-gs.md#generative-guardrails)。
></br>
>
>在Adobe Campaign Web中使用AI助手之前，必须同意[用户协议](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。 有关更多信息，请与您的 Adobe 代表联系。

AI Assistant通过建议与受众产生共鸣的不同内容，帮助优化投放的影响。

在以下示例中，利用AI Assistant来制作引人注目的消息，以创建更具吸引力的客户体验。

1. 创建和配置推送通知投放后，单击&#x200B;**[!UICONTROL 编辑内容]**。

   有关配置推送投放的详细信息，请参阅[此页面](../push/create-push.md)。

1. 访问&#x200B;**[!UICONTROL 显示AI助手]**&#x200B;菜单。

   ![显示“显示AI助手”菜单的屏幕快照](assets/push-genai-1.png){zoomable="yes"}

1. 为AI助手启用&#x200B;**[!UICONTROL 使用原始内容]**&#x200B;选项，以根据所选内容对新内容进行个性化设置。

1. 通过描述您要在&#x200B;**[!UICONTROL 提示]**&#x200B;字段中生成的内容，微调内容。

   如果创作提示时需要帮助，请访问&#x200B;**[!UICONTROL 提示库]**，该库提供了多种提示想法以改进投放。

   ![显示提示库界面的屏幕截图](assets/push-genai-2.png){zoomable="yes"}

1. 选择要生成的字段： **[!UICONTROL 标题]**、**[!UICONTROL 消息]**&#x200B;和/或&#x200B;**[!UICONTROL 图像]**。

1. 使用&#x200B;**[!UICONTROL 文本设置]**&#x200B;选项定制提示：

   * **[!UICONTROL 通信策略]**：为生成的文本选择最合适的通信样式。
   * **[!UICONTROL 音调]**：调整电子邮件的音调以便与受众产生共鸣。 无论您想听起信息性、娱乐性还是说服力，AI Assistant都会相应地调整消息。

   ![显示文本设置选项的屏幕快照](assets/push-genai-3.png){zoomable="yes"}

1. 选择您的&#x200B;**[!UICONTROL 图像设置]**：

   * **[!UICONTROL 内容类型]**：对可视元素的性质进行分类，区分不同的可视表示形式，如照片、图形或艺术品。
   * **[!UICONTROL 视觉强度]**：通过调整图像的强度来控制其影响。 较低的设置(2)产生更柔和、更受限的外观，而较高的设置(10)使图像更生动且视觉更强大。
   * **[!UICONTROL 光源]**：调整图像中的光源以调整其大气形状并突出显示特定元素。
   * **[!UICONTROL 合成]**：在图像的框架中排列元素。

   ![显示图像设置选项的屏幕快照](assets/push-genai-4.png){zoomable="yes"}

1. 从&#x200B;**[!UICONTROL 品牌资产]**&#x200B;菜单中，单击&#x200B;**[!UICONTROL 上传品牌资产]**&#x200B;以添加任何包含向AI助手提供其他上下文的内容的品牌资产，或选择以前上传的品牌资产。

   以前上传的文件在&#x200B;**[!UICONTROL 已上传的品牌资产]**&#x200B;下拉菜单中可用。 切换要包含在生成中的资产。

1. 提示就绪后，单击&#x200B;**[!UICONTROL 生成]**。

1. 浏览生成的&#x200B;**[!UICONTROL 变体]**&#x200B;并单击&#x200B;**[!UICONTROL 预览]**&#x200B;以查看所选变体的全屏版本。

1. 导航到&#x200B;**[!UICONTROL 预览]**&#x200B;窗口中的&#x200B;**[!UICONTROL 优化]**&#x200B;选项以访问其他自定义功能：

   * **[!UICONTROL 用作引用内容]**：将所选变量用作用于生成其他结果的引用内容。
   * **[!UICONTROL 重述]**：以不同的方式重述您的消息，以使您的写作保持新鲜，并吸引不同的受众。
   * **[!UICONTROL 使用更简单的语言]**：简化您的语言，确保更广大的受众能够清晰地访问这些内容。

   您还可以更改文本的&#x200B;**[!UICONTROL 音调]**&#x200B;和&#x200B;**[!UICONTROL 通信策略]**。

   ![显示优化选项的屏幕快照](assets/push-genai-5.png){zoomable="yes"}

1. 找到相应的内容后，单击&#x200B;**[!UICONTROL 选择]**。

1. 插入个性化字段，以根据用户档案数据自定义电子邮件内容。 然后，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以控制渲染并检查测试用户档案的个性化设置。 [了解详情](../preview-test/preview-content.md)

   ![显示“模拟内容”按钮的屏幕快照](assets/push-genai-6.png){zoomable="yes"}

在定义内容、受众和计划时，准备推送投放。 [了解详情](../monitor/prepare-send.md)