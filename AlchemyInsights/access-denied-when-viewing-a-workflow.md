---
title: Під час перегляду робочого циклу відмовлено в доступі
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688823"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Під час перегляду робочого циклу відмовлено в доступі

Робочі цикли SharePoint 2013, які намагаються надіслати повідомлення електронної пошти до групи SharePoint, можуть не працювати з повідомленням про помилку "відмовлено в доступі", якщо членство в групі SharePoint не настроєно для всіх користувачів.
  
 **Щоб вирішити цю проблему, виконайте наведені нижче дії.**
  
 1. Дозволити всім користувачам бачити учасників групи SharePoint.
  
 2. Видаліть групу SharePoint із рядка "Кому" або "Копія" повідомлення електронної пошти.
  
 3. Явно додати користувачів до рядка "Кому" або "Копія", якщо видимість членства не можна змінити для групи SharePoint.
  
Щоб переглянути докладні відомості, зверніться до [http-неавторизованого доступу до/_vti_bin/Client.SVC/SP.utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  