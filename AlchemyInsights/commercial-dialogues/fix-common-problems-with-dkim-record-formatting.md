---
title: Вирішення поширених проблем із форматуванням записів DKIM
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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930082"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Вирішення поширених проблем із форматуванням записів DKIM

Більшість проблем настроювання DKIM пов'язано з неправильними записами DNS.

Щоб виправити помилки настроювання DKIM, переконайтеся, що запис CNAME DKIM **(не** запис TXT) відформатовано належним чином. Докладні відомості див. [в цій](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)Office 365.

Якщо вам потрібна загальна довідка із записів DNS, див. розділ Створення записів DNS для служби Office 365 на сайті [будь-якого постачальника Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Коли ви створите або оновите записи DNS DKIM у службі розміщення DNS для свого домену, доведеться зачекати, доки ці записи DNS не почнуть діяти.
