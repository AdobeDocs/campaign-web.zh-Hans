---
audience: end-user
title: AI Assistant内容加速器入门
description: AI Assistant内容加速器入门
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: aea828da825a416dece6c4bee1da6d4e570e4e48
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 19%

---

# 使用AI Assistant内容加速器  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="AI Assistant内容加速器"
>abstract="AI Assistant可以跨渠道（如电子邮件、短信和推送）直观地创建和执行营销活动，既简单又无麻烦，同时还能节省时间、提高效率和产生更好的结果。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 助手"
>abstract="在精心设计并个性化设置投放后，您可使用 AI 助手来增强您的内容。此功能使您通过描述要生成的东西即可微调内容，从而简化个性化和改善内容的过程。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="在 Campaign 中使用 AI 助手定义上下文"
>abstract="要将所选内容用作内容生成的输入，请激活&#x200B;**用当前内容增强**&#x200B;切换开关。还可上传品牌资源以将其用作来源。如果不使用所选内容，则必须上传并选择品牌资源。"

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成式 AI 条款"
>abstract="您必须同意 Adobe Experience Cloud 生成式 AI 用户准则才能使用此功能。请检查此功能产生的任何输出是否准确，并确保它适合您的用例。"
>additional-url="https://www.adobe.com/cn/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成式 AI 用户准则"

>[!INFO]
>
>使用[我们的交互式演示](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator)亲身体验亲身体验，该演示旨在让您亲身体验其功能并充分了解其功能。


随着营销行业的竞争日益激烈，各大品牌都在寻求高效的方法，以便快速高效地生成有影响力的内容。 Adobe Campaign Web中的AI Assistant for Content Acceleration由Microsoft Azure OpenAI和Adobe Firefly提供支持，是Adobe的AI内容生成功能，它彻底改变了营销人员跨电子邮件、短信、推送等渠道创建专业且品牌一致的内容的方式。 借助高级GenAI模型以及对品牌准则的深入了解，AI Assistant可根据营销目标自动生成个性化、引人入胜且有效的内容，其内容针对品牌概述的样式、布局、色调等进行了优化。

AI Assistant可以跨渠道（如电子邮件、短信和推送）直观地创建和执行营销活动，既简单又无麻烦，同时还能节省时间、提高效率和产生更好的结果。

>[!IMPORTANT]
>
>* 在开始使用此功能之前，请阅读相关的[护栏和限制](#generative-guardrails)。
>
>* 您必须同意[用户协议](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)，然后才能使用Adobe Campaign Web中的AI助手进行内容加速。 有关更多信息，请与您的 Adobe 代表联系。

## 访问AI Assistant内容加速器 {#generative-access}

用于电子邮件、推送通知和短信的AI助手内容加速器现已正式发布(GA)，可供所有用户使用。 授予用户访问权限所需的权限和步骤详述如下。

+++  了解如何分配与内容生成相关的权限

1. **创建产品配置文件** — 在[Admin Console](https://stage.adminconsole.adobe.com/)中，使用以下特定模式创建产品配置文件：
   `Campaign - <instance-name> - AIAssistant`

1. **添加用户** — 将所需用户添加到该产品配置文件，
或
   **创建用户组**&#x200B;并将该用户组添加到产品配置文件中，并将用户添加到该产品配置文件中。

在[本节](../get-started/permissions.md)中了解如何在Campaign中定义权限。

+++

## 护栏和限制 {#generative-guardrails}

下面列出了在Adobe Campaign Web中使用AI助手进行内容加速以生成电子邮件的一般准则：

* 生成的内容的质量在很大程度上受您定义的营销目标/提示的影响。 使用明确定义的提示以准确解释GenAI模型。 
* 上传品牌资产以对品牌内容保持准确。 否则，内容基于公开可用的信息。 上传的内容可以具有以下格式：PDF、JPEG、PNG或ZIP文件（具有支持的文件格式）。
* 上传的品牌资产的最大大小为50MB。 较大的文件或大量的图像可以工作，但处理时间会增加。
* 使用[内置电子邮件模板](../email/create-email-templates.md)、品牌特定模板或自定义模板通过内容加速器创建电子邮件内容。 建议使用最多包含8至10个图像的电子邮件模板。
* 选择变体时，请确保使用向上缩略图、向下缩略图或标记图标报告任何有问题的输出。
* 您对AI助手的使用受Adobe Experience Cloud创作AI用户指南的约束。 [了解详情](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* 作为Adobe承诺在媒体创建中使用创新型人工智能工具时提高透明度的一部分，Adobe将在下载或导出内容或项目包含Firefly生成的资源时应用Content credentials。 [了解详情](https://helpx.adobe.com/firefly/using/content-credentials.html)

以下限制适用于Adobe Campaign Web中用于内容加速的AI助手：

* Adobe Campaign Web中用于内容加速的AI助手当前仅支持英语版本。 非英文输入内容可能会产生不一致或错误的结果。 非英文答复引起的问题目前不予处理或改进。
* 仅适用于电子邮件、推送和短信渠道。
* GenAI内容可能并不总是准确的：请分享您的反馈，以便我们的工程师可以优化模型。
* 您可以上传多个品牌资产，但只能为特定世代利用一个。

## AI助手内容生成功能 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="电子邮件生成" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
使用AI助手生成<a href="generative-content.md"><strong>电子邮件</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="短信生成" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div>使用AI助手生成<a href="generative-sms.md"><strong>短信</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="推送生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
使用AI助手生成<a href="generative-push.md"><strong>推送通知</strong></a>
</div>
<p></td>
</tr></table>
