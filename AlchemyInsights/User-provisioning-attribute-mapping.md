---
title: Зіставлення атрибутів користувача
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949900"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="715fc-102">Зіставлення атрибутів користувача</span><span class="sxs-lookup"><span data-stu-id="715fc-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="715fc-103">Щоб виправити помилки, які мають відомі проблеми з відображенням атрибутів, ознайомтеся з [зіставленнями атрибутів](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="715fc-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="715fc-104">Служба Microsoft Azure Active Directory (AD) надає підтримку для підготовки користувачів стороннім програмам SaaS, як-от "Salesforce", "G Suite" тощо.</span><span class="sxs-lookup"><span data-stu-id="715fc-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="715fc-105">Якщо ви активувати підготовку користувача для програми SaaS для третьої сторони, на порталі Azure можна керувати значеннями атрибутів за допомогою зіставлень атрибутів.</span><span class="sxs-lookup"><span data-stu-id="715fc-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="715fc-106">Щоб дізнатися, як настроїти зіставлення атрибутів за замовчуванням, перегляньте статтю [Настроювання атрибута підготовки користувачів – зіставлення для програм SaaS у службі Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="715fc-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="715fc-107">Докладні відомості про підготовку користувачів за програмою SaaS можна дізнатися про [те, що таке автоматизована програма підготовки користувачів SaaS в Лазурне AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="715fc-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="715fc-108">Під час настроювання зіставлення атрибутів для підготовки користувача може виявитися, що атрибут, який потрібно зіставити, не відображається у списку вихідних атрибутів.</span><span class="sxs-lookup"><span data-stu-id="715fc-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="715fc-109">[Атрибут Sync від локального служби Active Directory до Azure AD для підготовки до програми у](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) статті показано, як додати відсутній атрибут, синхронізуючи її з локального рекламного повідомлення в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="715fc-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
