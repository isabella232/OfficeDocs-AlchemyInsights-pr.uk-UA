---
title: Зміна параметрів обмеження трафіку у веб-службах Exchange (EWS)
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075918"
---
# <a name="changing-ews-throttling-settings"></a>Зміна параметрів обмеження трафіку у веб-службах Exchange (EWS)

Запустіть нашу автоматичну перевірку, щоб змінити політику обмеження трафіку для EWS на час перенесення. Зверніть увагу, що навіть після цієї перевірки імпорт EWS буде обмежено до 150 МБ на 5 хвилин для однієї поштової скриньки. Щоб досягти кращої пропускної здатності під час перенесення, рекомендується переносити більше користувачів одночасно.

Зверніть увагу, що зміни політики обмеження трафіку для EWS не впливають на такі типи перенесення (за допомогою інструментів Microsoft): гібридне, повне чи поетапне (з використанням віддаленого виклику процедур та HTTP), IMAP, G Suite, а також перенесення спільних папок чи імпорт файлів PST через службу.