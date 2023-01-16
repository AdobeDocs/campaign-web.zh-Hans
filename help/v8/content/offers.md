---
audience: end-user
title: 发送选件
description: 发送选件
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: de7f135b9ac25c5fe13df6a4033d8ef53d081e44
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# 发送选件 {#offers-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="选件设置"
>abstract="热障涂层"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="选件高级设置"
>abstract="热障涂层"

Adobe Campaign v8 Web允许您使用 **[!UICONTROL 互动]** 模块。 有关交互以及如何在控制台中管理优惠目录的更多信息，请参阅 [Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

通过电子邮件发送选件的步骤如下所示：

1. [配置要建议的选件](#configure),
1. [将选件插入电子邮件](#insert).

## 配置要建议的选件 {#configure}

1. 要选择要在电子邮件中建议的选件，请单击 **[!UICONTROL 选件]** 按钮。

   ![](assets/setup-offers.png)

1. 配置应向收件人建议的选件。 首先，选择 **[!UICONTROL 选件空间]** 与选件环境匹配的选件。

   ![](assets/create-content-offers.png)

1. 要优化引擎的选件选择，请选择 **[!UICONTROL 选件类别]** 其中选件进行了排序。

   如果未指定类别，则环境中包含的所有选件都将由选件引擎考虑，除非 **[!UICONTROL 选件主题]** 中。

   >[!NOTE]
   >
   >主题是在类别中上游定义的关键词。 它们充当过滤器，允许您通过在一组类别中选择选件来优化要显示的选件数量。

1. 使用 **[!UICONTROL 建议]** 字段以指定要插入到电子邮件中的选件数量。

1. 选择 **[!UICONTROL 排除不符合条件的收件人]** 选项。

   利用此选项，可激活或取消激活排除符合条件的选件不足的收件人。

   * 如果启用了选项，则投放中将排除没有足够建议的收件人。
   * 如果禁用了该选项，则不会排除这些收件人，但他们将没有请求的建议数。

1. 如有必要，请选择 **[!UICONTROL 未选择选件时隐藏所有内容]** 选项。

   此选项允许您选择在其中一个命题不存在时如何处理消息。

   * 如果启用了选项，则不会显示缺少命题的表示形式，并且此命题的消息中将不显示任何内容。
   * 如果禁用了选项，则在发送期间将取消消息本身，收件人将不再收到任何消息。

将选件配置为在电子邮件中建议后，您可以使用表达式编辑器将其插入到电子邮件中。 [了解如何在电子邮件中插入选件](#insert)

## 将选件插入电子邮件 {#insert}

可以使用表达式编辑器将选件添加到电子邮件中。 可以插入以下任一项：

* 在电子邮件主题行中，
* 通过允许在任何内容组件中进行个性化，在电子邮件正文中显示。 [了解如何添加内容组件](content-components.md)

>[!NOTE]
>
>在插入选件之前，请确保您已 [配置了要与电子邮件一起建议的选件](#configure).

要使用表达式编辑器插入选件，请执行以下步骤：

1. 打开表达式编辑器，然后选择 **[!UICONTROL 建议]** 菜单。

   可用的建议将显示在列表中。 在配置要建议的选件时定义建议的数量。

   ![](assets/offer-insertion.png)

1. 使用个性化字段、呈现函数或每个建议可用的选件属性，将建议添加到电子邮件主题或正文中。

   ![](assets/offer-inserted.png)
