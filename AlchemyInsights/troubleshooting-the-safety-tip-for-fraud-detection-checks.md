---
title: Виправлення неполадок для виявлення шахрайства, рада безпеки перевіряє
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353270"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Виправлення неполадок для виявлення шахрайства, рада безпеки перевіряє

Якщо ти отримую Безпека Підказка, яка говорить "відправник не вдалося наші чеки виявлення шахрайства і може не бути тим, ким вони, як видається, бути", а потім відправник не змогла пройти DKIM або SPF перевірки автентичності. Кращий спосіб вирішити це є для відправника авторизації себе. Якщо відправник надсилає від вашого імені, вам потрібно авторизувати їх, додавши IP адреса відправника до запису SPF.
  
Для отримання додаткової інформації див [усунення несправностей червоний (підозрілі) Безпека Підказка для виявлення шахрайства перевіряє](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Ось кілька посилань, які можуть допомогти:
  
- [Як Office 365 використовує відправника політичні рамки (SPF) для запобігання підміни](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Настроювання SPF у службі Office 365 для запобігання підміни](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
