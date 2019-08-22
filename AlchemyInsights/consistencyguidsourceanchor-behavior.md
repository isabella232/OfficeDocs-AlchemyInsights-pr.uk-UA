---
title: ConsistencyGuid / sourceAnchor поведінка
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517016"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="a097b-102">ConsistencyGuid / sourceAnchor поведінка</span><span class="sxs-lookup"><span data-stu-id="a097b-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="a097b-103">Блакитні оголошення підключення (версії 1.1.524.0 і після) тепер полегшує використання msDS-ConsistencyGuid як атрибут sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="a097b-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="a097b-104">При використанні цієї функції, Azure оголошення підключитися автоматично настроює правил синхронізації, щоб:</span><span class="sxs-lookup"><span data-stu-id="a097b-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="a097b-105">Для користувача об'єкти за допомогою msDS-ConsistencyGuid як атрибут sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="a097b-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="a097b-106">ObjectGUID використовується для інших типів об'єктів.</span><span class="sxs-lookup"><span data-stu-id="a097b-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="a097b-107">Для будь-якого з огляду на локальному Оголошень користувача назад об'єкт, чиї msDS-ConsistencyGuid атрибут не заселені, Azure оголошення підключення пише його objectGUID значення для msDS-ConsistencyGuid атрибут у локальній службі Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a097b-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="a097b-108">Після того, як населені атрибут msDS-ConsistencyGuid, Azure оголошення підключення експортує об'єкт в блакитні оголошення.</span><span class="sxs-lookup"><span data-stu-id="a097b-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="a097b-109">**Примітка:** Одного разу локальні оголошення об'єкт буде імпортовано до Azure оголошення підключення (тобто, імпортовані в Рекламний простір з'єднувача та прогнозовані в метавселенной), не можна змінити його sourceAnchor значення більше.</span><span class="sxs-lookup"><span data-stu-id="a097b-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="a097b-110">Вкажіть значення sourceAnchor для з огляду на локальному оголошення об'єкт, налаштувати його атрибут msDS-ConsistencyGuid, перш ніж вона буде імпортовано до Azure оголошення підключитися.</span><span class="sxs-lookup"><span data-stu-id="a097b-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="a097b-111">Більш докладну інформацію про SourceAnchor та ConsistencyGuid, Докладніше: [Azure оголошення підключитися: дизайн концепції](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="a097b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

