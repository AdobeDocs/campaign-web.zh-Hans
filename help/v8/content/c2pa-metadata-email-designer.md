---
audience: end-user
product: campaign
title: 电子邮件和登陆页面设计器中的 C2PA 元数据
description: 了解已附加到图像的C2PA元数据在Adobe Campaign Web用户界面中的电子邮件和登陆页设计器中移动时会发生什么情况。
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 4%
---

# 电子邮件和登陆页面设计器中的 C2PA 元数据 {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**在此页上：**&#x200B;了解已附加到图像的C2PA元数据在Adobe Campaign Web用户界面中的电子邮件和登陆页设计器中移动时发生了什么情况。

>[!ENDSHADEBOX]

>[!INFO]
>
>围绕创新型人工智能透明度的新法律正在出现，Adobe正在努力满足跨司法辖区的适用要求。 C2PA元数据是Adobe用于满足这些法规要求的源工具。

电子邮件和登陆页设计器本身不会生成或编辑图像。 它引用了在其他Adobe工具（如生成内容、Adobe Express或Firefly）或合作伙伴模型中已使用创作AI生成或编辑的图像。 构建、发布和发送时，已附加到这些图像的C2PA元数据将保留不变。

## 在生成和发送时，将保留C2PA元数据 {#c2pa-preserved}

下表总结了使用电子邮件和登陆页设计器构建和发送内容的每个步骤对C2PA元数据的影响。

| 操作 | 发生什么情况 | 是否保留C2PA元数据？ | 示例 |
| --- | --- | --- | --- |
| **将图像插入模板** | 设计器会添加对其他位置（如生成内容、Adobe Express、Firefly或合作伙伴模型）已使用创作AI生成或编辑的图像的引用。 不会更改图像文件本身。 | 是，未更改 | Firefly生成的横幅将插入到电子邮件模板中。 |
| **调整大小、重新定位或添加替换文本** | 仅显示模板的HTML更改中的属性。 图像文件未重新编码。 | 是，未更改 | 调整图像大小以适合移动布局和给定的替换文本。 |
| **发布** | 发布电子邮件或登陆页面，并存储图像以进行交付。 | 是，未更改 | 发布营销活动，并存储其图像以供发送。 |
| **发送电子邮件或查看登陆页面** | 图像会传送到收件人的收件箱或显示在实时页面上。 | 是，未更改 | 收件人打开电子邮件并下载图像；凭据仍与原始凭据匹配。 |

## 内容类型及其范围 {#c2pa-content-types}

* **图像**：已覆盖。 如上所示，已附加到图像的C2PA元数据在插入、调整、发布和交付时会保留。
* **视频、音频、文本**：不适用。 电子邮件和登陆页设计器不会使用创作AI生成或编辑这些内容类型。

## 内容移动时发生的情况 {#c2pa-content-moves}

C2PA元数据在Adobe Campaign Web用户界面中的电子邮件和登陆页设计器中随图像一起移动，从您的编辑器到存储区，再到收件人的收件箱或实时页面。 在以上任何步骤中，都不会创建、更改或删除任何凭据。

如果图像不带有创作AI C2PA元数据，则由于它不是使用创作AI生成或编辑的，因此此处不会显示凭据。 这是正常情况，而不是错误。

## 检查凭据 {#c2pa-checking-credential}

尚无法直接在电子邮件或登陆页面设计器中检查Content Credential。

## 其他资源

* [使用“生成内容”](generative-gs.md)
* [创作AI内容透明度](https://experienceleague.adobe.com/zh-hans/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)