---
audience: end-user
title: 在消息中添加优惠
description: 了解如何添加和发送优惠
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Beta"
source-git-commit: 6406be82c2bad9346f6743e18535fdfe132b2bd0
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 33%

---


# 在消息中添加优惠 {#offers-content}

Adobe Campaign v8 Web允许您使用在控制台中创建的投放选件进行发送。 **[!UICONTROL 互动]** 模块。 有关交互以及如何在控制台中管理优惠目录的更多信息，请参阅 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

通过投放发送优惠的步骤如下：

1. [配置要推荐的优惠](#configure)
1. [将优惠插入投放](#insert)

## 配置要推荐的优惠 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="定义优惠参数"
>abstract="通过定义优惠空间（可选类别和主题）来配置应向收件人建议的优惠，并指定要插入到投放中的优惠数量。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="设置选件高级设置"
>abstract="您可以启用排除没有足够合格选件的收件人，并选择在某个建议不存在时如何处理消息。"

利用Adobe Campaign，可向给定联系人建议一个或多个特定优惠。 交互模块，用于在交互期间通过向给定联系人建议单个或多个特定优惠来实时响应他们。 这些优惠可以是简单的通信消息、针对一个或多个产品或服务的特别优惠。

要选择要添加到投放的优惠，请执行以下步骤。

1. 单击 **[!UICONTROL 设置优惠]** 按钮。

   ![](assets/setup-offers.png)

1. 配置应向收件人推荐的优惠。

   首先，选择与优惠环境匹配的&#x200B;**[!UICONTROL 优惠空间]**。了解如何在中创建优惠空间 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}

   ![](assets/create-content-offers.png)

1. 要细化引擎的优惠选择，请选择已在其中对优惠排序的特定&#x200B;**[!UICONTROL 优惠类别]**。

   选择文件夹时，会自动包含所有子文件夹，并且无法将其删除。 请注意 [!DNL Campaign] 接口不反映此行为。

   >[!NOTE]
   >
   >如果未指定类别，除非已选中&#x200B;**[!UICONTROL 优惠主题]**，否则优惠引擎将考虑环境中包含的所有优惠。

1. （可选）输入主题以筛选类别。 主题是在类别上游定义的关键字。它们充当筛选器，可让您通过在一组类别中选择优惠来细化要显示的优惠数量。

1. 使用 **[!UICONTROL 建议]** 字段，用于指定要插入到投放中的选件数量。

1. 如有必要，可以选择&#x200B;**[!UICONTROL 排除不符合条件的收件人]**&#x200B;选项。

   使用此选项，您可以激活或停用排除不具有足量合格优惠的收件人的操作。

   * 如果启用此选项，则将从投放中排除不具有足量建议的收件人。
   * 如果禁用此选项，则不会排除这些收件人，但他们无法拥有请求的建议数量。

1. 如有必要，可以选择&#x200B;**[!UICONTROL 如果未选择任何优惠，则隐藏所有内容]**&#x200B;选项。

   此选项可让您选择在某个建议不存在的情况下处理消息的方式。

   * 如果启用此选项，则不会显示缺失建议的表示形式，并且此建议的消息中不会显示任何内容。
   * 如果禁用此选项，则消息本身将在发送过程中被取消，并且收件人再也无法收到任何消息。

将优惠配置为在投放中建议后，可以使用表达式编辑器将它们插入到投放内容中。

## 将优惠插入投放 {#insert}

可使用将优惠添加到投放中 [表达式编辑器](../personalization/gs-personalization.md#access). 可以将它们插入主题行或投放正文中。

>[!CAUTION]
>
>在将选件插入投放之前，请确保已 [已配置要在该投放中建议哪些优惠](#configure).

要使用表达式编辑器插入选件，请执行以下步骤。

1. 访问任何投放的主题行或内容。

1. 将鼠标光标放在要插入选件的位置，然后使用个性化图标打开表达式编辑器。

1. 选择 **[!UICONTROL 建议]** 菜单。 可用的建议将显示在列表中。

   >[!NOTE]
   >
   >在以下情况下定义建议数量 [设置优惠](#configure) 当前投放的。

   ![](assets/offer-insertion.png)

1. 使用可用于每个建议的个性化字段、渲染函数或优惠属性，将建议添加到投放主题行或正文中。

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >可用建议的数目取决于引擎调用的配置方式，其顺序取决于优惠的优先级。 在中了解详情 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. 保存您的更改。

1. 完成内容，测试并发送投放。

现在，当收件人收到投放时，将会向该特定用户档案显示正确的优惠。
