---
audience: end-user
title: 使用连续投放工作流活动
description: 了解如何使用连续投放工作流活动
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 3%

---

# 持续投放 {#continuous-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="连续投放活动"
>abstract="您现在可以向现有投放添加新收件人。 此投放类型可避免每次都创建新投放，从而更有效地根据需要发送低流量警报或通知。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

**连续投放**&#x200B;活动允许您向现有投放添加新收件人。 此投放类型可避免每次都创建新投放，从而更有效地根据需要发送低流量警报或通知。

连续投放会创建单个投放实例。 所有投放日志(broadLog)和跟踪日志都引用此一次投放，从而简化了监控和报告。

## 配置连续投放活动 {#configure}

1. 将&#x200B;**连续投放**&#x200B;活动添加到您的工作流画布。

   ![显示连续投放活动的屏幕截图](../assets/continuous-delivery.png){zoomable="yes"}

1. 为活动输入自定义&#x200B;**[!UICONTROL 标签]**（可选）。 默认情况下，它标记为“持续交付”。

1. 在&#x200B;**[!UICONTROL 模板]**&#x200B;字段旁边，单击搜索图标以选择投放模板。 只能选择模板（而非标准投放）。 模板定义投放渠道、内容和配置。

1. 在&#x200B;**[!UICONTROL 定位选项]**&#x200B;中，选择如何定义目标群体：

   * **[!UICONTROL 由入站事件指定]**：目标来自入站过渡（来自上游活动，如生成受众或增量查询）。 这是最常见的选项。

   * 在投放模板&#x200B;**[!UICONTROL 中指定]**：目标在模板本身中定义。

   * **[!UICONTROL 在输入事件中指定的文件]**：目标是通过工作流传递的文件提供的。

连续投放活动会自动生成叫客过渡以继续您的工作流。

## 相关主题 {#related}

* [关于工作流活动](about-activities.md)
* [电子邮件、短信、推送、直邮活动](channels.md)
* [投放模板](../../msg/delivery-template.md)
