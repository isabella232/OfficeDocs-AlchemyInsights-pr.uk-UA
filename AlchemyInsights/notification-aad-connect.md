---
title: Сповіщення про підключення до AAD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037232"
---
# <a name="notification-aad-connect"></a>Сповіщення про підключення до AAD

- Переконайтеся, що ви маєте право виконати операцію. Глобальні адміністратори мають доступ за замовчуванням. Крім того, можна використовувати [елемент керування доступом на основі ролей](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , щоб отримати дозвіл на реєстрацію представника.
- Переконайтеся, що потрібні кінцеві точки ввімкнуто, а не заблоковано через брандмауер. Докладні відомості наведено в статті [вимоги](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Реєстрація може не відповідно до вихідних повідомлень, які піддаються перевірці SSL через мережевий рівень.
- Переконайтеся, що ви перевірили параметри сповіщень для служби "Azure AD Connect Health" і перегляньте свій параметр. Щоб зрозуміти, як настроїти параметри сповіщень для сповіщень про справність служби Azure AD Connect, перегляньте цей [посібник](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Щоб дізнатися більше про звіт про синхронізацію служби AAD Connect, а також про те, як завантажити його, перегляньте статтю [звіт про синхронізацію на рівні об'єкта](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Щоб виправити неполадки з оповіщення про справність AAD Connect, виконайте вказівки [з виправлення неполадок для сповіщень про стан справності та відповіді](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) на поширені запитання в розділі [Загальні запитання про інсталяцію СПРАВНОСТІ служби aad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
