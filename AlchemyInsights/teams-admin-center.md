---
title: Центр адміністрування Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354109"
---
# <a name="teams-admin-center"></a>Центр адміністрування Teams

Дізнайтеся, як керувати Teams за допомогою [Центру адміністрування Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Якщо вам не вдається отримати доступ до Центру адміністрування Teams, виконайте наведені нижче вказівки.

- Пересвідчіться, що ви надали дозволи відповідним [IP- та URL-адресам Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всіх пристроях захисту мережевого периметра (брандмауер тощо) або в правилах брандмауера на локальному комп’ютері.
- Переконайтеся, що логін, який використовується, щоб отримати доступ до порталу адміністрування Teams, відповідає вашому імені користувача, вказаним на [порталі адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Якщо користувачі не відображаються в центрі адміністрування Teams, перевірте вказане нижче.

- Ви створювали користувачів або призначали ліцензії протягом останніх 24 годин? Перш ніж відкрити квиток підтримки, переконайтеся, що минуло принаймні 24 години.
- Пересвідчіться, що ви призначили відповідні ліцензії.
- Якщо у вас є локальний Active Directory, переконайтеся, що [значення msRTCSIP-первинний адресу або SIP-адресу в proxyAddresses поле в локальній Active Directory є унікальним і формат відповідає](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**ім'я** користувача з [центру адміністрування Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Якщо ви маєте намір зберегти Skype для розгортання бізнес-сервера і користувачі, виконайте реплікацію локальної та онлайн: виконайте **"створити змішаний з команди та Skype для бізнесу онлайн"** у Skype, для бізнес-сервер панелі керування та переміщення користувачів в Інтернеті.
