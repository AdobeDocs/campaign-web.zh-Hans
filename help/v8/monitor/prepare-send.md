---
audience: end-user
title: 准备并发送电子邮件
description: 了解如何使用 Campaign Web UI 准备并发送电子邮件
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Alpha" type="Positive"
source-git-commit: 7a58b8323dbecc7cca0ba513d98a5afb213d3bc2
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 96%

---


# 准备并发送您的电子邮件 {#prepare-send}


<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 准备发送{#prepare}

在定义了内容、受众和计划后，便可以准备您的邮件了。在准备期间，计算目标人群并为目标中包含的每个配置文件生成邮件内容。在准备工作完成后，可以立即发送邮件，也可以在计划的日期和时间发送。

投放准备期间使用的验证规则在中进行了描述 [Campaign v8 （控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/validate/delivery-analysis.html){target="_blank"}.

按照下面的步骤进行操作：

1. 在投放仪表板中，单击右上角的&#x200B;**准备**&#x200B;按钮并进行确认。

   ![](assets/prepare.png)

   这将显示准备进度。根据目标人群的规模，此操作可能需要花费一些时间。

   >[!NOTE]
   >
   >您可以随时使用&#x200B;**停止准备**&#x200B;按钮来停止准备过程。在准备阶段，不发送任何邮件。因此，您可以开始或停止准备而不影响任何内容。

1. 在准备完成后，检查 KPI。如果要发送的邮件数不符合您的期望，请修改您的受众并重新开始准备。

   ![](assets/prepare2.png)

   以下是显示的不同 KPI：

   * **定位**：目标收件人的数量
   * **投放**：将发送的邮件数
   * **排除**：由类型规则排除的邮件数

1. 单击&#x200B;**日志**&#x200B;按钮并检查确认没有错误。最后一条日志消息显示了所有错误消息和错误数。有关更多信息，请参阅[此章节](delivery-logs.md)。

   ![](assets/prepare-logs.png)

如果准备阶段检测到阻止发送投放的严重错误，则准备状态在投放仪表板中显示为失败。

![](assets/prepare-error.png)

如果您在准备好后需要对投放进行任何更改，则需要重新开始准备以使这些更改生效。

在准备工作完成且未出现错误后，便可发送邮件。有关更多信息，请参阅[此章节](#send)。

## 发送邮件{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="已送达"
>abstract="成功送达的邮件数。该指示器每 5 分钟更新一次。显示的百分比是基于已发送邮件的总数计算所得。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="打开"
>abstract="打开的邮件数。该指示器每 5 分钟更新一次。显示的百分比是不同打开次数与已送达邮件数的比率。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="单击次数"
>abstract="在电子邮件中至少单击一次的收件人的数目。该指示器每 5 分钟更新一次。显示的百分比是不同单击次数与已送达邮件数的比率。"


准备工作完成后，您现在可以发送邮件。仅立即发送的邮件需要执行此步骤。如果已计划邮件的发送日期，则它会在定义的日期发送。

执行以下步骤：

1. 从投放仪表板中，单击右上角的&#x200B;**发送**&#x200B;按钮并进行确认。

   ![](assets/send.png)

1. 这将显示发送进度。检查显示的 KPI。您也可以查看日志。有关更多信息，请参阅[此章节](delivery-logs.md)。

   ![](assets/send2.png)

   以下是显示的不同 KPI：

   * **已送达**：成功送达的邮件数。显示的百分比是基于已发送邮件的总数计算所得。
   * **打开**：打开的邮件数。显示的百分比是不同打开次数与已送达邮件数的比率。
   * **单击次数**：在电子邮件中至少单击一次的收件人的数目。显示的百分比是不同单击次数与已送达邮件数的比率。

   >[!NOTE]
   >
   >在投放开始后，所有指标每 5 分钟更新一次。投放准备指标是实时计算的。

   您可以随时暂停发送，随后将其恢复。如果您在发送过程中停止投放，则无法恢复。
