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
# <a name="consistencyguid--sourceanchor-behavior"></a>Спосіб відповідного ідентифікатора _ програми

Azure AD Connect (версія 1.1.524.0 і After) тепер полегшує використання msDS-послідовним GUID як атрибута Sourcetoror. Під час використання цієї функції функція Azure AD Connect автоматично настроює правила синхронізації:
  
- Використання msDS-Contencyguid як атрибута вихідного коду для об'єктів користувача. Для інших типів об'єктів використовується Obbguid.
    
- Для будь-якого локального об'єкта, який відповідає атрибуту msDS, який не заповнюється, функція Azure AD Connect записує його значення Obcoguid у локальній службі Active Directory. Після того, як атрибут msDS-Conctenyguid заповнено, Лазурне з'єднання потім експортує об'єкт в Лазурне AD.
    
 **Примітка.** Після того як локальний об'єкт AD імпортується в Azure AD Connect (що імпортується в простір з'єднувача AD і прогнозується в Метавселенну), більше не можна змінити його значення. Щоб указати вихідний параметр для вказаного локального об'єкта AD, настройте його атрибут msDS-confidenguid, перш ніж його буде імпортовано в Azure AD Connect. 
  
Щоб отримати докладніші відомості про ім'я та відповідний GUID, виконайте наведені нижче дії. [Azure AD Connect: концепції оформлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

