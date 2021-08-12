---
title: Виправлення неполадок, застереження щодо безпечності перевіряти шахрайство
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955987"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Виправлення неполадок, застереження щодо безпечності перевіряти шахрайство

Якщо з'являється повідомлення "Відправник не застереження щодо безпечності перевірки виявлення шахрайства та може бути не таким, як вони виглядають", відправнику не вдалося пройти перевірку автентифікації DKIM або SPF. Найкращий спосіб вирішити цю проблему – авторизувати самостійно відправника. Якщо відправник надсилає повідомлення від вашого імені, потрібно авторизувати їх, додавши IP-адресу відправника до запису SPF.
  
Докладні [відомості див.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) в застереження щодо безпечності для перевірки виявлення шахрайства в червоному (підозрілому) виправлення неполадок.
  
Ось ще кілька посилань, які можуть допомогти:
  
- [Запобігання спуфінгам за допомогою структури політики відправників (SPF)](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настроювання SPF для запобігання спуфінгу](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
