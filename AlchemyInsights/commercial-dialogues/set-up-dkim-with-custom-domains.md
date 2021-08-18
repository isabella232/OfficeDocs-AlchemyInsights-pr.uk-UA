---
title: Налаштування DKIM із настроюваними доменами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332328"
---
# <a name="set-up-dkim-with-custom-domains"></a>Налаштування DKIM із настроюваними доменами

Потрібно опублікувати два записи CNAME для кожного настроюваного домену в СЛУЖБі DNS. Для цього використовуйте такий формат:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Примітка.** **DomainGUID** – це текст ліворуч від **імені .mail.protection.outlook.com** у настроюваному записі MX настроюваного домену (наприклад, contoso-com для домену **contoso.com).** **InitialDomain –** це домен, який використовувався, коли ви зареєструвалися в службі Office 365 (наприклад, **contoso.onmicrosoft.com).**

Докладні відомості про записи DNS див. в розділі [Створення записів DNS на веб-сайті будь-якого](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)постачальника послуг розміщення DNS Office 365.