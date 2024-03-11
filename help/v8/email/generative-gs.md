---
audience: end-user
title: 内容助手快速入门
description: 内容助手入门
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 65f041275930a0f18993b1ba37b936d8ef51d119
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 22%

---

# 内容助手快速入门 {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="内容助手"
>abstract="在精心设计并个性化您的投放后，您可使用内容助手增强您的内容。此功能使您通过描述要生成的东西即可微调内容，从而简化个性化和改善内容的过程。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="定义内容生成的上下文"
>abstract="要将所选内容用作内容生成的输入，请激活&#x200B;**用当前内容增强**&#x200B;切换开关。还可上传品牌资源以将其用作来源。如果不使用所选内容，则必须上传并选择品牌资源。"


>[!CONTEXTUALHELP]
>id="acw_generate_emagica"
>title="Adobe 生成式 AI 术语"
>abstract="对此功能的访问取决于您对Adobe Experience Cloud创作AI用户指南的同意。 您为此功能提供的任何提示、上下文或补充信息或其他输入都必须与特定上下文绑定，该上下文可以包括您的品牌推广材料、网站内容、数据、此类数据的架构、模板或其他受信任文档，并且不得包含任何个人信息（个人信息包括可以链接回特定个人的任何内容）。 您应该检查此功能的任何输出是否准确，并确保它适合您的用例"
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe生成AI用户指南"


内容助手由创作AI提供支持，是改进电子邮件内容的宝贵工具。 它简化了个性化和内容增强，优化了电子邮件投放以更好地与受众引起共鸣。

此功能通过自动生成完整的电子邮件内容来节省时间并确保一致的质量。 通过使用Generative AI，您可以轻松创建引人注目的电子邮件，从而提高沟通的有效性和效率。


您可以在电子邮件中将Campaign内容助手发送至： [生成图像](generative-image.md)， [生成文本内容](generative-content.md)， [生成完整的HTML内容](generative-email.md).

>[!NOTE]
>
>此功能在其Alpha版本中提供，如有更改，恕不另行通知。 它将在10月初激活。

## 护栏和限制 {#generative-guardrails}

以下列出了使用内容助手生成电子邮件的一般准则：

* 生成的内容的质量在很大程度上受您定义的营销目标/提示的影响。 使用明确定义的提示以准确解释GenAI模型。 
* 上传品牌资产以对品牌内容保持准确。 否则，内容基于公开可用的信息。 上传的内容可以具有以下格式：PDF、JPEG、PNG或ZIP文件（具有支持的文件格式）。
* 上传的品牌资产的建议大小小于10MB。 较大的文件或大量的图像可以工作，但处理时间会增加。
* 使用Adobe Campaign创作的电子邮件模板，或者首选 [内置电子邮件模板](../email/create-email-templates.md) 以创建您的电子邮件内容。 建议使用最多包含8至10张图像的电子邮件模板。


以下限制适用于Campaign内容助手：

* 支持的语言仅是英语
* 仅适用于电子邮件渠道
* GenAI内容可能并不总是准确的：请分享您的反馈，以便我们的工程师可以优化模型
* 您可以上传多个品牌资产，但只能为特定世代利用一个



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="文本生成" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>使用内容助手生成文本</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="图像生成" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>使用内容助手生成图像</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="电子邮件生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>使用内容助手生成电子邮件</strong></a>
</div>
<p></td>
</tr></table>
