---
title: Використання веб-сайту Wix із придбаними або керованими доменами Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300748"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Використання веб-сайту Wix із придбаними або керованими доменами Office 365

- [Оновлення записів DNS для збереження веб-сайту за допомогою поточного постачальника послуг розміщення](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix статті "підключення домену до Wix за допомогою методу наведення" рекомендує використовувати наведення вказівника (додавання записів DNS для наведеної вище посилання) замість того, щоб змінювати імена серверів під час використання Office 365
- Якщо ви все ще вирішите змінити DNS-сервери на веб-сайт wx, то вам знадобиться [створити записи в службі "WRX для Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide) ".
- Якщо ваш домен придбано з корпорації Майкрософт, то не можна змінити сервери імен. Якщо потрібно змінити імена серверів, придбаному домену Microsoft, потрібно [перенести на інший хостинг-провайдер після 60 днів](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host) .