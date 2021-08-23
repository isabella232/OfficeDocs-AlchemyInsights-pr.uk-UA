---
title: Вимкнення TLS1.0 і TLS 1.1 для надсилання клієнта SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455129"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Вимкнення TLS1.0 і TLS 1.1 для надсилання клієнта SMTP AUTH

Нещодавно ми почали вимикати надсилання TLS1.0 і TLS 1.1 для клієнта SMTP AUTH. 

Якщо ви настроїли пристрій, програму або сервер, що надсилає електронну пошту на Microsoft 365 за допомогою методу надсилання через клієнт SMTP AUTH, переконайтеся, що пристрій, програма або сервер підтримують TLS 1.2 для SMTP. 