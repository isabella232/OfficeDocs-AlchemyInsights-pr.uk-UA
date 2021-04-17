---
title: ConsistencyGuid / sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817013"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="06d08-102">ConsistencyGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="06d08-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="06d08-103">Azure AD Connect (версія 1.1.524.0 і після) тепер спрощує використання msDS-ConsistencyGuid як атрибута sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="06d08-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="06d08-104">Коли ця функція використовується, Azure AD Connect автоматично настроєні правила синхронізації, щоб:</span><span class="sxs-lookup"><span data-stu-id="06d08-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="06d08-105">Використовуйте msDS-ConsistencyGuid як атрибут sourceAnchor для об'єктів користувачів.</span><span class="sxs-lookup"><span data-stu-id="06d08-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="06d08-106">ObjectGUID використовується для інших типів об'єктів.</span><span class="sxs-lookup"><span data-stu-id="06d08-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="06d08-107">Для будь-якого локального об'єкта користувача AD, атрибут msDS-ConsistencyGuid не заповнено, Azure AD Connect записує значення objectGUID назад до атрибута msDS-ConsistencyGuid в локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="06d08-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="06d08-108">Коли атрибут msDS-ConsistencyGuid заповнено, Azure AD Connect експортує об'єкт до Azure AD.</span><span class="sxs-lookup"><span data-stu-id="06d08-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="06d08-109">**Примітка.** Після імпорту локального об'єкта AD до Azure AD Connect (тобто імпортованого в область з'єднатора AD і проектування в метавимірник), більше не можна змінити його значення sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="06d08-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="06d08-110">Щоб указати значення sourceAnchor для даного локального об'єкта AD, настройте його атрибут msDS-ConsistencyGuid, перш ніж імпортувати його до Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="06d08-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="06d08-111">Докладні відомості про SourceAnchor і ConsistencyGuid див. в таких [статтях: Azure AD Connect: концепції розробки](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="06d08-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

