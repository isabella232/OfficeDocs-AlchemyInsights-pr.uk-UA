---
title: Послідовність надсилання GUID/Джереопору
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705754"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Послідовність надсилання GUID/Джереопору

Azure AD-підключення (версія 1.1.524.0 і після) тепер полегшує використання msDS-послідовність, як атрибут Джерелиприв'язки. Під час використання цієї функції, Azure AD Connect автоматично налаштовує правила синхронізації на:
  
- Використання msDS-послідовність, як атрибут, що Джерелиприв'язка об'єктів користувача. ObjectGUID використовується для інших типів об'єктів.
    
- Для будь-якого локального об'єкта користувача оголошення, якого атрибут msDS-послідовність Encyguid не вказано, Azure AD-підключення записує його objectGUID значення до атрибута msDS-послідовність Encyguid в локальній службі Active Directory. Після того, як атрибут msDS-послідовність Encyguid вказано, Azure AD-підключення експорту об'єкта Azure AD.
    
 **Примітка:** Після того, як локальний об'єкт оголошення імпортується в Azure AD-підключення (тобто імпортується у просторі з'єднувача оголошення та проектується метавсесвіту), більше не можна змінити його значення. Щоб указати Джерелюприв'язку значення для певного локального об'єкта оголошення, настройте його атрибут msDS-послідовність Encyguid перед імпортованим у Azure AD-підключення. 
  
Щоб отримати додаткові відомості про Джерелюякір і послідовність, GUID, зверніться до таких: [AZURE AD-підключення: концепції проектування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

