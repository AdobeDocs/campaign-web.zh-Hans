---
audience: end-user
title: Campaign Web 中的权限管理
description: 详细了解 Campaign Web v8 中的权限
badge: label="Beta"
source-git-commit: dce8351463f898ccf02816a521d9db3f80ce3dbc
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 50%

---


# 访问和权限 {#access-and-permissions}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="需要权限"
>abstract="您的管理员必须先授予您权限，然后您才能创建该对象。"


>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="此受众为只读"
>abstract="您无权编辑此受众。如果需要，请联系您的管理员以向您授予访问权限。"


>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="此服务为只读"
>abstract="您无权编辑此服务。如果需要，请联系您的管理员以向您授予访问权限。"


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="此活动为只读"
>abstract="您无权编辑此活动。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="此交付为只读"
>abstract="您无权编辑此交付。如果需要，请联系您的管理员以向您授予访问权限。"


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="此工作流为只读"
>abstract="您无权编辑此工作流。如果需要，请联系您的管理员以向您授予访问权限。"

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="此工作流为只读"
>abstract="由于画布不受支持或不兼容，您无法编辑此工作流程。"

访问控制可限制从主列表（如投放、收件人或工作流）对于对象和数据的访问。这些限制在资源管理器导航树中也适用。此外，需要相关权限才能从用户界面中创建、删除、复制和编辑对象。

在客户端控制台中管理访问控制。Campaign Web 中的所有权限都与 Campaign 客户端控制台权限同步。仅 Campaign 管理员能够定义和修改用户权限。可在 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html){target="_blank"}中详细了解用户权限。

在浏览Campaign Web用户界面时，您可以访问数据、对象和功能，具体取决于您的权限。 例如，如果您无权访问某个文件夹，则您看不到它。您的权限还影响对象和数据管理。没有特定文件夹的写入权限，即无法在该文件夹中创建某个投放，即使您可在用户界面中看到它也是如此。

## 查看权限 {#view-permissions}

从 **资源管理器**，您可以浏览每个文件夹的权限。 这些权限在客户端控制台中设置，用于组织和控制对Campaign数据的访问。

要查看文件夹的权限，请执行以下步骤：

1. 从 **资源管理器** 在左侧导航菜单中，选择一个文件夹。
1. 单击右上角的三个圆点，然后选择 **文件夹权限**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. 在屏幕中查看详细信息，如下所示：

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   组或操作员可以对存储在选定文件夹中的数据具有读取、写入和/或删除权限。

   如果 **传播** 选项，为文件夹定义的所有权限将应用于其所有子文件夹。 可以为每个子文件夹重载这些权限。

   如果 **系统文件夹** 选项时，允许所有操作员访问，无论其权限如何。

在中了解有关文件夹权限的更多信息 [Campaign v8（客户端控制台）文档](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## 使用文件夹 {#folders}

您可以创建、重命名、重新排序和移动文件夹来组织组件和数据。 您还可以从同一菜单删除文件夹。

>[!CAUTION]
>
>删除文件夹时，存储在文件夹中的所有数据也会被删除。

要创建文件夹，请执行以下步骤：

1. 从 **资源管理器** 在左侧导航菜单中，选择一个文件夹。
1. 单击右上角的三个圆点，然后选择 **创建新子文件夹**.
1. 输入文件夹名称并保存。

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   该文件夹将作为当前文件夹的子文件夹添加。 浏览到该新文件夹以直接在其中创建组件。 您还可以从任意文件夹创建一个组件，并将其保存在新文件夹中。 **其他选项** 部分，如下面的投放所示：

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}

