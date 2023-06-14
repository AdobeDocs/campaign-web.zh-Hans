---
audience: end-user
title: 发送优惠
description: 发送优惠
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha"
source-git-commit: a66fe155aa1543d53c3ba1b5620159240d50bf3a
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 94%

---


# 发送优惠 {#offers-content}

Adobe Campaign v8 Web 可让您使用&#x200B;**[!UICONTROL 交互]**&#x200B;模块通过电子邮件发送已在控制台中创建的优惠。有关交互以及如何在控制台中管理优惠目录的更多信息，请参阅 [Campaign v8 文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}。

使用电子邮件发送优惠的步骤如下：

1. [配置要提议的优惠](#configure)，
1. [将优惠插入电子邮件中](#insert)。

## 配置要推荐的优惠 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="优惠设置"
>abstract="配置应向收件人推荐的优惠。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="优惠高级设置"
>abstract="配置优惠的高级选项。"

1. 如果要选择要在电子邮件中推荐的优惠，请单击电子邮件内容编辑屏幕中的&#x200B;**[!UICONTROL 优惠]**&#x200B;按钮。

   ![](assets/setup-offers.png)

1. 配置应向收件人推荐的优惠。首先，选择与优惠环境匹配的&#x200B;**[!UICONTROL 优惠空间]**。

   ![](assets/create-content-offers.png)

1. 要细化引擎的优惠选择，请选择已在其中对优惠排序的特定&#x200B;**[!UICONTROL 优惠类别]**。选择文件夹时，会自动包含所有子文件夹，并且无法将其删除。 请注意，UI不会反映此行为。

   如果未指定类别，除非已选中&#x200B;**[!UICONTROL 优惠主题]**，否则优惠引擎将考虑环境中包含的所有优惠。

1. （可选）输入主题以筛选类别。 主题是在类别上游定义的关键字。它们充当筛选器，可让您通过在一组类别中选择优惠来细化要显示的优惠数量。

1. 使用&#x200B;**[!UICONTROL 建议]**&#x200B;字段可指定要插入电子邮件中的优惠数量。

1. 如有必要，可以选择&#x200B;**[!UICONTROL 排除不符合条件的收件人]**&#x200B;选项。

   使用此选项，您可以激活或停用排除不具有足量合格优惠的收件人的操作。

   * 如果启用此选项，则将从投放中排除不具有足量建议的收件人。
   * 如果禁用此选项，则不会排除这些收件人，但他们无法拥有请求的建议数量。

1. 如有必要，可以选择&#x200B;**[!UICONTROL 如果未选择任何优惠，则隐藏所有内容]**&#x200B;选项。

   此选项可让您选择在某个建议不存在的情况下处理消息的方式。

   * 如果启用此选项，则不会显示缺失建议的表示形式，并且此建议的消息中不会显示任何内容。
   * 如果禁用此选项，则消息本身将在发送过程中被取消，并且收件人再也无法收到任何消息。

配置要在电子邮件中推荐的优惠后，可以使用表达式编辑器将这些优惠插入到电子邮件中。[了解如何将优惠插入电子邮件中](#insert)

## 将优惠插入电子邮件中 {#insert}

可以使用表达式编辑器将优惠添加到电子邮件中。可以将优惠插入以下位置：

* 电子邮件主题行，
* 电子邮件正文中（通过允许在任意内容组件中进行个性化）。[了解如何添加内容组件](content-components.md)

>[!NOTE]
>
>在插入优惠之前，请确保您[已配置要通过电子邮件推荐的优惠](#configure)。

要使用表达式编辑器插入优惠，请执行以下步骤：

1. 打开表达式编辑器，然后选择&#x200B;**[!UICONTROL 建议]**&#x200B;菜单。

   可用的建议将显示在列表中。建议的数量是在配置要推荐的优惠时定义的。

   ![](assets/offer-insertion.png)

1. 使用对每个建议可用的个性化字段、渲染功能或优惠属性，将建议添加到电子邮件主题或正文中。

   ![](assets/offer-inserted.png)
