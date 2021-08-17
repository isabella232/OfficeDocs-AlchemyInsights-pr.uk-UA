---
title: Усунення несправностей SSPR
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038979"
---
# <a name="troubleshoot-sspr"></a>Усунення несправностей SSPR

**Виникли проблеми з настроюванням скидання пароля**

- Якщо ви адміністратор і шукаєте, як увімкнути самостійне скидання пароля, див. посібник із налаштування [SSPR,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)щоб налаштувати скидання пароля в організації. Крім того, можна переглянути [вимоги до ліцензування](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). В організації має бути призначено принаймні одну ліцензію.
    - **Лише користувачі в хмарі:** Office 365 (O365) або Azure AD Basic
    - **Хмарні та/або** локальні користувачі– Azure AD Premium P1 або P2, Enterprise Mobility + Security (EMS) або Secure Productive Enterprise (SPE)
- Щоб отримати додаткові запитання про самостійне скидання пароля, перегляньте [запитання й відповіді.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**З'являється повідомлення про помилку**

Перегляньте цю статтю, щоб дізнатися про поширені помилки та способи їх вирішення: Виправлення неполадок [самостійного скидання пароля](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Виникла проблема з політикою скидання пароля**

- Якщо ваша політика скидання паролів працює не так, як очікувалося, або у вас є запитання про політики скидання паролів, ознайомтеся з цією статтею: Політики паролів і обмеження в [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Політики скидання паролів не застосовуються до адміністраторів. Корпорація Майкрософт застосовує надійну політику двогалузевого скидання пароля за замовчуванням для будь-якої ролі адміністратора Azure. Переконайтеся, що ви перевіряєте тестування з користувачем, який не є адміністратором. Докладні відомості про політику скидання адміністраторів див. в цій статті: Різниця між [політикою скидання адміністраторів.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Я не хочу, щоб мої користувачі реєструли додаткові відомості для захисту для скидання пароля**

Ви можете заповнити дані (атрибути електронної пошти та телефону) користувачами, використовуючи API, PowerShell або Azure AD Підключення. Щоб дізнатися, як це зробити:

- [Розгортання скидання пароля без потреби реєстрації користувачів](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Які дані використовуються для скидання пароля?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Я хочу, щоб мої користувачі зареєстрував додаткові відомості для захисту для скидання пароля**

1. Зареєструйте свої користувачі для самостійного скидання пароля, спрямував їм [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Після заповнення даних користувачем (користувачем або адміністратором) спрямуйте користувача на aka.ms/sspr, щоб користувачі змогли скинути власні паролі. [](https://passwordreset.microsoftonline.com/)
1. Якщо в користувачів усе ще виникають проблеми, найімолодші федеративні користувачі або **синхронізовані гешування паролів.**  Це означає, що може виникати проблема зі службою записування паролів.