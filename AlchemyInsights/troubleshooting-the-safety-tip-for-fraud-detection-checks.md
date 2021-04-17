---
title: Виправлення застрягання безпеки для перевірок шахрайства
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834752"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Виправлення застрягання безпеки для перевірок шахрайства

Якщо з'являється запевнення щодо безпечності, у якому сказано, що відправник не пройшов перевірку автентичності DKIM або SPF і не пройшов перевірку автентичності DKIM або SPF. Найкращий спосіб вирішити цю проблему – авторизувати самостійно відправника. Якщо відправник надсилає повідомлення від вашого імені, потрібно авторизувати їх, додавши IP-адресу відправника до запису SPF.
  
Докладні відомості див. в розділах Виправлення неполадок, пов'язаних із червоним [(підозрілим)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) застряганням щодо безпечності для перевірки шахрайства.
  
Ось ще кілька посилань, які можуть допомогти:
  
- [Запобігання спуфінгам за допомогою структури політики відправників (SPF)](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настроювання SPF для запобігання спуфінгу](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
