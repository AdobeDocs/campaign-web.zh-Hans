---
title: 自定义字段
description: 了解如何配置自定义字段
hide: true
hidefromtoc: true
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: 3f4b2c83b5c651e473de9e32656aaf83af6fe8c6
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# 配置自定义字段 {#custom-fields}

自定义字段是通过Adobe Campaign控制台添加到现成模式的其他属性。 在中了解详情 [Adobe Campaign v8文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

这些自定义字段会显示在各种屏幕中，例如用户档案或测试用户档案的详细信息。

在Web用户界面中，不能创建自定义字段，但可以修改其显示方式。 修改适用于所有Campaign用户。

>[!NOTE]
>
>您需要具有管理员权限才能修改自定义字段。

自定义字段在以下架构中可用：

* 收件人(nms)
* 营销活动(nms)
* 投放(nms)
* 种子地址(nms)

要配置自定义字段，请执行以下步骤：

1. 下 **管理**，单击 **架构**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. 找到所需的架构，例如 **收件人(nms)** 架构。

   ![](assets/custom-fields2.png){zoomable="yes"}

1. 单击 **更多操作** 按钮并选择 **编辑自定义详细信息**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   此 **编辑自定义详细信息** 屏幕显示所有自定义字段及其类型。

   ![](assets/custom-fields4.png){zoomable="yes"}

   在此屏幕中，您可以执行以下操作：

   * 使用向上和向下箭头更改不同字段的顺序。
   * 将字段设为必填：选中 **必需** 盒子。
   * 使字段可见或隐藏：单击 **可见** 按钮。
   * 添加可见性条件：单击 **可见，如果** 按钮并使用可用的xtk函数编写xtk表达式。

1. 导航到显示自定义字段的屏幕。 在我们的示例中，显示的是配置文件详细信息屏幕。

   ![](assets/custom-fields5.png){zoomable="yes"}
