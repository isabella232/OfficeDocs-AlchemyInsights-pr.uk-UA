---
title: Використання сайту Wix з Office 365 придбані або керовані домени
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
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708505"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Використання сайту Wix з Office 365 придбані або керовані домени

- [Оновлення записів DNS для збереження веб-сайту за допомогою поточного постачальника послуг хостингу](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Стаття Wix "підключення домену до Wix за допомогою методу наведення" рекомендує використовувати вказівку (додавання записів DNS за вищевказаним посиланням), а не змінювати імена серверів під час використання Office 365
- Якщо ви все ще вирішите змінити ім'я сервера в Wix вам потрібно буде [створити ЗАПИСИ DNS в Wix для Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Якщо домен придбано в корпорації Майкрософт, сервери імен не можна змінити. Якщо вам потрібно змінити імена серверів, які придбали домен Microsoft, потрібно буде [перенести до іншого хостинг-провайдера після 60 днів](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)