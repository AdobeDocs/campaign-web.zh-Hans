---
audience: end-user
title: 建立和管理审批流程
description: 了解如何在Campaign Web中管理营销活动的批准
feature: Approvals, Campaigns
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 4%

---

# 管理审批流程 {#campaign-approvals}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn6"
>title="活动审批管理"
>abstract="您现在可以在发送投放之前协调利益相关者验证。 需要营销经理、数据分析师或其他团队的审批以进行质量控制。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hans" text="请参阅发行说明"

>[!IMPORTANT]
>
>审批仅适用于在营销策划内创建的投放。 这不适用于独立投放或在活动上下文之外的工作流中创建的投放。

批准流程有助于协调多个利益相关者，并确保在发送投放之前进行质量控制。 当您的组织需要经过不同团队的验证时，例如营销经理审查内容或数据分析师验证目标受众，请使用批准。

启用审批后，您必须提交内容或目标以供审批。 指定的审阅人会收到请求验证的电子邮件通知，并可直接从Web UI界面批准或拒绝。 在获得所有必需的批准之前，无法发送投放。 您可以启用：

* **内容审批**：验证邮件内容、设计和个性化
* **目标审批**：验证受众和定位条件
* **投放确认**：发送前需要最终确认

## 配置审批设置 {#configure-approvals}

审批设置继承自活动模板，并且可以为各个活动修改。 按照以下步骤配置审批设置：

1. 从&#x200B;**[!UICONTROL 营销活动]**&#x200B;菜单打开您的营销活动或营销活动模板，或创建一个新模板。

1. 单击营销活动仪表板右上角的&#x200B;**[!UICONTROL 设置]**&#x200B;按钮。

1. 在&#x200B;**[!UICONTROL 审批]**&#x200B;部分中，配置以下选项：

   ![显示活动审批设置的屏幕截图](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL 启用内容审批]**：启用后，发送前必须批准投放内容。 单击&#x200B;**[!UICONTROL 查看者]**&#x200B;字段中的文件夹图标以选择操作员或操作员组。

   * **[!UICONTROL 启用目标审批]**：启用时，必须审批投放目标受众。 单击&#x200B;**[!UICONTROL 查看者]**&#x200B;字段中的文件夹图标以选择操作员或操作员组。

   * **[!UICONTROL 发送前确认投放]**：要求在发送前进行最终手动确认，即使所有其他审批都已完成。

>[!NOTE]
>
>* 如果未指定审核者，则活动所有者将被分配为审核者。
>* 审阅人需要具有相应的权限才能批准投放。 只有查看者列表中标识的用户才能批准。

## 提交等待审批 {#submit-approval}

创建投放后，请按照以下步骤提交内容和目标以供审批。

>[!NOTE]
>审批在活动工作流投放和活动独立投放中均可用。

1. 在投放仪表板中，单击&#x200B;**[!UICONTROL 提交内容]**&#x200B;按钮。 指定的审阅人可以批准或拒绝。 请参阅此[章节](#approve-reject)。

   ![显示“提交内容”按钮的屏幕截图](assets/approvals2.png){zoomable="yes"}

   投放仪表板的&#x200B;**[!UICONTROL 属性]**&#x200B;部分中的审批状态更改为待处理。 请参阅此[章节](#rack-approvals)。

1. 内容获得批准后，单击&#x200B;**[!UICONTROL 准备]**&#x200B;按钮以准备投放目标。 系统准备受众和定位标准。

1. 单击&#x200B;**[!UICONTROL 提交目标]**&#x200B;按钮。 然后，指定的审阅人可批准或拒绝。 请参阅此[章节](#approve-reject)。

   ![显示提交目标按钮的屏幕截图](assets/approvals5.png){zoomable="yes"}

   审批状态更改为待定。 请参阅此[章节](#rack-approvals)。

1. 目标获得批准后，准备工作将继续，并且投放。

>[!NOTE]
>如果批准被拒绝，则投放责任人必须根据审阅人的反馈对内容或目标进行所有必要的更改，然后重新提交以供批准。

## 批准或拒绝 {#approve-reject}

指定的审阅人可以批准或拒绝内容并定位提交。 请参阅此[章节](#submit-approval)。

>[!NOTE]
>对于要发送的电子邮件通知，必须在实例中配置查看者的地址。

1. 当您收到通知电子邮件时，请直接从Web UI界面打开需要审批的投放。

1. 查看内容或目标信息。

1. 单击&#x200B;**[!UICONTROL 批准内容]**&#x200B;或&#x200B;**[!UICONTROL 批准目标]**&#x200B;按钮。

   ![在投放仪表板中显示“批准内容”按钮的屏幕截图](assets/approvals3.png){zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 批准]**&#x200B;或&#x200B;**[!UICONTROL 拒绝]**。

1. （可选）添加&#x200B;**[!UICONTROL 评论]**&#x200B;以解释您的决定。

   ![屏幕截图显示审批对话框，其中包含审批、拒绝按钮和评论字段](assets/approvals4.png){zoomable="yes"}

1. 确认您的决定。 审批状态会在投放仪表板中立即更新。 请参阅此[章节](#rack-approvals)。

## 跟踪审批状态 {#track-approvals}

审批状态显示在投放仪表板的&#x200B;**[!UICONTROL 属性]**&#x200B;部分中。 状态显示正在等待哪些审批及其当前状态：

![显示审批状态的屏幕快照](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL 正在编辑]**：尚未提交内容或目标以供审批
* **[!UICONTROL 未决批准]**：内容或目标正在等待审阅
* **[!UICONTROL 已批准]**：内容或目标已由审阅人批准
* **[!UICONTROL 已拒绝]**：审阅者已拒绝内容或目标

审批部分实时显示所有启用的审批和更新，因为审核者验证或拒绝每个步骤。

## 相关主题 {#related}

* [创建活动](create-campaigns.md)
* [管理活动](manage-campaigns.md)
