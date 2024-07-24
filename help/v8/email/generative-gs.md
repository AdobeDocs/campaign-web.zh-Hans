---
audience: end-user
title: 开始使用 AI 助手
description: AI助手入门
badge: label="Beta 版"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 32%

---

# 开始使用 AI 助手 {#generative-gs}

>[!BEGINSHADEBOX]

**目录**

* 开始使用 AI 助手
* [使用 AI 助手生成电子邮件](generative-content.md)
* [使用 AI 助手生成短信](generative-sms.md)
* [使用 AI 助手生成推送通知](generative-push.md)

>[!ENDSHADEBOX]

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

随着营销行业的竞争日益激烈，各大品牌都在寻求高效的方法，以便快速高效地生成有影响力的内容。 Campaign中的AI助手由Azure OpenAI提供支持，是Adobe的AI内容生成功能，可彻底改变营销人员跨电子邮件、短信、推送等渠道创建专业且品牌一致的内容的方式。 借助高级GenAI模型以及对品牌准则的深入了解，AI Assistant可根据营销目标自动生成个性化、引人入胜且有效的内容，其内容针对品牌概述的样式、布局、色调等进行了优化。

AI Assistant可以跨渠道（如电子邮件、短信和推送）直观地创建和执行营销活动，既简单又无麻烦，同时还能节省时间、提高效率和产生更好的结果。

>[!NOTE]
>
>此功能在其Beta版本中提供，如有更改，恕不另行通知。

## 护栏和限制 {#generative-guardrails}

下面列出了在Campaign中使用AI助手生成电子邮件的一般准则：

* 生成的内容的质量在很大程度上受您定义的营销目标/提示的影响。 使用明确定义的提示以准确解释GenAI模型。 
* 上传品牌资产以对品牌内容保持准确。 否则，内容基于公开可用的信息。 上传的内容可以具有以下格式：PDF、JPEG、PNG或ZIP文件（具有支持的文件格式）。
* 上传的品牌资产的最大大小为50MB。 较大的文件或大量的图像可以工作，但处理时间会增加。
* 使用Adobe Campaign创作的电子邮件模板（最好是[内置电子邮件模板](../email/create-email-templates.md)）、特定于品牌的模板或自定义模板来创建您的电子邮件内容。 建议使用最多包含8至10张图像的电子邮件模板。
* 选择变体时，请确保使用向上缩略图、向下缩略图或标记图标报告任何有问题的输出。
* 您对AI助手的使用受Adobe Experience Cloud创作AI用户指南的约束。 [了解详情](https://www.adobe.com/cn/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

以下限制适用于Campaign中的AI助手：

* 支持的语言仅是英语。
* 仅适用于电子邮件、推送和短信渠道。
* GenAI内容可能并不总是准确的：请分享您的反馈，以便我们的工程师可以优化模型。
* 您可以上传多个品牌资产，但只能为特定世代利用一个。

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
