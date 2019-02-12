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
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912369"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Помилка під час надсилання електронної пошти: клієнт хост заблоковано за допомогою Spamhaus

IP-адресу, який надіслав повідомлення є блок списку належить [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Причини час заблоковано Spamhaus в розрізі порушення безпеки, скомпрометований машини обмін публічної адреси IP та Інтернет-провайдер (ISP) політики. Наведено можливі виправлення:
  
- Для заблокованого вхідних повідомлень до Office 365, де ви керуєте вихідного сервера електронної пошти вам потрібно визначити причину і видалити блок з сайту Spamhaus.
    
- Для заблокованого вхідних повідомлень до Office 365, де джерело IP-адреса належить іншому користувачу власником адрес потрібно видалити блок з сайту Spamhaus. Якщо IP-адреси на список блок політики (PBL), власник може призначити різні статичної IP-адреси або видалити адресу від на PBL.
    
- Для заблокованого вихідне повідомлення з вашого домену Office 365 ви можете отримувати цю помилку, якщо переадресовується через 3rd party службу. За допомогою інструмент пошук WHOIS для пошуку заблокованих IP адреса власника.
    

