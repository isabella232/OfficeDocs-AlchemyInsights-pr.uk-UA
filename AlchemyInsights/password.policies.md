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
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040851"
---
# <a name="password-policies"></a>Політики паролів

**Виникли проблеми з політикою паролів для користувача**

- Політика паролів для користувача залежить від того, чи користувач – лише в хмарі або в локальному середовищі.
- Лише в хмарі користувачі повинні вибрати пароль, який відповідає вимогам, описаним в цій статті: Політики паролів, які [застосовуються лише до хмарних облікових записів користувачів](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Локальні користувачі повинні вибрати пароль, який відповідає локальним вимогам. Якщо локальному користувачу не вдалося встановити пароль, перевірте локальні вимоги.

**Я не знаю, як установити або перевірити політики терміну дії паролів**

- За допомогою PowerShell можна встановити та перевірити політику терміну дії для користувачів хмари в цьому клієнта. Виконайте вказівки з цієї статті: [Установлення або перевірка політик паролів за допомогою PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Політика терміну дії паролів для локальних користувачів установлена в локальній ad.

**Інші корисні посилання:**
- [Початок роботи зі скиданням пароля](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Усунення несправностей, ініційованих адміністратором скидання пароля](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
