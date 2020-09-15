---
title: Відмовлено в доступі під час зіставлення диска з SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668764"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Вирішення проблем із бібліотеками SharePoint, зіставленими з мережними дисками

Під час переходу на зіставлений мережний диск може з'явитися одне з таких повідомлень:
  
- **\\Шлях не доступний. Можливо, у вас немає дозволу на використання цього мережевого ресурсу. Зверніться до адміністратора цього сервера, щоб дізнатися, чи є у вас дозволи на доступ.**

- **Відмовлено в доступі. Перш ніж відкривати файли в цьому розташуванні, потрібно спочатку додати веб-сайт до списку надійних сайтів, перейти до веб-сайту та вибрати параметр для автоматичного входу.**

[Отримайте довідку з виправлення неполадок із зіставленими мережевими дисками](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
Зіставлення бібліотеки як мережевого диска тимчасовий і підтримується лише в Internet Explorer. Натомість [Синхронізуйте файли SharePoint за допомогою нового клієнта синхронізації "OneDrive"](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , яка містить [файли на вимогу](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Доступ до всіх файлів у службі OneDrive без використання локального простору для сховища.
  