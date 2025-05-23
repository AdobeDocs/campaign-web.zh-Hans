---
title: 创建轮廓
description: 了解如何在Campaign Web中创建用户档案。
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 46%

---

# 创建轮廓 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="基本详细信息"
>abstract="本节深入介绍了轮廓的基本详细信息。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="联系人信息"
>abstract="本节深入介绍了轮廓的联系信息。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="地址"
>abstract="本节深入介绍轮廓的邮政地址和地址质量。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="帐户详细信息"
>abstract="本节深入介绍轮廓的帐户详细信息。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="不再是联系人"
>abstract="本节深入介绍轮廓的联系偏好设置。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="自定义字段"
>abstract="自定义字段是根据您需求定制并为您实例配置的特定属性。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="其他 "
>abstract="本节提供额外的内置属性。要修改任何信息，请直接在相应字段中进行更改，然后单击屏幕右上角的&#x200B;**保存**&#x200B;按钮。"

要创建配置文件，请执行以下步骤：

1. 导航到&#x200B;**[!UICONTROL 客户管理]** > **[!UICONTROL 配置文件]**，然后单击屏幕右上角的&#x200B;**[!UICONTROL 创建配置文件]**&#x200B;按钮。

1. 此时将显示配置文件可用的属性列表，这些属性分为下表详述的不同部分。

   ![显示配置文件可用属性列表的屏幕截图，这些属性按章节](assets/create-profile.png){zoomable="yes"}

   | “属性”部分 | 说明 |
   |  ---  |  ---  |
   | **基本详细信息** | 个人资料的基本信息，如姓名或出生日期。<br/>默认情况下，配置文件存储在&#x200B;**[!UICONTROL 收件人]**&#x200B;文件夹中。 您可以通过浏览到所需的位置来更改它。 [了解如何使用文件夹](../get-started/permissions.md#folders) |
   | **联系信息** | 用户档案的联系信息，如电子邮件地址或电话号码。 |
   | **地址** | 用户档案的邮政地址。 此部分还提供地址质量的评估。 如果指定了“姓氏”、“城市”和“邮政编码”字段，则会将用户档案的地址视为有效。 |
   | **帐户详细信息** | 用户档案帐户的信息，如状态或帐号。 |
   | **不再联系** | 配置文件的联系人首选项。 当选取这些选项中的任何一个选项时，配置文件都会处于阻止列表中。<br/>例如，如果收件人点击了新闻稿中的退订链接，此信息将添加到联系人数据中。 此类收件人不再位于所选渠道中。 请参阅[Adobe Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=zh-Hans){target="_blank"}以了解有关隔离管理的更多信息 |
   | **自定义字段** | 如果自定义字段已配置，则会显示在此部分中。 自定义字段是通过Adobe Campaign控制台添加到&#x200B;**[!UICONTROL 配置文件]**&#x200B;架构的其他属性。 请参阅[Adobe Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=zh-Hans){target="_blank"}以了解详情 |
   | **其他** | 其他内置属性。 |

1. 配置配置文件后，单击&#x200B;**[!UICONTROL 创建]**&#x200B;以将其保存到数据库中。

   保存后，可随时从用户档案列表中打开该用户档案以进行编辑。 [了解如何浏览用户档案的详细信息](profile-view.md)。