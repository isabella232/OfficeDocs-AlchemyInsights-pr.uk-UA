---
title: Помилка 1554 Winsock 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698883"
---
# <a name="winsock-error-10061"></a>Помилка "Winsock 10061"

Цей код помилки означає, що корпорація Майкрософт не може встановити TCP-роз'єм (підключення) із цільовим хостом. Скоріш за все, причиною цієї помилки є проблема з конфігурацією брандмауера. Щоб вирішити цю проблему, перевірте ці параметри.

- Перевірка конфігурації брандмауера за відомостями в [діапазонах URL-адрес і IP-адрес Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Якщо ця помилка стосується захисту Exchange Online (EOP), ви повинні були попередньо проінформовані про змінення [IP-адрес захисту Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Переконайтеся, що ваш постачальник послуг Інтернету (ISP) не блокує порт.

- Перевірте настройки смарт-хоста та цільового сервера в сполуках.

Зверніть увагу, що корпорація Майкрософт 365 не блокує *Вхідні* підключення таким чином.
