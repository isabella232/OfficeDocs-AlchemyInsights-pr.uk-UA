---
title: Регулювання SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931463"
---
# <a name="sharepoint-online-throttling"></a>Регулювання SharePoint Online

**Важливо**: багато SharePoint Online і OneDrive клієнтів, запустіть бізнес-критичних програм від служби, які працюють у фоновому режимі. До них відносяться міграція вмісту, запобігання втрати даних (ЗВД) і рішення для резервного копіювання. У ці безпрецедентні часи Ми вживаємо заходів, щоб гарантувати, що служби SharePoint Online та OneDrive залишаються дуже доступними та надійними для користувачів, які залежать від служби, ніж будь-коли в віддалених сценаріях роботи.

На підтримку цієї мети, ми реалізували жорсткі обмеження регулювання на фонових програм (міграція, ЗВД і резервне копіювання рішень) в будні дні вдень. Ви повинні очікувати, що ці програми будуть досягати дуже обмежену пропускну здатність в ці часи. Однак під час вечірніх та вихідних годин для регіону служба буде готова обробляти значно більший обсяг запитів від фонових програм.

**Регулювання SharePoint Online**

SharePoint Online використовує дроселювання для підтримки оптимальної продуктивності та надійності служби SharePoint Online. Дроселювання обмежує кількість дій користувача або одночасних викликів (за сценарієм або кодом) для запобігання надмірного використання ресурсів. Для отримання додаткової інформації, будь ласка, відвідайте посилання нижче.

- [Уникайте отримання обмежено або заблоковано в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Міграція даних і дроселювання](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [Швидкість міграції SharePoint Online та OneDrive](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [Обробляти в SharePoint Online дроселювання за допомогою експоненційного назад](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Планування потужностей та тестування навантаження SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

