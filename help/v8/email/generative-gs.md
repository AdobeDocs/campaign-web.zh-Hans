---
audience: end-user
title: 开始使用 AI 助手
description: AI助手入门
badge: label="Beta 版"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 40%

---

# 开始使用 AI 助手 {#generative-gs}

>[!BEGINSHADEBOX]

**目录**

* **[AI助手入门](generative-gs.md)**
* [使用AI助手生成电子邮件](generative-content.md)
* [使用AI助手生成短信](generative-sms.md)
* [使用AI助手生成推送通知](generative-push.md)

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
>abstract="您必须同意 Adobe Experience Cloud 生成式 AI 用户准则才能使用此功能。您向此功能提供的任何提示、上下文或补充信息或其他输入都必须与特定的上下文关联，这些特定的上下文可包括您的品牌宣传材料、网站内容、数据、此类数据的架构、模板或其他可信文档，并且不得包含任何个人信息（个人信息包括任何可追溯回具体个人的信息）。您应检查此功能产生的任何输出是否准确，并确保它适合您的用例"
>additional-url="https://www.adobe.com/cn/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成式 AI 用户准则"

AI助手是改进电子邮件内容的宝贵工具。 它简化了个性化和内容增强，优化了电子邮件投放以更好地与受众引起共鸣。

此功能通过自动生成完整的电子邮件内容来节省时间并确保一致的质量。 通过使用Generative AI，您可以轻松创建引人注目的电子邮件，从而提高沟通的有效性和效率。

>[!NOTE]
>
>此功能在其Alpha版本中提供，如有更改，恕不另行通知。 它将在10月初激活。

## 护栏和限制 {#generative-guardrails}

下面列出了在Campaign中使用AI助手生成电子邮件的一般准则：

* 生成的内容的质量在很大程度上受您定义的营销目标/提示的影响。 使用明确定义的提示以准确解释GenAI模型。 
* 上传品牌资产以对品牌内容保持准确。 否则，内容基于公开可用的信息。 上传的内容可以具有以下格式：PDF、JPEG、PNG或ZIP文件（具有支持的文件格式）。
* 上传的品牌资产的建议大小小于50MB。 较大的文件或大量的图像可以工作，但处理时间会增加。
* 最好使用Adobe Campaign创作的电子邮件模板 [内置电子邮件模板](../email/create-email-templates.md)，用于创建电子邮件内容的特定于品牌的模板或自定义模板。 建议使用最多包含8至10张图像的电子邮件模板。


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
<a href="generative-content.md"><strong>使用AI助手生成电子邮件</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="短信生成" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>使用AI助手生成短信</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="推送生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>使用AI助手生成推送通知</strong></a>
</div>
<p></td>
</tr></table>
