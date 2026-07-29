---
audience: end-user
title: 将可编辑列表添加到选件架构
description: 了解如何直接在选件详细信息屏幕中将自定义收藏集链接显示为可编辑列表。
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 1%

---

# 将可编辑列表添加到选件架构 {#offer-editable-list}

当您使用自定义收藏集链接（例如链接到选件的一组区段）扩展 [!DNL nms:offer] 架构](../administration/schemas.md)时，可以直接在选件的&#x200B;**[!UICONTROL 自定义选项]**&#x200B;部分中将其显示为可编辑列表。 [收藏集不是通过单独的屏幕管理相关记录，而是呈现为选件详细信息中的列表，您可以通过专用对话框内联创建新的相关记录。

>[!NOTE]
>
>此功能当前仅适用于选件架构。

## 添加收藏集链接字段 {#add-field}

1. 使用自定义收藏集扩展[!DNL nms:offer]架构，然后浏览到&#x200B;**[!UICONTROL 架构]**&#x200B;菜单，打开&#x200B;**[!UICONTROL 营销优惠]**&#x200B;架构，然后单击&#x200B;**[!UICONTROL 屏幕版本]**。 [了解详情](../administration/schemas-browse-access.md#screen-def)。

   ![显示屏幕定义按钮的屏幕截图。](assets/offers-editable-list.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 详细信息屏幕配置]**&#x200B;部分中，单击&#x200B;**[!UICONTROL 自定义字段列表]**&#x200B;表上方的省略号图标，然后选择&#x200B;**[!UICONTROL 选择属性]**。 [了解详情](../administration/schemas-custom-fields.md)。

   ![显示屏幕定义按钮的屏幕截图。](assets/offers-editable-list-0.png){zoomable="yes"}

1. 浏览属性并选择您的自定义收藏集链接，该链接由其收藏集图标标识。

   ![显示具有集合链接属性的属性选取器的屏幕截图。](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >集合链接字段无法设为必填字段，并且不支持子属性。 默认情况下，它们跨越表单中的两列。

1. 确认您的选择。 收藏集链接已添加到自定义字段&#x200B;]**表的**[!UICONTROL &#x200B;列表，其类型为&#x200B;**[!UICONTROL 收藏集]**。

   ![显示已添加属性的屏幕截图。](assets/offers-editable-list-2.png){zoomable="yes"}

## 配置收藏集的可编辑列表 {#configure-list}

1. 单击收藏集字段行上的省略号图标，然后选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以打开&#x200B;**[!UICONTROL 收藏集链接设置]**&#x200B;对话框。

   ![显示编辑按钮的屏幕截图。](assets/offers-editable-list-3.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 常规]**&#x200B;选项卡中，可以选择设置&#x200B;**[!UICONTROL Visible if]**&#x200B;条件，或启用&#x200B;**[!UICONTROL 只读]**。

   ![显示版本屏幕的屏幕截图。](assets/offers-editable-list-4.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 屏幕配置]**&#x200B;选项卡中，单击&#x200B;**[!UICONTROL 选择属性]**&#x200B;并选择将新元素添加到列表时要使用的属性，例如区段名称和自定义字段。

   ![显示集合链接设置对话框的屏幕配置选项卡的屏幕截图。](assets/offers-editable-list-5.png){zoomable="yes"}

1. 在&#x200B;**[!UICONTROL 布局]**&#x200B;选项卡中，保留或清除&#x200B;**[!UICONTROL 跨越两列]**。

1. 单击&#x200B;**[!UICONTROL 确认]**，然后单击&#x200B;**[!UICONTROL 保存]**&#x200B;屏幕定义。

## 在选件中使用可编辑列表 {#use-list}

1. 从左侧菜单中，单击&#x200B;**选件**&#x200B;并打开一个选件。 [了解更多信息](create-offer.md#create)

   ![显示选件屏幕的屏幕截图。](assets/offers-editable-list-7.png){zoomable="yes"}

1. 访问选件属性。 该收藏集在&#x200B;**自定义选项**&#x200B;部分中呈现为列表。

   ![在选件详细信息屏幕中显示可编辑列表渲染的屏幕快照。](assets/offers-editable-list-6.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 添加]**&#x200B;以显示您配置的属性，填写这些属性，然后单击&#x200B;**[!UICONTROL 确认]**。 新元素即添加到列表中。

   您可以将多个元素添加到同一列表，并且选件详细信息可包含多个可编辑列表。

1. 单击&#x200B;**[!UICONTROL 保存]**。

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->