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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044362"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Підключення (версія 1.1.524.0 і новіші) тепер спрощує використання msDS-ConsistencyGuid як атрибута sourceAnchor. Коли ця функція використовується, Підключення Azure AD автоматично настроєні правила синхронізації, щоб:
  
- Використовуйте msDS-ConsistencyGuid як атрибут sourceAnchor для об'єктів користувачів. ObjectGUID використовується для інших типів об'єктів.
    
- Для будь-якого локального об'єкта користувача AD, атрибут msDS-ConsistencyGuid не заповнено, Azure AD Підключення записує значення objectGUID назад до атрибута msDS-ConsistencyGuid в локальній службі Active Directory. Коли атрибут msDS-ConsistencyGuid заповниться, Azure AD Підключення потім експортує об'єкт до Azure AD.
    
 **Примітка.** Якщо імпортувати локальний об'єкт AD до Azure AD Підключення (тобто імпортувати його до простору з'єднатора AD та проектувати його в metaverse), більше не можна змінити його значення sourceAnchor. Щоб указати значення sourceAnchor для даного локального об'єкта AD, настройте його атрибут msDS-ConsistencyGuid перед імпортом в Azure AD Підключення. 
  
Докладні відомості про SourceAnchor і ConsistencyGuid див. в таких статтях: [Azure AD Підключення: концепції розробки](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

