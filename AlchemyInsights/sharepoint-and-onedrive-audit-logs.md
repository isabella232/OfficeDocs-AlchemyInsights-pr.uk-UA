---
title: Класичні звіти журналу аудиту SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662229"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Журнали аудиту SharePoint і OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Журнали аудиту SharePoint Classic

Відстеження успадкованого аудиту в службі єдиного журналу аудиту (UAL). У всіх звітах про успадковані аудиторські звіти тепер буде здійснюватися через Al, а успадковані сигналах, які було перенесено до UAL.

Основні зміни:

* Функція обрізки недоступна як можливість.
* Вибір певних подій для аудиту недоступний. Зверніться до [цього документа](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) , щоб переглянути повний список перевірених подій, доступних за замовчуванням.
* Параметр " **розташування** " в розділі " **Настроювані звіти** " недоступний.
* Параметр " **відкриття або завантаження** подій для документів" недоступний.

[Настроювання параметрів аудиту для колекції сайтів](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Служби SharePoint і OneDrive для сучасних уніфікованих журналів аудиту відповідно

* [Увімкнення та вимкнення журналювання єдиного аудиту](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

У службі SharePoint або OneDrive не потрібне додаткове настроювання.

Використання функції журналювання аудиту для перевірки діяльності файлів (-ів), папок, користувачів, дозволів:

* [Дії з файлами та сторінками](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Дії з папками](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Надання спільного доступу до дій і запитів на доступ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Дії з синхронізації](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Дії з адміністрування сайту](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Додаткові відомості про те, як отримати ці події, наведено [в статті пошук у журналі аудиту](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
