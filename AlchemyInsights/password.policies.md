---
title: Політики паролів
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747057"
---
# <a name="password-policies"></a>Політики паролів

**У мене виникли проблеми з політикою паролів для користувача**

- Політика паролів для користувача залежить від того, чи є користувач хмарним або локальною.
- Хмарні лише користувачі мають вибрати пароль, який відповідає вимогам цієї статті: [політики паролів, які застосовуватимуться лише до облікових записів користувачів у хмарі](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) .
- Локальні користувачі мають вибрати пароль, який відповідає локальним вимогам. Якщо локальний користувач не може встановити пароль, перевірте свої локальні вимоги.

**Я не знаю, як установлювати або перевіряти політики терміну дії паролів**

- Ви можете встановити та перевірити політику терміну дії для хмарних користувачів у клієнті за допомогою PowerShell. Виконайте вказівки, описані в цій статті: [Установлення або перевірка політик паролів за допомогою PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Політика терміну дії пароля для локальних користувачів встановлюється в локальній службі AD.

**Інші корисні посилання:**
- [Початок роботи з Скидмою пароля](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Виправлення неполадок із Скидленням пароля адміністратора](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
