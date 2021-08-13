---
title: Access denied when mapping a drive to SharePoint
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
ms.openlocfilehash: 1ed67ec926c3e73f7a16b927729255505dfe93a0ae442a5dff9400afafb41d8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938752"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Вирішення проблем із SharePoint бібліотеками, зіставленими з мережевими дисками

Під час переходу до підключеного мережевого диска може з'явитися одне з таких повідомлень:
  
- **\\Шлях недоступний. Можливо, у вас немає дозволу на використання цього мережевого ресурсу. Зверніться до адміністратора цього сервера, щоб дізнатися, чи маєте ви дозволи на доступ.**

- **Access Denied. Перш ніж відкривати файли в цьому розташуванні, потрібно спочатку додати веб-сайт до списку надійних сайтів, перейти на веб-сайт і вибрати параметр для автоматичного входу.**

[Отримайте довідку з виправлення неполадок підключених мережевих дисків](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
Зіставлення бібліотеки як мережевого диска тимчасове та підтримується лише в браузері Internet Explorer. Натомість [синхронізуйте SharePoint за допомогою нового](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) клієнта синхронізатор OneDrive який містить файли на [вимогу.](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx) Отримуйте доступ до всіх файлів у OneDrive, не використовуючи локальний простір для зберігання.
  