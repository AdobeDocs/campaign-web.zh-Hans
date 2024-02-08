---
solution: Journey Optimizer
product: journey optimizer
title: 登陆页面用例
description: 了解Journey Optimizer中登陆页面的最常见用例
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: 登录、登陆页面、用例
exl-id: 8c00d783-54a3-45d9-bd8f-4dc58804d922
source-git-commit: 601cc62c5640069ce9e6ee4830f924c610e0915f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 如何使用登陆页面 {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="复制URL时请务必谨慎"
>abstract="要完全测试或利用您的登陆页面，您不能将此链接直接复制粘贴到Web浏览器或投放中。 请改用 **模拟内容** 函数进行测试，并按照文档中描述的步骤正确使用登陆页面。"

要正确使用登陆页面，您应使用专用选项在投放中将其引用为链接。

>[!CAUTION]
>
>要充分利用登陆页面，您不能将已发布的投放仪表板中显示的链接直接复制粘贴到您的投放或网页中。

在 [!DNL Adobe Campaign Web] 下面，您可以使用四个现成的模板实施不同的用例。 但是，主要步骤保持不变，详见下文。

1. [创建登陆页面](create-lp.md#create-landing-page) 并根据用例选择您选择的模板：

   * [客户获取](#lp-acquisition)
   * [订阅](#lp-subscription)
   * [退订](#lp-unsubscription)
   * [阻止列表](#lp-denylist)

1. 定义登陆页面的属性和设置。

   ![](assets/lp-uc-properties.png)

1. 根据您的情况，选择 **[!UICONTROL 客户获取]**， **[!UICONTROL 订阅]**， **[!UICONTROL 退订]** 或 **[!UICONTROL 阻止列表]** 页面。

1. 将显示页面内容。 选择与登陆页面表单对应的部分。

   ![](assets/lp-uc-form.png)

1. 根据需要，对登陆页面标签和字段进行其他任意数量的更新。 根据需要编辑其余内容，保存更改并关闭。

1. 对于每种用例，请遵循以下详述步骤。

1. 编辑 **[!UICONTROL 确认]** 页面，以及 **[!UICONTROL 错误]** 和 **[!UICONTROL 过期]** 页数。 收件人提交注册表后，该屏幕即会显示。

   ![](assets/lp-uc-confirmation-page.png)

1. 测试和 [发布](create-lp.md#publish-landing-page) 您的登陆页面。

1. 创建 [电子邮件](../email/create-email.md) 以将流量引导至登陆页面的投放。

1. [插入链接](../email/message-tracking.md#insert-links) 放入您的消息内容。 选择 **[!UICONTROL 登陆页面]** 作为 **[!UICONTROL 链接类型]** 并选择 [登陆页面](create-lp.md#configure-primary-page) 你创造的。

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >要能够发送消息，请确保您选择的登陆页面尚未过期。 了解如何更新到期日期 [在此部分中](create-lp.md#create-landing-page).

收到电子邮件后，如果您的收件人单击登陆页面的链接并提交登陆页面表单，则他们将定向到确认页面，并应用登陆页面中定义的任何其他操作（例如，用户将订阅您的服务，或者不会收到您发送的任何其他通信）。

以下是如何使用的一些示例 [!DNL Adobe Campaign] 登陆页面，让您的客户选择启用/禁用接收您的部分或全部通信。

## 用户档案获取 {#lp-acquisition}

1. [创建登陆页面](create-lp.md#create-landing-page). 选择 **[!UICONTROL 客户获取]** 模板。

1. 定义登陆页面的属性和设置。

   ![](assets/lp-uc-properties.png)

1. 选择 **[!UICONTROL 客户获取]** 页面以编辑其内容。

1. 将显示页面内容。 选择与登陆页面表单对应的部分。

## 订阅服务 {#lp-subscription}

最常见的用例之一是邀请您的客户 [订购服务](../audience/manage-services.md) （例如新闻稿或活动）。 请按照以下步骤操作。

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. 首先，为订阅事件的用户创建确认模板，以便在创建服务时可以轻松选择它。 [了解详情](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. 创建订阅服务，该服务会将已注册的用户存储到您的事件中。 [了解如何创建服务](../audience/manage-services.md)

1. 选择您创建的模板，作为用户订阅时将收到的确认电子邮件。

   ![](assets/lp-uc-subscription-service.png)

1. [创建登陆页面](create-lp.md#create-landing-page) 以使您的收件人能够注册您的事件。 选择 **[!UICONTROL 订阅]** 模板。

   <!--![](assets/lp-uc-subscription-template.png)-->

1. 定义登陆页面的属性和设置。

   <!--![](assets/lp-uc-properties.png)-->

1. 选择 **[!UICONTROL 订阅]** 页面以编辑其内容。

   ![](assets/lp-uc-subscription-page-edit.png)

1. 将显示页面内容。 选择与登陆页面表单对应的部分，然后展开 **[!UICONTROL 复选框1]** 部分。

   在 **[!UICONTROL 订阅和服务]** 字段中，选择为事件创建的服务。 离开 **[!UICONTROL 如果选中，则订阅]** 选项已启用。

   ![](assets/lp-uc-subscription-checkbox-1.png)

1. 例如，您可以添加其他复选框以提供对您的新闻稿的订阅。

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. 根据需要，对登陆页面标签和字段进行其他任意数量的更新。 根据需要编辑其余内容，保存更改并关闭。

1. 编辑 **[!UICONTROL 确认]** 页面，以及 **[!UICONTROL 错误]** 和 **[!UICONTROL 过期]** 页数。 收件人提交注册表后，该屏幕即会显示。

   ![](assets/lp-uc-confirmation-page.png)

1. 测试和 [发布](create-lp.md#publish-landing-page) 您的登陆页面。

1. 创建 **电子邮件** 投放，以将流量引向注册登陆页面。 设计电子邮件以宣布您的活动现已开放注册。

1. [插入链接](../email/message-tracking.md#insert-links) 放入您的消息内容。 选择 **[!UICONTROL 登陆页面]** 作为 **[!UICONTROL 链接类型]** 并选择 [登陆页面](create-lp.md#configure-primary-page) 您为注册而创建的。

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >要能够发送消息，请确保您选择的登陆页面尚未过期。 了解如何更新到期日期 [在此部分中](create-lp.md#create-landing-page).

收到电子邮件后，如果您的收件人单击登陆页面的链接并提交登陆页面表单，则他们将被定向到确认页面，并将被添加到订阅列表。

## 退订 {#lp-unsubscription}

1. [创建登陆页面](create-lp.md#create-landing-page). 选择 **[!UICONTROL 退订]** 模板。

1. 定义登陆页面的属性和设置。

1. 选择 **[!UICONTROL 退订]** 页面以编辑其内容。

1. 将显示页面内容。 选择与登陆页面表单对应的部分。

## 设置选择退出登陆页面 {#lp-denylist}

向收件人提供取消从品牌接收通信的功能是一项法律要求。 进一步了解 [Experience Platform文档](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html#regulations){target="_blank"}.

因此，您必须始终包含 **取消订阅链接** 在发送给收件人的每封电子邮件中：

* 单击此链接后，收件人将被定向到一个包含确认选择退出的按钮的登陆页面。
* 单击选择退出按钮后，用户档案数据将使用此信息更新。

您可以设置 **[!UICONTROL 阻止列表]** 使用户能够选择退出所有投放的登陆页面。

要使用户能够选择退出所有投放，您必须创建和发布 **[!UICONTROL 阻止列表]** 登陆页面。

一旦用户单击登陆页面链接， **[!UICONTROL 不再联系（通过任何渠道）]** 配置文件中的选项将被自动选中。

![](assets/blocklisting_allchannels.png)

定义 **[!UICONTROL 选择退出]** 复选框，然后选择以更新 **[!UICONTROL 渠道（电子邮件）]**：选中登陆页面上的选择退出框的配置文件将退出您的所有通信。

收到消息后，如果收件人单击电子邮件中的取消订阅链接，则会显示您的登陆页面。

![](assets/lp_opt-out-submit-form.png)

如果收件人选中该框并提交表单：

* 选择退出的收件人将被重定向至确认消息屏幕。

* 配置文件数据已更新，除非再次订阅，否则将不会收到您品牌的通信。

要检查相应用户档案的选择是否已更新，请转到“用户档案”并选择用户档案。







