---
audience: end-user
title: 创新型内容
description: 了解如何使用AI助手生成图像
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 2%

---

# 使用AI助手生成图像 {#generative-image}

>[!IMPORTANT]
>
>在开始使用此功能之前，请阅读相关的[护栏和限制](generative-gs.md#generative-guardrails)。
></br>
>
>在Adobe Campaign Web中使用AI助手之前，必须同意[用户协议](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}。 有关更多信息，请与您的 Adobe 代表联系。

使用Adobe Campaign Web中的AI助手创建引人注目的可视内容，以增强跨电子邮件、登陆页和推送通知的消息。 AI Assistant可帮助您生成和优化图像，确保您的内容在视觉上吸引人并与您的品牌保持一致。

## 用于电子邮件和登陆页面 {#email-web-channels}

AI助手可以为您的电子邮件投放和登陆页面生成完整的可视化体验。 此功能允许您制作品牌上吸引眼球的图像，从而在数字接触点上与受众产生共鸣。

### 访问和配置 {#access-configure}

要开始使用AI助手生成图像，请首先设置投放并打开内容编辑器。 执行以下步骤以准备工作区并访问AI助手面板。

1. 创建和配置投放：

   * **电子邮件**：创建和配置电子邮件投放后，单击&#x200B;**[!UICONTROL 编辑内容]**。 [了解详情](../email/create-email-content.md)
   * **登陆页面**：创建和配置登陆页面后，单击&#x200B;**[!UICONTROL 编辑内容]**。 [了解详情](../landing-pages/create-lp.md)

1. 选择要使用AI助手更改的资产，并访问&#x200B;**[!UICONTROL AI助手]**&#x200B;菜单。

   ![显示Adobe Campaign Web中的文本组件选择的屏幕截图](assets/image-genai-1.png){zoomable="yes"}

### 生成内容 {#generate-content}

1. 为AI助手启用&#x200B;**[!UICONTROL 引用样式]**&#x200B;选项，以便根据所选内容对新内容进行个性化设置。

1. 选择您的&#x200B;**[!UICONTROL 品牌]**&#x200B;以确保AI生成的内容与您的品牌规格一致。 [了解有关Brands的更多信息](brands.md)。

1. 通过描述您要在&#x200B;**[!UICONTROL 提示]**&#x200B;字段中生成的内容，微调内容。

   如果您在编写提示时需要帮助，请访问&#x200B;**[!UICONTROL 提示库]**，该库提供了多种提示想法以改进投放。 [了解有关提示最佳实践的更多信息](ai-assistant-prompting-guide.md)

   ![屏幕截图显示Adobe Campaign Web中用于生成图像的提示库](assets/image-genai-2.png){zoomable="yes"}

1. 使用&#x200B;**[!UICONTROL 图像设置]**&#x200B;选项定制提示：

   * **[!UICONTROL 宽高比]**：确定资源的宽度和高度。 从通用比率（如16:9、4:3、3:2或1:1）中选择，或输入自定义大小。
   * **[!UICONTROL 内容类型]**：对可视元素的性质进行分类，区分不同的可视表示形式，如照片、图形或艺术品。
   * **[!UICONTROL 视觉强度]**：通过调整图像的强度来控制其影响。 较低的设置(2)产生更柔和的外观，而较高的设置(10)使图像更生动。
   * **[!UICONTROL 颜色和色调]**：调整颜色的总体外观以及传达的气氛或气氛。
   * **[!UICONTROL 光源]**：修改图像中的光源，以调整其大气形状并突出显示特定元素。
   * **[!UICONTROL 合成]**：在图像的框架中排列元素。

     ![显示Adobe Campaign Web中的图像设置选项的屏幕截图](assets/image-genai-4.png){zoomable="yes"}

1. 从&#x200B;**[!UICONTROL 引用内容]**&#x200B;菜单中，单击&#x200B;**[!UICONTROL 上载文件]**&#x200B;以添加任何品牌资产，这些品牌资产包含可以提供其他上下文AI助手的内容或选择以前上载的内容。

   以前上载的文件在&#x200B;**[!UICONTROL 上载的引用内容]**&#x200B;下拉列表中可用。 只需切换您想要包含到层代中的资产。

1. 如果对提示配置满意，请单击&#x200B;**[!UICONTROL 生成]**。

### 优化并完成 {#refine-finalize}

生成图像变体后，您可以查看结果、检查品牌对齐方式并为内容选择最佳选项。

1. 浏览生成的&#x200B;**[!UICONTROL 变体]**。

1. 单击百分比图标可查看您的&#x200B;**[!UICONTROL 品牌一致性得分]**&#x200B;并识别与您的品牌的所有不一致性。

   了解有关[品牌一致性分数](../content/brands-score.md)的更多信息。

   ![](assets/image-genai-3.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 预览]**&#x200B;以查看所选变体的全屏版本，或单击&#x200B;**[!UICONTROL 应用]**&#x200B;以替换当前内容。

1. 如果要查看与此变体相关的图像，请选择&#x200B;**[!UICONTROL 生成类似项]**。

1. 打开&#x200B;**[!UICONTROL 品牌一致性]**&#x200B;选项卡，查看内容如何与[品牌指南](../content/brands.md)保持一致。

1. 找到相应的内容后，单击&#x200B;**[!UICONTROL 选择]**。

1. 定义消息内容后，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮以控制渲染并使用测试用户档案检查个性化设置。 [了解详情](../preview-test/preview-content.md)

1. 查看并激活您的内容：
   * **电子邮件**：定义内容、受众和计划后，您就可以准备电子邮件投放了。 [了解详情](../monitor/prepare-send.md)
   * **登陆页面**：登陆页面准备就绪后，您可以发布该登陆页面，以供在消息中使用。 [了解详情](../landing-pages/create-lp.md)

## 适用于移动渠道 {#mobile-channels}

AI Assistant使您能够生成用于推送通知的引人入胜的图像，帮助您创建吸引眼球并与受众引起共鸣的有视觉吸引力的移动通信。

### 访问和配置 {#mobile-access-configure}

要开始使用AI助手为推送通知生成图像，请首先设置投放并打开AI助手。

1. 创建和配置推送通知投放后，单击&#x200B;**[!UICONTROL 编辑内容]**。 [了解详情](../push/create-push.md)

1. 访问&#x200B;**[!UICONTROL 显示AI助手]**&#x200B;菜单。

   ![显示“显示AI助手”菜单的屏幕快照](assets/push-img-1.png){zoomable="yes"}

### 生成内容 {#mobile-generate-content}

在访问AI助手后，您可以调整生成设置以创建与您的品牌相一致的图像并支持您的目标。

1. 选择您的&#x200B;**[!UICONTROL 品牌]**&#x200B;以确保AI生成的内容与您的品牌规格一致。 [了解有关Brands的更多信息](brands.md)。

1. 通过描述要在&#x200B;**[!UICONTROL 提示]**&#x200B;字段中生成的内容，优化内容。

   如果您在制作提示时寻求帮助，请访问&#x200B;**[!UICONTROL 提示库]**，该库提供了多种提示想法来改进促销活动。 [了解有关提示最佳实践的更多信息](ai-assistant-prompting-guide.md)

   具有提示字段和选项的![AI助手](assets/push-img-2.png){zoomable="yes"}

1. 选择&#x200B;**[!UICONTROL 图像]**&#x200B;以仅生成资源。

1. 选择您的&#x200B;**[!UICONTROL 图像设置]**：

   * **[!UICONTROL 内容类型]**：对可视元素的性质进行分类，区分不同的可视表示形式，如照片、图形或艺术品。
   * **[!UICONTROL 视觉强度]**：通过调整图像的强度来控制其影响。 较低的设置(2)产生更柔和、更受限的外观，而较高的设置(10)使图像更生动且视觉更强大。
   * **[!UICONTROL 光源]**：调整图像中的光源以调整其大气形状并突出显示特定元素。
   * **[!UICONTROL 合成]**：在图像的框架中排列元素。

     ![显示图像设置选项的屏幕快照](assets/push-img-3.png){zoomable="yes"}

1. 从&#x200B;**[!UICONTROL 引用内容]**&#x200B;菜单中，单击&#x200B;**[!UICONTROL 上载文件]**&#x200B;以添加任何品牌资产，这些品牌资产包含可以提供其他上下文AI助手的内容或选择以前上载的内容。

   以前上载的文件在&#x200B;**[!UICONTROL 上载的引用内容]**&#x200B;下拉列表中可用。 只需切换您想要包含到层代中的资产。

1. 提示就绪后，单击&#x200B;**[!UICONTROL 生成]**。

### 优化并完成 {#mobile-refine-finalize}

在为移动消息生成图像变体后，您可以微调结果以确保它们符合您的确切要求。

1. 生成后，浏览&#x200B;**[!UICONTROL 变体]**。

1. 单击百分比图标可查看您的&#x200B;**[!UICONTROL 品牌一致性得分]**&#x200B;并识别与您的品牌的所有不一致性。

   了解有关[品牌一致性分数](../content/brands-score.md)的更多信息。

   ![](assets/push-img-4.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 预览]**&#x200B;浏览&#x200B;**[!UICONTROL 变体]**。

1. 打开&#x200B;**[!UICONTROL 品牌一致性]**&#x200B;选项卡，查看内容如何与[品牌指南](brands.md)保持一致。

1. 找到相应的内容后，单击&#x200B;**[!UICONTROL 选择]**。

定义内容、受众和计划后，请准备推送投放。 [了解详情](../monitor/prepare-send.md)
