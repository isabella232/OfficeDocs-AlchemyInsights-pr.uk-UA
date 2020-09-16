---
title: Спосіб відповідного ідентифікатора _ програми
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756304"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="aa786-102">Спосіб відповідного ідентифікатора _ програми</span><span class="sxs-lookup"><span data-stu-id="aa786-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="aa786-103">Azure AD Connect (версія 1.1.524.0 і After) тепер полегшує використання msDS-послідовним GUID як атрибута Sourcetoror.</span><span class="sxs-lookup"><span data-stu-id="aa786-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="aa786-104">Під час використання цієї функції функція Azure AD Connect автоматично настроює правила синхронізації:</span><span class="sxs-lookup"><span data-stu-id="aa786-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="aa786-105">Використання msDS-Contencyguid як атрибута вихідного коду для об'єктів користувача.</span><span class="sxs-lookup"><span data-stu-id="aa786-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="aa786-106">Для інших типів об'єктів використовується Obbguid.</span><span class="sxs-lookup"><span data-stu-id="aa786-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="aa786-107">Для будь-якого локального об'єкта, який відповідає атрибуту msDS, який не заповнюється, функція Azure AD Connect записує його значення Obcoguid у локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa786-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="aa786-108">Після того, як атрибут msDS-Conctenyguid заповнено, Лазурне з'єднання потім експортує об'єкт в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="aa786-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="aa786-109">**Примітка.** Після того як локальний об'єкт AD імпортується в Azure AD Connect (що імпортується в простір з'єднувача AD і прогнозується в Метавселенну), більше не можна змінити його значення.</span><span class="sxs-lookup"><span data-stu-id="aa786-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="aa786-110">Щоб указати вихідний параметр для вказаного локального об'єкта AD, настройте його атрибут msDS-confidenguid, перш ніж його буде імпортовано в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="aa786-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="aa786-111">Щоб отримати докладніші відомості про ім'я та відповідний GUID, виконайте наведені нижче дії. [Azure AD Connect: концепції оформлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="aa786-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

