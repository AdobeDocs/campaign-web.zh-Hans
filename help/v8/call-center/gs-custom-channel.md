---
audience: end-user
title: 自定义渠道入门
description: 了解如何使用Adobe Campaign Web创建和发送自定义渠道投放
exl-id: b4336a0a-d845-4024-a06b-400fce1316a4
source-git-commit: 1a5f49cfdf56a21faedcef3029b62b88ebd81c8d
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 3%

---

# 自定义渠道入门 {#gs-custom-channel}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="API投放的自定义渠道"
>abstract="现在，您可以直接从Adobe Campaign Web UI基于自定义API渠道编排和执行投放。 这些投放可以是独立投放或工作流的一部分。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

您可以直接从Adobe Campaign Web UI根据与第三方集成的自定义渠道编排和执行投放。 自定义渠道的配置在客户端控制台中执行。

支持两种类型的自定义渠道：外部和API。 借助外部渠道，Campaign会生成可自定义的导出文件，其中包含所有必要的联系和个性化数据。 通过API渠道，消息会通过配置的API发送到目标用户档案。

您可以在工作流中添加自定义渠道投放，也可以将其用作独立投放。

以下步骤详细介绍了独立（一次性）投放的过程。 大多数步骤类似于呼叫中心投放。 有关详细信息，请参阅此[页面](../call-center/create-call-center.md)。

要发送新的独立自定义投放，请执行以下步骤：

1. 配置自定义渠道，[了解更多](#create-channel)
1. 创建投放，[了解更多](#create-delivery)
1. 定义受众，[了解更多](#select-audience)
1. 编辑内容，[阅读更多](#edit-content)
1. 预览并发送投放，[了解更多](#preview-send)

## 配置自定义渠道{#create-channel}

首先，您需要配置自定义渠道。 以下是要在客户端控制台中执行的主要步骤。 这些步骤对于自定义外部和API渠道是通用的：

1. 配置架构以将新渠道添加到可用渠道列表。 [了解更多信息](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans#configure-schema){target="_blank"}
1. 创建新的路由外部帐户。 [了解更多信息](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans#reate-ext-account){target="_blank"}
1. 创建与新渠道关联的新投放模板。 [了解更多信息](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans#create-template){target="_blank"}

自定义API渠道需要其他配置。 [了解更多信息](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans#api-additional){target="_blank"}

## 创建投放{#create-delivery}

请按照以下步骤创建投放并配置其属性：

1. 选择&#x200B;**[!UICONTROL 投放]**&#x200B;菜单并单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮。

1. 选择所需的自定义渠道，选择关联的模板，然后单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;以进行确认。

   ![显示自定义投放创建的屏幕截图](assets/cus-create.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 属性]**&#x200B;下，输入投放的&#x200B;**[!UICONTROL 标签]**。

   ![显示自定义投放的属性配置的屏幕截图](assets/cus-properties.png){zoomable="yes"}

有关投放创建的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#create-delivery)。

## 定义受众{#select-audience}

现在，您需要定义将定向的受众。

1. 从投放仪表板的&#x200B;**[!UICONTROL 受众]**&#x200B;部分，单击&#x200B;**[!UICONTROL 选择受众]**。

1. 选择现有受众或创建您自己的受众。

   ![显示自定义投放的受众选择的屏幕截图](assets/cc-audience2.png){zoomable="yes"}

有关受众定义的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#select-audience)。

## 编辑内容{#edit-content}

现在，我们来编辑投放的内容。

>[!BEGINTABS]

>[!TAB 自定义外部渠道]

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。

1. 指定&#x200B;**[!UICONTROL 文件名]**，选择&#x200B;**[!UICONTROL 文件格式]**，然后根据需要为提取文件添加任意数量的列。

   ![显示提取文件属性配置选项的屏幕快照。](assets/cc-content-attributes.png)

>[!TAB 自定义API渠道]

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。

1. 根据需要填写字段。 要了解如何设置此屏幕，请参阅此[页面](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans#api-additional-screen){target="_blank"}。

   ![显示API渠道属性配置选项的屏幕截图。](assets/cc-content-attributes-api.png)

>[!ENDTABS]

有关内容版本的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#edit-content)。

## 预览并发送投放{#preview-send}

当投放内容准备就绪时，您可以使用测试用户档案预览该内容。 然后，您可以发送投放以生成提取文件或通过API发送消息。

>[!BEGINTABS]

>[!TAB 自定义外部渠道]

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。

1. 在投放内容页面中，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮并选择测试配置文件。

   ![在投放内容页面中显示模拟内容选项的屏幕截图](assets/cus-simulate.png){zoomable="yes"}

>[!TAB 自定义API渠道]

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。

1. 在投放内容页面中，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮并选择测试配置文件。

1. 单击右侧的&#x200B;**打开预览**。 此功能需要使用JSSP进行配置。 请参见[此页面](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans#api-additional-preview){target="_blank"}。

   ![屏幕截图显示API的投放内容页面中的“模拟内容”选项](assets/cus-simulate-api.png){zoomable="yes"}

>[!ENDTABS]

在投放仪表板中，单击&#x200B;**[!UICONTROL 审阅和发送]**，然后单击&#x200B;**[!UICONTROL 准备]**。 然后，确认。 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以继续执行最终发送过程，然后确认。

![显示准备选项和日志菜单的屏幕快照](assets/cus-prepare.png){zoomable="yes"}

有关预览和发送的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#preview-send)。
