---
title: Використання веб-сайту Wix з придбаними або керованими доменами Office 365
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
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825968"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Використання веб-сайту Wix з придбаними або керованими доменами Office 365

- [Оновлення записів DNS для збереження веб-сайту в поточного постачальника послуг розміщення](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Стаття Wix "Підключення домену до Wix Using the Pointing Method" рекомендує використовувати вказівку (додавання записів DNS за наведеним вище посиланням), а не змінення DNS-серверів під час використання служби Office 365.
- Якщо все одно потрібно змінити DNS-сервери на Wix, знадобиться створити записи  [DNS на сайті Wix для Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Якщо домен придбано в корпорації Майкрософт, змінити DNS-сервери не можна. Якщо потрібно змінити dns-сервери імен, придбаний домен Microsoft потрібно буде перенести до іншого постачальника послуг розміщення  [через 60 днів](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)