---
audience: end-user
title: 自定义外部渠道入门
description: 了解如何使用Adobe Campaign Web创建和发送自定义外部渠道投放
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# 自定义外部渠道入门 {#gs-custom-channel}

您可以直接从Adobe Campaign Web UI根据与第三方集成的自定义外部渠道编排和执行投放。 自定义外部渠道的创建在客户端控制台中执行。

您可以在工作流中配置自定义渠道外部投放，或将其配置为独立投放，定义受众，并使用所有必需的联系人和个性化数据生成可自定义的导出文件。

>[!NOTE]
>
>在Web UI中，报告不适用于自定义渠道外部投放。 您必须浏览到“客户端控制台”才能访问报告。

以下步骤详细介绍了独立（一次性）投放的过程。 大多数步骤类似于呼叫中心投放。 有关详细信息，请参阅此[页面](../call-center/create-call-center.md)。

要创建和发送新的独立自定义外部投放，请执行以下步骤：

1. 创建自定义外部渠道，[了解更多](#create-channel)
1. 创建投放，[了解更多](#create-delivery)
1. 定义受众，[了解更多](#select-audience)
1. 编辑内容，[阅读更多](#edit-content)
1. 预览并发送投放，[了解更多](#preview-send)

## 创建自定义外部渠道{#create-channel}

首先，您需要配置自定义外部渠道。 以下是要在客户端控制台中执行的主要步骤：

1. 配置架构以将新渠道添加到可用渠道列表。
1. 创建新的路由外部帐户。
1. 创建与新渠道关联的新投放模板。

有关详细信息，请参阅[客户端控制台文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=zh-Hans)

## 创建投放{#create-delivery}

请按照以下步骤创建投放并配置其属性：

1. 选择&#x200B;**[!UICONTROL 投放]**&#x200B;菜单并单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;按钮。

1. 选择所需的自定义外部渠道，选择关联的模板，然后单击&#x200B;**[!UICONTROL 创建投放]**&#x200B;以进行确认。

   ![显示自定义投放创建的屏幕截图](assets/cus-create.png){zoomable="yes"}


1. 在&#x200B;**[!UICONTROL 属性]**&#x200B;下，输入投放的&#x200B;**[!UICONTROL 标签]**。

   ![显示自定义投放的属性配置的屏幕截图](assets/cus-properties.png){zoomable="yes"}

有关投放创建的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#create-delivery)。

## 定义受众{#select-audience}

现在，您需要定义提取文件将定向的受众。

1. 在投放页面的&#x200B;**[!UICONTROL 受众]**&#x200B;部分中，单击&#x200B;**[!UICONTROL 选择受众]**。

1. 选择现有受众或创建您自己的受众。

   ![显示自定义投放的受众选择的屏幕截图](assets/cc-audience2.png){zoomable="yes"}

有关受众定义的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#select-audience)。

## 编辑内容{#edit-content}

现在，让我们编辑将由自定义渠道投放生成的提取文件的内容。

1. 在投放页面中，单击&#x200B;**[!UICONTROL 编辑内容]**&#x200B;按钮。

1. 指定&#x200B;**[!UICONTROL 文件名]**，选择&#x200B;**[!UICONTROL 文件格式]**，然后根据需要为提取文件添加任意数量的列。

   ![显示提取文件属性配置选项的屏幕快照。](assets/cc-content-attributes.png)

有关内容版本的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#edit-content)。

## 预览并发送投放{#preview-send}

当投放内容准备就绪时，您可以使用测试用户档案预览该内容并发送校样。 然后，您可以发送投放以生成提取文件。

1. 在投放内容页面中，单击&#x200B;**[!UICONTROL 模拟内容]**&#x200B;按钮并选择测试配置文件。

   ![在投放内容页面中显示模拟内容选项的屏幕截图](assets/cus-simulate.png){zoomable="yes"}

1. 在投放页面中，单击&#x200B;**[!UICONTROL 审阅和发送]**，然后单击&#x200B;**[!UICONTROL 准备]**。 然后，确认。

   ![显示准备选项和日志菜单的屏幕快照](assets/cus-prepare.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 发送]**&#x200B;以继续执行最终发送过程，然后确认。

有关预览和发送的更多详细信息，请参阅呼叫中心[文档](../call-center/create-call-center.md#preview-send)。
