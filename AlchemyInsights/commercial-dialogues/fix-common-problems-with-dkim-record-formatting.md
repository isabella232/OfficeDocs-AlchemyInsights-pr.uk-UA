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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324011"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Вирішення поширених проблем із форматуванням записів DKIM

Більшість проблем настроювання DKIM пов'язано з неправильними записами DNS.

Щоб виправити помилки настроювання DKIM, переконайтеся, що запис CNAME DKIM **(не** запис TXT) відформатовано належним чином. Докладні відомості див. в [Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Якщо вам потрібна загальна довідка із записів DNS, див. розділ Створення записів DNS для служби Office 365 на сайті [будь-якого постачальника послуг Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Примітка.** Коли ви створите або оновите записи DNS DKIM у службі розміщення DNS для свого домену, знадобиться зачекати, доки ці записи DNS не почнуть діяти.
