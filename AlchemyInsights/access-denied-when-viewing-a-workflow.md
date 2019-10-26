---
title: Відмовлено в доступі під час перегляду робочого процесу
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747769"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Відмовлено в доступі під час перегляду робочого процесу

SharePoint 2013 робочих циклів, які намагаються надіслати повідомлення електронної пошти до групи SharePoint може не з повідомлення про помилку "немає доступу", якщо членство групи SharePoint не встановлено для всіх.
  
 **Щоб вирішити цю проблему, виконайте такі дії:**
  
 1. Дозволити всім користувачам бачити учасників групи SharePoint.
  
 2. Видалити групу SharePoint, з до або копія рядок повідомлення електронної пошти.
  
 3. Явно додати користувачів до рядка кому або копія, якщо видимість членства не можна змінити для групи SharePoint.
  
Для перегляду більш докладної інформації, будь ласка, зверніться до [http несанкціонований/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  