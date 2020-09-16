---
title: Під час фіксації програм Microsoft 365 не вдалося знайти зв'язане повідомлення про ліцензії Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747716"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Виправлення програм Microsoft 365 "не вдалося знайти повідомлення, пов'язані з ліцензіями Office"

Якщо ви отримали це повідомлення, виконайте наведені нижче дії.

1. Перевірте брандмауер, антивірусне програмне забезпечення та параметри проксі-сервера, щоб підтвердити, що вони не блокують доступ до Інтернету до програм Microsoft 365. Переглянути [URL-адреси Microsoft 365 і діапазони IP-адрес](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Видаліть і [Перепризначте ліцензію Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) для постраждалому користувачу. 
3. Відкрийте програму Office і [вийдіть](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) із наявних облікових записів користувачів.
4. Перейдіть до параметрів Windows > **облікові**записи  >  **електронної пошти & облікових записів**і видаліть усі робочі облікові записи, окрім облікового запису, який впливає на обліковий запис.
5. Перейдіть до настройок Windows > **облікові записи**для  >  **роботи або навчального закладу**, а також відключіть усі робочі облікові записи, окрім облікового запису, який впливає на нього.
6. Скидання стану активації Office. [Дізнайтеся, як це зробити](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Увійдіть](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) за допомогою облікового запису користувача, що вплинуло.

Додаткові рішення щодо виправлення неполадок наведено [в статті неліцензований продукт і помилки активації в Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).