---
title: Виправлення неполадок підказки безпеки для виявлення шахрайства перевірки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505004"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Виправлення неполадок підказки безпеки для виявлення шахрайства перевірки

Якщо ви отримуєте безпеки відгук, який говорить: "відправник не вдалося наші перевірки шахрайства перевіряє і не може бути, хто вони здаються", то відправник не вдалося передати або DKIM або SPF перевірки автентичності. Найкращий спосіб вирішити це для відправника, щоб авторизуватися. Якщо відправник розсилає відправлення від вашого імені, вам необхідно авторизувати їх, додавши ІР-адресу відправника до запису SPF.
  
Перегляньте [Виправлення неполадок Червоної (підозрілої) підказки щодо безпеки для виявлення шахрайства](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) для отримання додаткових відомостей.
  
Ось деякі інші посилання, які можуть допомогти:
  
- [Як корпорація Майкрософт використовує Framework політики відправника (SPF), щоб запобігти спуфінгу](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Налаштуйте SPF, щоб запобігти спуфінгу](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
