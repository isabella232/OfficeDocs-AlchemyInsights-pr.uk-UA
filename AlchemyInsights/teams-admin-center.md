---
title: Центр адміністрування Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826400"
---
# <a name="teams-admin-center"></a>Центр адміністрування Teams

Дізнайтеся, як керувати Teams за допомогою [Центру адміністрування Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Якщо вам не вдається отримати доступ до Центру адміністрування Teams, виконайте наведені нижче вказівки.

- Пересвідчіться, що ви надали дозволи відповідним [IP- та URL-адресам Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всіх пристроях захисту мережевого периметра (брандмауер тощо) або в правилах брандмауера на локальному комп’ютері.
- Переконайтеся, що логін, який використовується, щоб отримати доступ до порталу адміністрування Teams, відповідає вашому імені користувача, вказаним на [порталі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Якщо користувачі не відображаються в центрі адміністрування Teams, перевірте вказане нижче.

- Ви створювали користувачів або призначали ліцензії протягом останніх 24 годин? Перш ніж відкрити квиток підтримки, переконайтеся, що минуло принаймні 24 години.
- Пересвідчіться, що ви призначили відповідні ліцензії.
- Якщо у вас є локальна служба Active Directory, переконайтеся, що значення [msRTCSIP-PrimaryUserAddress або SIP-адреси в полі ProxyAddresses](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) у локальній службі Active Directory унікальне, а формат відповідає sip: ім'я користувача з Центру адміністрування Microsoft [365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Якщо ви планували зберегти розгортання "Skype для бізнесу – сервер" і розгорнути їх у локальному середовищі та онлайн, виконайте вказівки "Налаштування гібридного розгортання з Teams і "Skype для бізнесу – онлайн" на Панелі керування "Skype для бізнесу – **сервер"** і перемістіть користувачів через Інтернет.
