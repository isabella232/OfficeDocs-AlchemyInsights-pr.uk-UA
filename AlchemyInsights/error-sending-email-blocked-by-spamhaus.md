---
title: Помилка під час надсилання електронної пошти заблоковано SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527163"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Помилка під час надсилання електронної пошти: клієнт хост заблоковано за допомогою Spamhaus

IP-адресу, який надіслав повідомлення є блок списку належить [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Причини час заблоковано Spamhaus в розрізі порушення безпеки, скомпрометований машини обмін публічної адреси IP та Інтернет-провайдер (ISP) політики. Наведено можливі виправлення:
  
- Для заблокованого вхідних повідомлень до Office 365, де ви керуєте вихідного сервера електронної пошти вам потрібно визначити причину і видалити блок з сайту Spamhaus.

- Для заблокованого вхідних повідомлень до Office 365, де джерело IP-адреса належить іншому користувачу власником адрес потрібно видалити блок з сайту Spamhaus. Якщо IP-адреси на список блок політики (PBL), власник може призначити різні статичної IP-адреси або видалити адресу від на PBL.

- Для заблокованого вихідне повідомлення з вашого домену Office 365 ви можете отримувати цю помилку, якщо переадресовується через 3rd party службу. За допомогою інструмент пошук WHOIS для пошуку заблокованих IP адреса власника.
