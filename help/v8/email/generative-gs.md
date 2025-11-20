---
audience: end-user
title: 开始使用 AI 助手
description: AI 助手入门
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 22%

---

# 使用 AI 助手 {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 助手"
>abstract="在精心制作和个性化定制您的投放内容后，请使用 AI 助手来提升您的内容质量。使用此功能，您可以通过描述要生成什么来微调内容，从而简化个性化及提升内容的过程。"

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="在 Campaign 中使用 AI 助手定义上下文"
>abstract="要将所选内容用作内容生成的输入，请激活&#x200B;**用当前内容增强**&#x200B;切换开关。还可上传品牌资源以将其用作来源。如果不使用所选内容，就必须上传并选择品牌资产。"

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成式 AI 条款"
>abstract="能否访问此功能取决于您是否同意遵守 Adobe Experience Cloud 生成式 AI 用户指南。请检查此功能产生的任何输出是否准确，并确保它适合您的用例。"
>additional-url="https://www.adobe.com/cn/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成式 AI 用户准则"

>[!INFO]
>
>使用[我们的实时功能预览](https://experienceleague.adobe.com/zh-hans/apps/journey-optimizer/ai-assistant-content-accelerator)，亲身体验亲身体验各种功能，让您亲身体验各种功能并充分了解其功能。

随着营销行业的竞争日益激烈，品牌厂商开始寻求有效的方法来快速生成有影响力的内容。 Adobe Campaign Web中的AI助手由Microsoft Azure OpenAI和Adobe Firefly提供支持，是Adobe的AI内容生成功能，可转变营销人员如何跨电子邮件、短信和推送通知等渠道创建专业且品牌一致的内容。 借助高级GenAI模型以及对品牌准则的深入了解，AI Assistant可根据营销目标自动生成个性化、引人入胜且有效的内容，并根据品牌概述的样式、布局、色调等优化内容。

AI Assistant可简化跨渠道（如电子邮件、短信和推送通知）的营销活动的创建和执行过程，从而节省时间、提高效率和取得更好的结果。

>[!IMPORTANT]
>
>* 在使用此功能之前，请查看相关的[护栏和限制](#generative-guardrails)。
>
>* 在Adobe Campaign Web中使用AI助手之前，必须同意[用户协议](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。 有关更多信息，请与您的 Adobe 代表联系。

## 访问AI助手 {#generative-access}

用于电子邮件、推送通知和短信的AI助手现已正式发布(GA)，可供所有用户使用。 授予用户访问权限所需的权限和步骤详述如下。

+++ 了解如何分配与内容生成相关的权限

1. **创建产品配置文件** — 在[Admin Console](https://stage.adminconsole.adobe.com/)中，使用以下特定模式创建产品配置文件：
   `Campaign - <instance-name> - AIAssistant`

1. **添加用户** — 将所需用户添加到该产品配置文件，\
   或者\
   **创建用户组**&#x200B;并将该用户组添加到产品配置文件，然后将用户添加到该产品配置文件。

在[本节](../get-started/permissions.md)中了解如何在Campaign中定义权限。

+++

## 护栏和限制 {#generative-guardrails}

下面列出了在Adobe Campaign Web中使用AI助手生成电子邮件的一般准则：

* 生成的内容的质量在很大程度上取决于您定义的营销目标或提示。 使用明确定义的GenAI模型提示来准确地解释。
* 上传品牌资产以确保准确的品牌内内容。 否则，内容将基于公开可用的信息。 上传的内容可以采用以下格式：PDF、JPEG、PNG或ZIP文件（具有支持的文件格式）。
* 上传的品牌资产的最大大小为50MB。 较大的文件或大量的图像可能会增加处理时间。
* 使用[内置电子邮件模板](../content/create-email-templates.md)、品牌特定模板或自定义模板通过AI助手创建电子邮件内容。 建议使用最多包含8至10个图像的电子邮件模板。
* 在选择变体时，使用拇指上移、拇指下移或标记图标报告任何有问题的输出。
* 您对AI助手的使用受Adobe Experience Cloud创作AI用户指南的约束。 [了解详情](https://www.adobe.com/cn/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。
* 作为Adobe在媒体创建中使用创作AI工具时实现透明化承诺的一部分，Adobe在下载或导出内容或项目时应用Content Credentials，其中包含Firefly生成的资源。 [了解详情](https://helpx.adobe.com/cn/firefly/using/content-credentials.html)。

以下限制适用于Adobe Campaign Web中的AI助手：

* Adobe Campaign Web中的AI助手当前仅支持英文。 非英文输入内容可能会产生不一致或错误的结果。 非英文答复引起的问题，目前不予处理或改进。
* 仅适用于电子邮件、推送和短信渠道。
* GenAI内容可能并不总是准确的。 分享您的反馈，以便工程师可以优化模型。
* 您可以上传多个品牌资产，但只能为特定世代利用一个品牌资产。

## AI助手内容生成功能 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[使用AI助手生成电子邮件]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
使用AI助手生成<a href="generative-content.md"><strong>电子邮件</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[使用AI助手生成短信]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div>使用AI助手生成<a href="generative-sms.md"><strong>短信</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[使用AI助手生成推送通知]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
使用AI助手生成<a href="generative-push.md"><strong>推送通知</strong></a>
</div>
<p></td>
</tr></table>