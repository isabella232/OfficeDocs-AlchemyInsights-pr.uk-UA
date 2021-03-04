---
title: Виправлення неполадок із SУРП
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430362"
---
# <a name="troubleshoot-sspr"></a>Виправлення неполадок із SУРП

**У мене виникли проблеми з настроюванням скидання пароля**

- Якщо ви адміністратор і шукаєте, як можна ввімкнути скидання пароля самостійно, ознайомтеся з посібником з [ввімкнення функції sурп](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), щоб настроїти скидання пароля для вашої організації. Ви також можете переглянути [вимоги до ліцензування](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Потрібно мати принаймні одну ліцензію, призначену в організації.
    - **Хмарні тільки користувачі** – будь-який Office 365 (O365) платний обліковий номер або ЛАЗУРНЕ AD Basic
    - **Хмарні та/або Локальні користувачі** – AZURE AD Premium P1 або P2, Enterprise Mobility + Security (EMS) або захищене продуктивне підприємство (SPE).
- Щоб отримати додаткові запитання про скидання пароля служби самообслуговування, перегляньте [наші запитання й відповіді](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Я можу отримати повідомлення про помилку**

Перегляньте цю статтю, щоб отримати поширені помилки та їх вирішення: [Виправлення неполадок із скидленням пароля для самостійного обслуговування](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Виникла проблема з політикою скидання пароля**

- Якщо політика скидання пароля не працює належним чином, або якщо у вас виникли запитання про політику скидання пароля, перегляньте цю статтю: [політики паролів і обмеження в Лазурому Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Політики скидання пароля не застосовуватимуться до адміністраторів. Корпорація Майкрософт забезпечує сильну політику скидання пароля за два ворота за замовчуванням для будь-якого ролі «Лазурний адміністратор». Переконайтеся, що ви тестуєте з користувачем, який не є адміністратором. Докладні відомості про політику скидання адміністратора наведено в статті: [відмінності політики скидання адміністратора](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Я не хочу, щоб користувачі зареєструвати додаткові відомості про безпеку для скидання пароля**

Ви можете попередньо заповнити дані (електронні листи та телефонні атрибути) для користувачів за допомогою API, PowerShell або Azure AD Connect. Дізнайтеся, як читати:

- [Розгортання скидання пароля без необхідності реєструвати користувачів](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Дані, які використовуються для скидання пароля](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Я хочу, щоб користувачі зареєструвати свої додаткові відомості про безпеку для скидання пароля**

1. Попросіть користувачів зареєструвати свою інформацію про безпеку для скидання пароля служби самообслуговування, спрямовуючи їх на [AKA.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Після заповнення даних для користувача (користувачем або адміністратором) спрямувати користувача на [AKA.MS/sspr](https://passwordreset.microsoftonline.com/) , щоб користувачі могли мати можливість скинути власні паролі.
1. Якщо користувачі все ще зазнають проблем, які вони найчастіше можуть використовувати **Федеративні** або **гешування паролів** користувачів. Це означає, що скоріш за все виникла проблема з Wriliback для роботи з паролем.