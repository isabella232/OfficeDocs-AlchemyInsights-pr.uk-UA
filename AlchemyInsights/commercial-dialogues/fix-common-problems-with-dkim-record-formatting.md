---
title: Виправлення поширених проблем із форматуванням запису DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750752"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Виправлення поширених проблем із форматуванням запису DKIM

Більшість проблем із настроюванням DKIM пов'язані з неправильними записами DNS.

Щоб виправити проблеми з настроюванням DKIM, переконайтеся, що запис DKIM CNAME (**не** запис txt) відформатовано правильно. Щоб отримати докладніші відомості, Дізнайтеся, [що потрібно зробити, щоб вручну налаштувати DKIM в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Якщо вам потрібна Довідка з записів DNS загалом, перегляньте статтю [створення записів DNS на сайті будь-якого постачальника послуг розміщення DNS для Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Створивши або оновіть записи DNS DKIM у службі розміщення DNS для свого домену, необхідно зачекати, доки записи DNS потрібно буде розповсюдити.
