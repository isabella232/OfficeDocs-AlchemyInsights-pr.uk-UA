---
title: Код помилки 550 5.7.501 Access denied, виявлено зловживання спамом
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044289"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>Відмовлено в доступі, виявлено зловживання спамом (550 5.7.501)

Зазвичай це повідомлення з'являється, коли користувачі надсилаються електронні листи з IP-адрес, використовуючи початковий домен *.onmicrosoft.com,* призначений новим клієнтам у Microsoft 365. Найпростіший спосіб вирішити цю проблему – зробити ось що:

1. [Додайте домен до свого клієнта.](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)

2. [Змініть основну адресу електронної пошти користувачів](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) на щойно доданий настроюваний домен.
