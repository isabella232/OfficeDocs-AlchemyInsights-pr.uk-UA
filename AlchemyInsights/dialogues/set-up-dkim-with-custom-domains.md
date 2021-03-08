---
title: Настроювання DKIM з настроюваними доменами
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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527269"
---
# <a name="set-up-dkim-with-custom-domains"></a>Настроювання DKIM з настроюваними доменами

Потрібно опублікувати два записи CNAME для кожного настроюваного домену в службі DNS. Для цього використовуйте такий формат:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **Domainідентифікатором** – це текст зліва від **. mail.Protection.Outlook.com** у настроюваному записі MX для настроюваного домену (наприклад, contoso-com для домену **contoso.com**). **Ім'я _ домену** – це домен, який ви використовували під час реєстрації в Office 365 (наприклад, **contoso.onmicrosoft.com**).

Докладні відомості про записи DNS наведено в статті [створення записів DNS на сайті будь-якого постачальника послуг розміщення DNS для Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).