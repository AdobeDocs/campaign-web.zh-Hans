---
product: campaign
title: 审核记录
description: 了解如何使用Campaign审核记录监控实例
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: 0fe12b469810c946ab0b9472e9a877aaaa41581d
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%

---

# 审核记录{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="审核记录"
>abstract="新的审核记录功能按时间顺序详细记录了对 Adobe Campaign 实例进行的所有操作和事件。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hans" text="请参阅发行说明"


在Adobe Campaign Web用户界面中，**[!UICONTROL 审核跟踪]**&#x200B;功能可让用户完全了解对实例中的重要实体所做的所有修改，通常是对实例的顺利操作产生显着影响的修改。

>[!IMPORTANT]
>
>* Adobe Campaign Web用户界面不审核在用户权限、模板、个性化或营销活动中所做的更改。
>* 审核记录只能由实例的管理员管理。

**[!UICONTROL 审核跟踪]**&#x200B;功能会持续实时记录在Adobe Campaign实例中发生的操作和事件的详细日志。 它提供了一种方便的方法来访问按时间顺序排列的数据记录，从而解决各种查询，例如：工作流的状态、要修改它们的最新个人，或用户在实例中执行的活动。

+++ 了解有关审核记录可用实体的更多信息

* **Source架构审核跟踪**&#x200B;允许您在Campaign V8客户端控制台中监视活动以及最近对架构所做的修改。

  有关架构的详细信息，请参阅[Campaign v8文档](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas)。

* **工作流审核跟踪**&#x200B;允许您跟踪活动以及对工作流所做的最新更改，包括其当前状态，例如：

   * 开始
   * 暂停
   * 停止
   * 重新启动
   * 清除等于操作清除历史记录
   * 模拟在模拟模式下等于操作“开始”的项
   * 唤醒等于操作立即执行待处理任务
   * 无条件停止

  有关工作流的详细信息，请参阅此[页面](../workflows/gs-workflows.md)。

* **选项审核记录**&#x200B;允许您监视活动以及最近对Campaign V8中的选项所做的修改。

  有关选项的更多信息，请参阅此[页面](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options)。

* **投放审核跟踪**&#x200B;允许您检查投放的活动和上次所做的修改。

  有关投放的详细信息，请参阅此[页面](../msg/gs-deliveries.md)。

* **外部帐户**&#x200B;允许您检查Campaign V8中对外部帐户所做的修改，这些修改由技术工作流或营销活动工作流等技术流程使用。

  有关外部帐户的详细信息，请参阅此[页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts)。

* 通过&#x200B;**投放映射**，您可以监视活动以及最近对Campaign V8中的投放映射所做的修改。

  有关投放映射的详细信息，请参阅此[页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings)。

* **Web应用程序**&#x200B;允许您检查Campaign V8中对Web窗体所做的修改，该窗体用于创建具有输入和选择字段的页面，并且可能包含来自数据库的数据。

  有关Web应用程序的详细信息，请参阅此[页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps)。

* **选件**&#x200B;允许您检查活动和对选件所做的最后修改。

  有关选件的详细信息，请参阅此[页面](../msg/offers.md)。

* **操作员**&#x200B;允许您监视活动以及最近在Campaign V8中对操作员进行的修改。

  有关运算符的详细信息，请参阅此[页面](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators)。

+++

## 访问审核记录 {#accessing-audit-trail}

要访问实例的&#x200B;**[!UICONTROL 审核跟踪]**，请执行以下操作：

1. 在&#x200B;**[!UICONTROL 管理]**&#x200B;菜单下，选择&#x200B;**[!UICONTROL 审核跟踪]** 。

   ![](assets/audit-trail-1.png)

1. 将打开&#x200B;**[!UICONTROL 审核跟踪]**&#x200B;窗口，其中包含实体列表。 Adobe Campaign Web用户界面审核工作流、选项、投放和架构的创建、编辑和删除操作。

   选择其中一个实体以了解有关上次修改的更多信息。

1. **[!UICONTROL 审核实体]**&#x200B;窗口为您提供有关所选实体的更多详细信息，例如：

   * **[!UICONTROL 类型]** ：工作流、选项、投放或架构。
   * **[!UICONTROL 实体]** ：活动的内部名称。
   * **[!UICONTROL 修改者]** ：上次修改此实体的人员的用户名。
   * **[!UICONTROL 操作]** ：对此实体执行的最后一个操作，已创建、已修改或已删除。
   * **[!UICONTROL 修改日期]** ：对此实体执行的上次操作的日期。

   代码块为您提供了有关实体中确切更改的更多信息。

   ![](assets/audit-trail-2.png)
