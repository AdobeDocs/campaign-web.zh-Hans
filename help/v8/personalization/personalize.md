---
title: 在 Campaign 中个性化您的内容
description: 了解如何在 Adobe Campaign Web UI 中个性化您的内容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 551e6b9efa8b29475bd2f0a71ce016681bf70289
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 5%

---


# 个性化您的内容 {#add-personalization}

可以使用表达式编辑器将个性化添加到任何投放中，该编辑器可通过在每个字段中访问 **[!UICONTROL 打开个性化对话框]** 图标，例如主题行字段，或电子邮件链接和文本/按钮内容组件。 [了解在何处添加动态内容](gs-personalization.md/#access)

## 个性化语法 {#syntax}

个性化标记始终使用以下语法： `<%=table.field%>`. 例如，要插入存储在收件人表中的收件人名称，个性化标记使用&lt;%= recipient.lastName %>语法。

准备投放后，Adobe Campaign会自动解释这些标记，并将其替换为给定收件人的字段值。 然后，在模拟内容时，可以查看物理替换。

## 添加个性化标记 {#add}

要将个性化标记添加到投放中，请使用以下内容打开表达式编辑器 **[!UICONTROL 打开个性化对话框]** 可从文本类型编辑字段（如主题行或短信正文）访问的图标。 [了解在何处添加动态内容](gs-personalization.md/#access)

![](assets/perso-access.png)

此时将显示表达式编辑器。 个性化字段被组织到位于屏幕左侧的多个菜单中。 通过这些菜单，可以访问Adobe Campaign数据库中可用的所有字段。

![](assets/perso-insert-field.png)

| 菜单 | 说明 |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | 此 **[!UICONTROL 订阅者应用程序]** 菜单列出与应用程序的订阅者相关的所有字段，例如使用的终端或操作系统。 *此菜单仅适用于推送通知* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | 此 **[!UICONTROL 收件人]** 菜单列出了收件人表中定义的所有字段，例如收件人的姓名、年龄或地址。 |
| ![](assets/do-not-localize/perso-message-menu.png) | 此 **[!UICONTROL 消息]** 菜单列出与投放日志相关的所有字段，即跨所有渠道发送到收件人或设备的所有消息，如与给定收件人发生的最后一个事件的日期 |
| ![](assets/do-not-localize/perso-delivery-menu.png) | 此 **[!UICONTROL 投放]** 菜单列出与执行投放所需的参数相关的所有字段，例如投放渠道、标签等。 |

>[!NOTE]
>
>默认情况下，每个菜单都会显示选定表中的所有字段（收件人、/消息/投放）。 如果要包含链接到选定表的表中的字段，请启用 **[!UICONTROL 显示高级属性]** 选项的位置。

要添加个性化字段，请将光标放在内容中的所需位置，然后单击+按钮以插入该字段。

内容准备就绪后，您可以保存内容并通过模拟内容来测试个性化内容的渲染。 在以下示例中，我们使用目标用户档案的名字个性化短信消息。

*在消息内容中添加个性化标记*

![](assets/perso-preview1.png)

*模拟给定测试用户档案的个性化渲染*

![](assets/perso-preview2.png)
