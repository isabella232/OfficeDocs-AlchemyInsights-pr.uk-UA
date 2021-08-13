---
title: Використання веб-сайту Wix із Office 365 придбаними доменами або керованими доменами
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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980198"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Використання веб-сайту Wix із Office 365 придбаними доменами або керованими доменами

- [Оновлення записів DNS для збереження веб-сайту в поточного постачальника послуг розміщення](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Стаття Wix "Підключення домену до Wix Using the Pointing Method" рекомендує використовувати вказівку (додавання записів DNS за наведеним вище посиланням), а не змінення DNS-серверів під час використання Office 365
- Якщо все одно потрібно змінити DNS-сервери на Wix, знадобиться створити записи  [DNS на сайті Wix для Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Якщо домен придбано в корпорації Майкрософт, змінити DNS-сервери не можна. Якщо потрібно змінити dns-сервери імен, придбаний домен Microsoft потрібно буде перенести до іншого постачальника послуг розміщення  [через 60 днів](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)