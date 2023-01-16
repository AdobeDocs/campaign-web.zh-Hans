---
audience: end-user
title: 发送测试电子邮件
description: 了解如何定义和发送测试电子邮件
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 8438c7ab35c2423beddbb36db2fcf52f661876bf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# 发送测试电子邮件 {#send-proofs}

![](../assets/do-not-localize/badge.png)

发送测试电子邮件是验证电子邮件促销活动并确定潜在问题的重要步骤。 通过发送测试电子邮件，您可以检查各种元素，如链接、选择退出链接、图像和镜像页面，并检测任何错误。

测试电子邮件可发送给两种类型的收件人：

* **测试用户档案**:向种子地址发送测试电子邮件，种子地址是数据库中其他虚构的收件人，
* **替换用户档案**:模拟现有用户档案时，向特定电子邮件地址发送测试电子邮件。 这样，您就可以像收件人一样体验电子邮件，从而准确呈现用户档案将收到的消息。

## 选择校样收件人 {#recipients}

1. 访问电子邮件内容创建屏幕，然后单击 **[!UICONTROL 模拟内容]**.

1. 单击 **[!UICONTROL 测试]** 按钮，然后使用 **[!UICONTROL 模式]** 下拉列表中选择要接收校样的收件人类型：

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### 向测试用户档案发送校样

1. 选择 **[!UICONTROL 使用测试用户档案]** 模式。

1. 添加将接收测试电子邮件的测试用户档案。

   <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

   ![](assets/test-profiles-audience.png)

### 向替换用户档案发送校样

1. 选择 **[!UICONTROL 目标替换]** 模式。

1. 添加将接收校样的电子邮件地址。

   >[!NOTE]
   >
   >您可以指定任何电子邮件地址。 这样，即使用户不是Adobe Campaign V8用户，您也可以向其发送校样。

1. 对于每个电子邮件地址，从目标中选择要使用的用户档案。 您还可以让Adobe Campaign从目标中选择一个随机配置文件。

   ![](assets/substitution.png)

选择校样收件人后，您可以发送测试电子邮件。 [了解如何发送校样](#send)

>[!NOTE]
>
>如果要向校样的收件人发送最终电子邮件，请启用 **[!UICONTROL 在主目标中包含测试群体]** 选项。

## 发送校样 {#send}

要将校样发送给选定的收件人，请单击 **[!UICONTROL 发送测试电子邮件]** 然后确认发送。

![](assets/send-proof.png)

发送所需数量的校样，直到完成投放的内容为止。 完成此操作后，您可以向主目标发送电子邮件。 [了解如何准备和发送电子邮件](../monitor/prepare-send.md)

## 访问发送的校样 {#access-proofs}

发送校样后，即可从 **[!UICONTROL 查看测试电子邮件日志]** 按钮。 利用这些日志，可访问为选定投放发送的所有校样，并可视化与其发送相关的特定统计信息。

![](assets/proof-log.png)

您还可以从投放列表（如任何投放）访问校样。

![](assets/delivery-list.png)
