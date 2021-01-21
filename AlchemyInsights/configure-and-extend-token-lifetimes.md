---
title: Настроювання й розширення терміну дії маркера
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917200"
---
# <a name="configure-and-extend-token-lifetimes"></a>Настроювання й розширення терміну дії маркера

Ви можете вказати термін дії доступу, САМЛ або ІДЕНТИФІКАТОРА, виданий платформою Microsoft Identity. Ви можете встановити термін служби маркерів для всіх програм у вашій організації, для багатоклієнтської програми (мульти-організація) або для певної основної служби в організації. Щоб отримати докладні відомості, ознайомтеся з [настроюваним терміном існування маркера](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Наприклад, ознайомтеся [з прикладами того, як настроїти тривалість роботи маркера](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Щоб дізнатися, як настроїти тривалість життя та сумісність маркера в Лазурові Active Directory B2C (Azure AD B2C), перегляньте статтю [настроїти маркери в полі Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

У статті [Настроювання поведінки сеансу в Лазур Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) описує методи єдиного входу (SSO), які використовуються в ЛАЗУРОВІ B2C, і дає змогу вибрати найбільш підходящий метод єдиного входу під час настроювання політики.

**Як довго тривають маркери? Як довго вони діють?**

Термін дії маркера – 1 година, а тривалість сеансу – 24 години. Це означає, що якщо не вдалося виконати запит протягом 24 годин, перш ніж запитувати новий маркер, потрібно знову ввійти знову.

> [!NOTE]
> Після 30 травня 2020, жоден новий клієнт не зможе використовувати настроювані правила Lifetime для настроювання сеансу та оновлення маркерів. Після цього відбудеться протягом кількох місяців після цього, що означає, що ми припиняємо на честь наявного сеансу та оновити маркери. Ви все ще можете налаштувати час існування маркера доступу після закінчення.






