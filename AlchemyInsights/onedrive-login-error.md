---
title: OneDrive входу AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112933"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive входу AADSTS50011

Якщо під час входу в програму OneDrive відображається повідомлення про помилку "AADSTS50011: URL-адреса відповіді, указана в запиті, не збігається з відповіддю" під час входу в програму OneDrive, перевірте таке:

Ваша OneDrive має бути дорівнювати або більшою за версію 20.052.XXXX.XXXX. Щоб перевірити свою версію, клацніть синю піктограму OneDrive в області сповіщень, виберіть **Довідка & Настройки > Настройки > Про програму**.

Ваша мережа може блокувати трафік до **g.live.com** та **oneclient.sfx.ms**. Якщо цей трафік заблоковано, його OneDrive оновити самостійно. Зверніться до адміністратора мережі, щоб переконатися, що ви маєте доступ до цих URL-адрес. [Ці кінцеві точки](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) мають бути доступні клієнтам, які Microsoft 365 планами.

Якщо потрібно вручну отримати поточну версію пакета OneDrive, відвідайте веб-сайт [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
