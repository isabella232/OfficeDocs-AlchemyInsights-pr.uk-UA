---
title: 1554 Winsock помилка 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766190"
---
# <a name="winsock-error-10061"></a>Winsock помилка 10061

Цей код помилки означає, що корпорація Майкрософт не може встановити TCP-сокет (підключення) з цільового хоста. Найбільш вірогідною причиною цієї помилки є проблема з конфігурацією брандмауера. Щоб вирішити цю проблему, перевірте, чи ці параметри:

- Перевірте конфігурацію брандмауера з відомостями в [Microsoft 365 URL-адрес і діапазонів IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Якщо повідомлення про помилку, специфічні для Exchange Online захисту (кінець періоду), ви повинні були раніше повідомлені зміни в [Exchange Online захист IP-адрес](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Переконайтеся, що ваш інтернет-провайдер (ISP) не блокує порт.

- Перевірте настройки смарт-хоста та цільового сервера в з'єднувачів.

Зверніть увагу, що Microsoft 365 не блокує *Вхідні* підключення таким чином.
