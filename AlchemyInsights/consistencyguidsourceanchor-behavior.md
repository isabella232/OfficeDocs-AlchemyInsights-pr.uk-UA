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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Connect (версія 1.1.524.0 і після) тепер спрощує використання msDS-ConsistencyGuid як атрибута sourceAnchor. Коли ця функція використовується, Azure AD Connect автоматично настроєні правила синхронізації, щоб:
  
- Використовуйте msDS-ConsistencyGuid як атрибут sourceAnchor для об'єктів користувачів. ObjectGUID використовується для інших типів об'єктів.
    
- Для будь-якого локального об'єкта користувача AD, атрибут msDS-ConsistencyGuid не заповнено, Azure AD Connect записує значення objectGUID назад до атрибута msDS-ConsistencyGuid в локальній службі Active Directory. Коли атрибут msDS-ConsistencyGuid заповнено, Azure AD Connect експортує об'єкт до Azure AD.
    
 **Примітка.** Після імпорту локального об'єкта AD до Azure AD Connect (тобто імпортованого в область з'єднатора AD і проектування в метавимірник), більше не можна змінити його значення sourceAnchor. Щоб указати значення sourceAnchor для даного локального об'єкта AD, настройте його атрибут msDS-ConsistencyGuid, перш ніж імпортувати його до Azure AD Connect. 
  
Докладні відомості про SourceAnchor і ConsistencyGuid див. в таких [статтях: Azure AD Connect: концепції розробки](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

