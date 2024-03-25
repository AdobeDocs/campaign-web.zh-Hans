---
audience: end-user
title: 使用AI助手显示文本
description: Campaign中的AI助手入门
badge: label="Beta 版"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 5%

---

# 使用AI助手生成电子邮件 {#generative-content}

>[!BEGINSHADEBOX]

**目录**

* [AI助手入门](generative-gs.md)
* **[使用AI助手生成电子邮件](generative-content.md)**
* [使用AI助手生成短信](generative-sms.md)
* [使用AI助手生成推送通知](generative-push.md)

>[!ENDSHADEBOX]

创建电子邮件并使其个性化后，可使用由创作AI提供支持的Campaign中的Journey Optimizer AI Assistant将您的内容提升到新的水平。

AI Assistant可以通过建议更可能引起受众共鸣的不同内容来帮助您优化投放的影响。

>[!NOTE]
>
>在开始使用此功能之前，请阅读相关内容 [护栏和限制](generative-gs.md#guardrails-and-limitations).

## 使用AI助手生成内容 {#generative-text}

1. 创建和配置电子邮件投放后，单击 **[!UICONTROL 编辑内容]**.

   有关如何配置电子邮件投放的更多信息，请参阅 [此页面](../email/create-email-content.md).

1. 填写 **[!UICONTROL 基本详细信息]** 用于您的投放。 完成后，单击 **[!UICONTROL 编辑内容]**.

1. 根据需要个性化您的电子邮件。 [了解详情](content-components.md)

1. 访问 **[!UICONTROL AI助手]** 菜单。

   您还可以选择 **[!UICONTROL 文本组件]** 以仅定位特定内容。

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. 通过描述您要在 **[!UICONTROL 提示]** 字段。

   如果您在制作提示时需要帮助，请访问 **[!UICONTROL 提示库]** 其中提供了多种旨在改进交付的即时想法。

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. 切换 **[!UICONTROL 主题行]** 或 **[!UICONTROL 预编译标头]** 以将其包含在变量生成中。

1. 在上下文菜单中，启用 **[!UICONTROL 使用当前上下文增强]** AI助手选项，用于根据投放、投放名称和所选受众来个性化新内容。

   >[!IMPORTANT]
   >
   > 您的提示必须始终通过上传品牌资产或启用 **[!UICONTROL 增强当前内容]** 选项。

1. 单击 **[!UICONTROL 上传品牌资产]** 添加任何品牌资产，其中包含可为AI助手提供其他上下文的内容。

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. 选择 **[!UICONTROL 沟通策略]** 最符合你的需要。 这将影响生成的文本的色调和样式。

1. 选择 **[!UICONTROL 语言]** 和 **[!UICONTROL 色调]** 您希望生成的文本包含。 这将确保文本适合您的受众和用途。

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. 提示就绪后，单击 **[!UICONTROL 生成]**.

1. 浏览生成的页面 **[!UICONTROL 变体]** 并单击 **[!UICONTROL 应用]** 找到相应的内容后。

   单击 **[!UICONTROL 预览]** 以查看所选变体的全屏版本。

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. 插入个性化字段，以根据用户档案数据自定义电子邮件内容。 [详细了解内容个性化](../personalization/personalize.md)

   ![](assets/text-genai-6.png){zoomable=&quot;yes&quot;}

1. 定义消息内容后，单击 **[!UICONTROL 模拟内容]** 按钮来控制渲染，并使用测试用户档案检查个性化设置。 [了解详情](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

1. 定义内容、受众和计划后，便可以准备电子邮件投放。 [了解详情](../monitor/prepare-send.md)

## 使用AI助手生成图像 {#generative-image}

在下面的示例中，了解如何利用AI Assistant优化和改进您的内容，确保获得对用户更友好的体验。 执行以下步骤：

1. 创建和配置电子邮件投放后，单击 **[!UICONTROL 编辑内容]**.

   有关如何配置电子邮件投放的更多信息，请参阅 [此页面](../email/create-email-content.md).

1. 填写 **[!UICONTROL 基本详细信息]** 用于您的投放。 完成后，单击 **[!UICONTROL 编辑电子邮件内容]**.

1. 选择要使用AI助手更改的资源。

1. 从右侧菜单中，选择 **[!UICONTROL AI助手]**.

   ![](assets/image-genai-1.png){zoomable=&quot;yes&quot;}

1. 通过描述您要在 **[!UICONTROL 提示]** 字段。

   如果您在制作提示时需要帮助，请访问 **[!UICONTROL 提示库]** 其中提供了多种旨在改进交付的即时想法。

   ![](assets/image-genai-2.png){zoomable=&quot;yes&quot;}

1. 单击 **[!UICONTROL 上传品牌资产]** 添加任何品牌资产，其中包含可为AI助手提供其他上下文的内容。

   >[!IMPORTANT]
   >
   > 您的提示必须始终与特定上下文关联。

1. 选择 **[!UICONTROL 宽高比]** 您的资产的。 这会确定资源的宽度和高度。

   您可以选择常用比率，如16:9、4:3、3:2或1:1，也可以输入自定义大小。

1. 自定义 **[!UICONTROL 颜色和色调]**， **[!UICONTROL 内容类型]**， **[!UICONTROL 照明]** 和 **[!UICONTROL 合成]** 设置以匹配所需的资源特征。

   ![](assets/image-genai-3.png){zoomable=&quot;yes&quot;}

1. 对提示配置感到满意后，单击 **[!UICONTROL 生成]**.

1. 浏览 **[!UICONTROL 变量建议]** 以查找所需的资产。

   单击 **[!UICONTROL 预览]** 以查看所选变体的全屏版本。

   ![](assets/image-genai-5.png){zoomable=&quot;yes&quot;}

1. 选择 **[!UICONTROL 显示类似项]** 如果您想查看与此变体相关的图像。

1. 单击 **[!UICONTROL 选择]** 找到相应的内容后。

   ![](assets/image-genai-6.png){zoomable=&quot;yes&quot;}

1. 定义消息内容后，单击 **[!UICONTROL 模拟内容]** 按钮来控制渲染，并使用测试用户档案检查个性化设置。  [了解详情](../preview-test/preview-content.md)

   ![](assets/image-genai-7.png){zoomable=&quot;yes&quot;}

1. 定义内容、受众和计划后，便可以准备电子邮件投放。 [了解详情](../monitor/prepare-send.md)
