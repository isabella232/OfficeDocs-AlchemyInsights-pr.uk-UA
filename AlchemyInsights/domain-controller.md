---
title: Контролер домену
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901318"
---
# <a name="domain-controller"></a>Контролер домену

**Не вдається ввімкнути AAD-DS або розгортання не вдається**

Щоб вирішити проблему, яка не активується (AAD-DS) не ввімкнуто або не вдається розгорнути, виконайте наведені нижче дії.

1. Якщо ви використовуєте вже наявну віртуальну мережу, перевірте свої правила, які блокують порти, необхідні для синхронізації в AAD-DS на порталі https://aka.ms/aadds-networking .
2. Перевірте, чи відповідь на повідомлення про помилку в цьому посібнику з виправлення неполадок, доступний у програмі  https://aka.ms/aadds-troubleshoot-enable .
3. У новій віртуальній мережі можна виконати розгортання служб для домену Azure AD.
4. Виконайте посібник із початку роботи, щоб розгорнути AAD-DS, який можна отримати в [Посібнику з створення служб домену Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Якщо у вас виникли проблеми з розгортанням служб домену Azure AD, перегляньте статтю [Виправлення неполадок служби "Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) " для вирішення поширених помилок, щоб допомогти вам знову працювати з ними. 

**Не вдається вимкнути AAD-DS**

AAD-DS не може бути призупинено. Якщо ви хочете припинити використовувати керований домен, його потрібно видалити.

Якщо ви зіткнулися з проблемами, щоб вирішити поширені повідомлення про помилки, а також пов'язані з ними кроки з виправлення неполадок, щоб допомогти вам знову працювати з ними, ознайомтеся з [усуненням служб домену "Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)"
