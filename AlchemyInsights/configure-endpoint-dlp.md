---
title: Налаштування Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892820"
---
# <a name="configure-endpoint-dlp"></a>Налаштування Endpoint DLP

Microsoft Endpoint DLP дає змогу використовувати захист і моніторинг ЗВД для делікатної інформації на пристроях із Windows 10. Після приєднання пристроїв до системи керування пристроями можна створити політики ЗВД, щоб застосовувати захисні дії до елементів. Для моніторингу дій із делікатними елементами можна використовувати оглядач діяльності. Докладні відомості див. в статті [Приєднання пристроїв до системи керування пристроями](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Щоб почати роботу з Endpoint DLP:

- Переконайтеся, що у вас є відповідні ліцензії на продукти або передплачені ліцензії. Докладні відомості див. в статті [Ліцензії на продукти або передплачені ліцензії](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Перевірте наявність дозволів, необхідних для вмикання керування пристроями, доступу до сторінки приєднання та вмикання або вимикання моніторингу пристроїв. Докладні відомості див. в статті [Дозволи](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Приєднайте пристрої до системи керування пристроями за допомогою відповідної процедури. Докладні відомості див. в статті [Приєднання пристроїв](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Створіть політики ЗВД для захисту делікатних елементів. Відомості див. в статті [Сценарії політики захисту від втрати даних у кінцевих точках](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Додаткові відомості про Microsoft Endpoint DLP див. в статті [Відомості про Захист від втрати даних у кінцевих точках Microsoft 365 (підготовча версія)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Важливі кроки зі збирання даних у разі необхідності підтримки:**

1. [Завантажте аналізатор клієнта MDATP Preview.](https://aka.ms/betamdatpanalyzer)
1. Запустіть інструмент як адміністратор із вікна командного рядка:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Коли з'явиться запит із запитом введіть кількість хвилин для збирання **трасування:**, введіть кількість хвилин, потрібних для запуску сценарію.
1. Виконайте сценарій.

Зберіть вихідні дані ZIP-файлу, щоб надати агенту підтримки.
