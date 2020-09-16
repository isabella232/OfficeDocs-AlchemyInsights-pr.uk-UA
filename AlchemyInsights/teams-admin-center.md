---
title: Центр адміністрування Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670385"
---
# <a name="teams-admin-center"></a>Центр адміністрування Teams

Дізнайтеся, як керувати Teams за допомогою [Центру адміністрування Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Якщо вам не вдається отримати доступ до Центру адміністрування Teams, виконайте наведені нижче вказівки.

- Пересвідчіться, що ви надали дозволи відповідним [IP- та URL-адресам Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всіх пристроях захисту мережевого периметра (брандмауер тощо) або в правилах брандмауера на локальному комп’ютері.
- Переконайтеся, що логін, який використовується, щоб отримати доступ до порталу адміністрування Teams, відповідає вашому імені користувача, вказаним на [порталі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Якщо користувачі не відображаються в центрі адміністрування Teams, перевірте вказане нижче.

- Ви створювали користувачів або призначали ліцензії протягом останніх 24 годин? Перш ніж відкрити квиток підтримки, переконайтеся, що минуло принаймні 24 години.
- Пересвідчіться, що ви призначили відповідні ліцензії.
- Якщо у вас є локальна Служба Active Directory, переконайтеся, що [значення параметра msRTCSIP-PrimaryUserAddress або SIP-адреса в полі "proxyAddress" в локальному Active Directory є унікальним, а формат відповідає](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**ім'я** користувача в [центрі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Якщо ви збираєтесь зберегти розгортання на сервері Skype для бізнесу, а також користувачі, які створили локальну та онлайнове повідомлення, виконайте **команду "Настроювання гібридного використання команд і" Skype для бізнесу – онлайн "** на панелі керування служби" Skype для бізнесу "та перенесіть користувачів в онлайні.
