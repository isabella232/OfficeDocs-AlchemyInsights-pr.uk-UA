---
title: Зміна параметрів обмеження трафіку у веб-службах Exchange (EWS)
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818057"
---
# <a name="changing-ews-throttling-settings"></a>Зміна параметрів обмеження трафіку у веб-службах Exchange (EWS)

Запустіть нашу автоматичну перевірку, щоб змінити політику обмеження трафіку для EWS на час перенесення. Зверніть увагу, що навіть після цієї перевірки імпорт EWS буде обмежено до 150 МБ на 5 хвилин для однієї поштової скриньки. Щоб досягти кращої пропускної здатності під час перенесення, рекомендується переносити більше користувачів одночасно.

Зверніть увагу, що зміни політики обмеження трафіку для EWS не впливають на такі типи перенесення (за допомогою інструментів Microsoft): гібридне, повне чи поетапне (з використанням віддаленого виклику процедур та HTTP), IMAP, G Suite, а також перенесення спільних папок чи імпорт файлів PST через службу.