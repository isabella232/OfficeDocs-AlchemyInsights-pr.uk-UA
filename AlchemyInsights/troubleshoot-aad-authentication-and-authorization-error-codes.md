---
title: Усунення несправностей із кодами помилок автентифікації Azure AD і авторизації (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037843"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Усунення несправностей із кодами помилок автентифікації Azure AD і авторизації (AADSTS)

Щоб вирішити помилки автентифікації AAD і коди помилок авторизації (AADSTS), виконайте наведені нижче Рекомендовані дії.

1. **Оброблення кодів помилок у програмі**

- Функція **OAuth 2.0 Spec** https://tools.ietf.org/html/rfc6749#section-5.2 дає вказівки про те, як обробляти помилки під час автентифікації за допомогою частини помилки під час відповіді на помилку.

    - **Помилка**: рядок коду помилки, який можна використовувати для класифікації типів помилок, які трапляються, і їх слід використовувати для реагування на помилки.
    - У полі " **Помилка** " є кілька можливих значень: огляд посилань на протоколи документації та "oauth 2,0 специфікації" для отримання додаткових відомостей про певні помилки та способи їх реагування на них.

- Нижче наведено зразок відповіді про помилку:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Підстановка поточних відомостей про код помилки**

- Коди помилок і повідомлення можуть змінюватися. Щоб отримати найактуальніші відомості, перегляньте https://login.microsoftonline.com/error сторінку, щоб знайти описи помилок AADSTS, виправлення та деякі запропоновані способи вирішення.
- Ви також можете шукати та усувати [коди помилок Aadsts](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , перелічені в розділі [коди автентифікації в статті Azure AD і помилки авторизації](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Отримання довідки**

- [Варіанти підтримки та довідки для розробників](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – якщо вам потрібна відповідь на запитання або довідку з вирішення проблем, не охоплених нашою документацією, можливо, настав час охопити фахівців для довідки. У цій статті наведено кілька порад, які допоможуть отримати відповіді на запитання, коли ви розробляєте програми, які інтегруються з платформою ідентифікації Microsoft.








