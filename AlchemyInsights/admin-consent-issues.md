---
title: Проблеми згоди адміністратора
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952594"
---
# <a name="admin-consent-issues"></a>Проблеми згоди адміністратора

1. [Увімкніть робочий](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) цикл згоди адміністратора, щоб дозволити користувачам запитувати схвалення адміністратора безпосередньо з екрана згоди.

1. Якщо в процесі згоди користувачі або вашої програми побачать неочікувані помилки, див. цю статтю для виправлення неполадок: Неочікувана помилка під час виконання [згоди програми.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Дізнайтеся більше про згоду адміністратора [платформа ідентичностей Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)принцип роботи запиту на згоду, а також про те, як оцінити запит на згоду адміністратора [для клієнта.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)

1. Програми, які інтегруються платформа ідентичностей Microsoft до моделі авторизації, яка надає користувачам і адміністраторам контроль над доступом до даних. Впровадження моделі авторизації оновлено в кінцевій точці платформа ідентичностей Microsoft, і вона змінює спосіб взаємодії програми з платформа ідентичностей Microsoft. Огляд цієї моделі авторизації, зокрема областей, [дозволів](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) і згоди, див. в розділі Дозволи та згода в кінцевій точці платформа ідентичностей Microsoft.