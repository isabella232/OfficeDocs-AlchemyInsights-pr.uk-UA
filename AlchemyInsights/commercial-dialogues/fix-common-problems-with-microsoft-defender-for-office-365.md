---
title: Вирішення поширених проблем із Захисником Microsoft для Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898265"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Вирішення поширених проблем із Захисником Microsoft для Office 365

Ось кілька способів вирішення поширених проблем із Захисником Microsoft для Office 365:

- **Затримка повідомлення:**

  Затримки доставки електронної пошти можуть спричиняти Сейф перевірок вкладень повідомлень. Докладні відомості див. [в Сейф параметри політики вкладень.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Повідомити про хибні додатні або від'ємні результати:**

  Докладні відомості див. в [статті Звітування про повідомлення та файли до корпорації Майкрософт.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Увімкніть Сейф Захист посилань:**

  1. На порталі Microsoft 365 Defender перейдіть до розділу Політики співпраці & електронної <https://security.microsoft.com/> **пошти** \> **&** \> **правилами** Сейф \>   посилання в розділі Політики.

     Щоб перейти безпосередньо на сторінку **посилання Сейф,** скористайтеся <https://security.microsoft.com/safelinksv2> .

  2. На сторінці **Сейф Посилання** виберіть політику, клацнувши ім'я політики.
  3. У вікні відомостей, що з'являться, виконайте одну з таких дій:
     - Щоб додати нову політику, виберіть **+ Створити**. Запуститься майстер, який допоможе визначити параметри політики.
     - Щоб змінити наявну політику, виберіть її, клацнувши ім'я політики. У вікні відомостей, що з'являться, виберіть **Редагувати** в **розділі Параметри** захисту.
  4. На сторінці **Параметри захисту** налаштуйте такі параметри:
     - Увімкніть параметр Виберіть дію для **потенційно зловмисних URL-адрес у повідомленнях.**
     - Виберіть **Елемент Застосувати безпечні посилання до повідомлень, надісланих у межах організації.**

  Докладні відомості див. [в статті Налаштування політик посилань Сейф в Microsoft Defender для Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
