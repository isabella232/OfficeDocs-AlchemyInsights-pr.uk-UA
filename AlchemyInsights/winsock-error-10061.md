---
title: 1554 помилку Winsock 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420001"
---
# <a name="winsock-error-10061"></a>Помилку Winsock 10061

Цей код помилки означає, що Office 365 не міг встановити TCP сокет (підключення) з кінцевого вузла. Найбільш вірогідною причиною цієї помилки є проблеми з конфігурацією брандмауера. Щоб усунути цю проблему, перевірте ці параметри:

- Перевірте конфігурацію брандмауера з інформацією в [Office 365 URL-адрес і Вихідна IP-адреса](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Якщо повідомлення про помилку є специфічним для Exchange Online захисту (EOP), вам повинно було бути раніше повідомлення до зміни до [Exchange Online захисту IP-адрес](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Переконайтеся, що ваш інтернет-провайдер (ISP) не блокує порту.

- Перевірте, чи смарт-хоста і цільової настройки сервера у вашому сполучні лінії.

Зверніть увагу, що Office 365 не блокує *Вхідні* підключення таким чином.
