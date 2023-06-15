---
audience: end-user
title: 发送优惠
description: 发送优惠
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha"
source-git-commit: a653fe4329f449a94f8056e4b5f2247bd839b87a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 发送优惠 {#offers-content}

Adobe Campaign v8 Web允许您使用在控制台中创建的投放选件进行发送。 **[!UICONTROL 互动]** 模块。 有关交互以及如何在控制台中管理优惠目录的详细信息，请参阅 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

通过投放发送优惠的步骤如下：

1. [配置要推荐的优惠](#configure)
1. [将优惠插入到投放中](#insert)

## 配置要推荐的优惠 {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="优惠设置"
>abstract="配置应向收件人推荐的优惠。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="提供高级设置"
>abstract="配置优惠的高级选项。"

1. 要选择要在投放中建议的优惠，请单击 **[!UICONTROL 设置优惠]** 按钮。

   ![](assets/setup-offers.png)

1. 配置应向收件人推荐的优惠。

   首先，选择与优惠环境匹配的&#x200B;**[!UICONTROL 优惠空间]**。了解如何在中创建优惠空间 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}

   ![](assets/create-content-offers.png)

1. 要细化引擎的优惠选择，请选择已在其中对优惠排序的特定&#x200B;**[!UICONTROL 优惠类别]**。

   选择文件夹时，会自动包含所有子文件夹，并且无法将其删除。 请注意 [!DNL Campaign] 界面不反映此行为。

   >[!NOTE]
   >
   >如果未指定类别，除非已选中&#x200B;**[!UICONTROL 优惠主题]**，否则优惠引擎将考虑环境中包含的所有优惠。

1. （可选）输入主题以筛选类别。 主题是在类别上游定义的关键字。它们充当筛选器，可让您通过在一组类别中选择优惠来细化要显示的优惠数量。

1. 使用 **[!UICONTROL 建议]** 字段，用于指定要插入到投放中的优惠数量。

1. 如有必要，可以选择&#x200B;**[!UICONTROL 排除不符合条件的收件人]**&#x200B;选项。

   使用此选项，您可以激活或停用排除不具有足量合格优惠的收件人的操作。

   * 如果启用此选项，则将从投放中排除不具有足量建议的收件人。
   * 如果禁用此选项，则不会排除这些收件人，但他们无法拥有请求的建议数量。

1. 如有必要，可以选择&#x200B;**[!UICONTROL 如果未选择任何优惠，则隐藏所有内容]**&#x200B;选项。

   此选项可让您选择在某个建议不存在的情况下处理消息的方式。

   * 如果启用此选项，则不会显示缺失建议的表示形式，并且此建议的消息中不会显示任何内容。
   * 如果禁用此选项，则消息本身将在发送过程中被取消，并且收件人再也无法收到任何消息。

将优惠配置为在投放中建议后，可以使用表达式编辑器将它们插入到投放内容中。

## 将优惠插入到投放中 {#insert}

可以使用将选件添加到投放中 [表达式编辑器](../personalization/gs-personalization.md#access). 它们可以插入主题行或投放正文中。

>[!CAUTION]
>
>在将选件插入投放之前，请确保已 [已配置要在该投放中建议哪些优惠](#configure).

要使用表达式编辑器插入选件，请执行以下步骤。

1. 访问任何投放的主题行或内容。

1. 将鼠标光标放在要插入选件的位置，然后使用个性化图标打开表达式编辑器。

1. 选择 **[!UICONTROL 建议]** 菜单。 可用的建议将显示在列表中。

   >[!NOTE]
   >
   >在以下情况下定义建议数量： [设置优惠](#configure) 用于当前投放。

   ![](assets/offer-insertion.png)

1. 使用每个建议可用的个性化字段、渲染函数或优惠属性，将建议添加到投放主题行或正文中。

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >可用建议的数目取决于引擎调用的配置方式，其顺序取决于优惠的优先级。

1. 保存您的更改。

1. 完成内容、测试并发送投放。

现在，当收件人收到投放时，将会为该特定用户档案显示正确的优惠。
