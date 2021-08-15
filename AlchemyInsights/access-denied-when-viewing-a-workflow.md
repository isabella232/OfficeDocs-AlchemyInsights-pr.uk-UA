---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955222"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint 2013 робочих циклів, які намагаються надіслати повідомлення електронної пошти групі SharePoint, може виникнути помилка з повідомленням про помилку "Немає доступу", якщо учасник групи SharePoint не встановлено значення "Усі".
  
 **Щоб вирішити цю проблему, виконайте такі дії:**
  
 1. Дозвольте всім користувачам переглядати учасників SharePoint групи.
  
 2. Видалити групу SharePoint з рядка Кому або Копія електронного листа.
  
 3. Явно додайте користувачів до рядка Кому або Копія, якщо не можна змінити видимість членства для SharePoint групі.
  
Докладні відомості див. в [статті HTTP Неавторизовано на адресу /_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  