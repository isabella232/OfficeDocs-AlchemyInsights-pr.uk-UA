---
title: Віртуальна конфігурація з службами доменів AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885654"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Віртуальна конфігурація з службами доменів AAD

Віртуальна конфігурація з службами доменів AAD включає наведені нижче дії. 

1. Перевірка справності вашого домену на порталі «Лазурний» https://aka.ms/aadds-health
2. Перевірка НСГ для правил, які блокують порти, необхідні для синхронізації в службі "Azure domain AD" на порталі https://aka.ms/aadds-networking
3. Переконайтеся, що віртуальну мережу розгорнуто в тій самій Лазужній області, як-от домен Azure AD служби доменів.
4. Переконайтеся, що у вас немає наявного домену з таким самим іменем домену, доступним у віртуальній мережі.

Щоб отримати докладні відомості про розгляд у віртуальній мережі Azure Virtual Network для підтримки служб домену AAD, ознайомтеся з відомостями про [віртуальну мережу](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

