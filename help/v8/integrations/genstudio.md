---
title: 在Adobe Campaign中使用GenStudio for Performance Marketing
description: 了解如何在Adobe Campaign中使用GenStudio for Performance Marketing
feature: Email Design
topic: Content Management, Artificial Intelligence
badge: label="有限可用性" type="Informative"
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 7%

---

# 使用 GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="使用 GenStudio 构建的模板"
>abstract="得益于与 Adobe GenStudio for Performance Marketing 的无缝集成，您可以轻松导入使用 Adobe AI 技术优化的 GenStudio 模板。"

## GenStudio入门 {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"}是一个创新型人工智能优先应用程序，它允许营销团队创建自己的广告和电子邮件，以推动符合您的品牌标准并遵守企业政策的有影响力的个性化营销活动。 通过利用Adobe AI技术，它提供了一套全面的工具，可简化内容创建和管理过程，以便创意人员可以专注于创新。

>[!AVAILABILITY]
>
>此功能仅适用于电子邮件渠道。

为了提高营销效率并维护品牌一致性，您可以将&#x200B;[!DNL **GenStudio for Performance Marketing**]&#x200B;体验与&#x200B;[!DNL **Adobe Campaign**]&#x200B;无缝集成。 这使您能够利用[!DNL GenStudio]的AI功能内容创建以及[!DNL Adobe Campaign]的高级编排功能。

>[!INFO]
>
>若要继续，请查看此[概述](https://business.adobe.com/cn/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"}和[的](https://business.adobe.com/cn/products/genstudio-for-performance-marketing.html#demo){target="_blank"}演示[!DNL Adobe GenStudio for Performance Marketing]。

## 在Adobe Campaign中使用GenStudio功能 {#use-genstudio}

通过[!DNL GenStudio for Performance Marketing]和[!DNL Adobe Campaign]集成，您可以让公司中的营销人员更好地协作以简化流程。

例如，使用[!DNL Adobe Campaign]开发和自动化电子邮件营销活动的技术营销人员可以与使用[!DNL GenStudio]创建内容的性能营销人员协作。

通过此集成，双方可以共同轻松地将[!DNL GenStudio]中的品牌上内容集成到[!DNL Adobe Campaign]中，从而提供针对特定客户细分并促进销售的引人入胜的电子邮件。

### 将HTML模板从Adobe Campaign导出到GenStudio {#export-from-campaign-to-genstudio}

首先，您可以将包含品牌准则的[!DNL Adobe Campaign] HTML模板导出到[!DNL GenStudio for Performance Marketing]。 请按照以下步骤操作。

1. 在[!DNL Adobe Campaign]中，访问电子邮件的内容。 [了解如何操作](../email/create-email.md#create-content)

1. 在电子邮件Designer中，从&#x200B;**[!UICONTROL 更多]**&#x200B;按钮中选择&#x200B;**[!UICONTROL 导出HTML]**。

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. 将此HTML导出模板上载到[!DNL GenStudio for Performance Marketing]。<!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >在[!DNL GenStudio]HTML用户指南[专用部分中了解如何将Adobe GenStudio for Performance Marketing模板上载到](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}。<!--GenStudio doc to be updated with Campaign-->

1. 在GenStudio中，使用此模板创建多个具有AI提示的电子邮件变体并保存它们。

   >[!NOTE]
   >
   >了解如何在GenStudio专用的[部分](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"}中创建电子邮件体验。

### 在Adobe Campaign中利用GenStudio体验 {#leverage-genstudio-experiences}

要利用您刚刚通过将变体导入到[!DNL GenStudio]中而创建的[!DNL Adobe Campaign]电子邮件变体，请执行以下步骤。

1. 在[!DNL Adobe Campaign]中，[创建电子邮件投放](../email/create-email.md)。

1. 在电子邮件投放仪表板中，单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。 [了解详情](../email/create-email.md#create-content)

1. 在电子邮件Designer主页上，选择&#x200B;**[!UICONTROL 导入HTML]**，然后单击&#x200B;**[!UICONTROL Adobe GenStudio for Performance Marketing]**&#x200B;按钮。

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. 浏览GenStudio体验以开始构建您的内容。 您可以根据多个标准筛选体验，例如产品、角色、品牌甚至颜色。

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. 选择一个体验，然后单击&#x200B;**[!UICONTROL 使用]**。

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. 选择要导入GenStudio体验的文件夹。

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. 选定的内容显示在电子邮件Designer中。

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >从[模板 [!DNL Adobe Campaign] 创建的GenStudio体验](#export-from-ajo-to-genstudio)将直接导入电子邮件Designer。 未使用[!DNL Adobe Campaign]模板创建的GenStudio体验已导入到[兼容模式](../email/existing-content.md)中。

   使用[电子邮件内容编辑工具](../email/create-email-content.md)和[个性化字段](../personalization/personalize.md)根据需要编辑电子邮件。 保存您的内容。

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456059/?captions=chi_hans&quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->