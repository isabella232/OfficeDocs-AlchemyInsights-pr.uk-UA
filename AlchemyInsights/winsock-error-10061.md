---
title: Помилка 10061 (1554 winsock)
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083251"
---
# <a name="winsock-error-10061"></a>Помилка 10061 у winsock

Цей код помилки означає, що корпорації Майкрософт не вдалося встановити для цільового хоста сокет TCP (підключення). Найімолодніша причина цієї помилки – проблема з конфігурацією брандмауера. Щоб вирішити цю проблему, перевірте ці параметри:

- Перевірте конфігурацію брандмауера за допомогою [відомостей у діапазонах URL Microsoft 365 URL- і IP-адрес.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Якщо ця помилка характерна Exchange Online Protection (EOP), вам потрібно було повідомити про зміну IP-адрес Exchange Online Protection [адрес.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Переконайтеся, що ваш інтернет-провайдер не блокує порт.

- Перевірте параметри смарт-вузла та цільового сервера в з'єдначах.

Зверніть увагу Microsoft 365 що вхідні підключення не *блокуватимуться* таким чином.
