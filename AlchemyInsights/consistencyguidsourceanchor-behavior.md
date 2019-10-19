---
title: Послідовність надсилання GUID/Джереопору
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36517016"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="62e4c-102">Послідовність надсилання GUID/Джереопору</span><span class="sxs-lookup"><span data-stu-id="62e4c-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="62e4c-103">Azure AD-підключення (версія 1.1.524.0 і після) тепер полегшує використання msDS-послідовність, як атрибут Джерелиприв'язки.</span><span class="sxs-lookup"><span data-stu-id="62e4c-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="62e4c-104">Під час використання цієї функції, Azure AD Connect автоматично налаштовує правила синхронізації на:</span><span class="sxs-lookup"><span data-stu-id="62e4c-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="62e4c-105">Використання msDS-послідовність, як атрибут, що Джерелиприв'язка об'єктів користувача.</span><span class="sxs-lookup"><span data-stu-id="62e4c-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="62e4c-106">ObjectGUID використовується для інших типів об'єктів.</span><span class="sxs-lookup"><span data-stu-id="62e4c-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="62e4c-107">Для будь-якого локального об'єкта користувача оголошення, якого атрибут msDS-послідовність Encyguid не вказано, Azure AD-підключення записує його objectGUID значення до атрибута msDS-послідовність Encyguid в локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="62e4c-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="62e4c-108">Після того, як атрибут msDS-послідовність Encyguid вказано, Azure AD-підключення експорту об'єкта Azure AD.</span><span class="sxs-lookup"><span data-stu-id="62e4c-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="62e4c-109">**Примітка:** Після того, як локальний об'єкт оголошення імпортується в Azure AD-підключення (тобто імпортується у просторі з'єднувача оголошення та проектується метавсесвіту), більше не можна змінити його значення.</span><span class="sxs-lookup"><span data-stu-id="62e4c-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="62e4c-110">Щоб указати Джерелюприв'язку значення для певного локального об'єкта оголошення, настройте його атрибут msDS-послідовність Encyguid перед імпортованим у Azure AD-підключення.</span><span class="sxs-lookup"><span data-stu-id="62e4c-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="62e4c-111">Щоб отримати додаткові відомості про Джерелюякір і послідовність, GUID, зверніться до таких: [AZURE AD-підключення: концепції проектування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="62e4c-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

