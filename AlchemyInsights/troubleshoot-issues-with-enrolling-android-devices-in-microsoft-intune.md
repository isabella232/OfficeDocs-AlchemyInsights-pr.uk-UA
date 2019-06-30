---
title: Усунення несправностей із зарахування Android пристроїв у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367310"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Усунення несправностей із зарахування Android пристроїв у Microsoft Intune

Огляд ресурсів, перераховані нижче, щоб вирішити проблему, ваш тепер.
  
Деякі загальні питання і резолюції кроки:
  
 **Пристрої не зашифровані помилка на порталі компанії:** Новіші версії Android, особливо починаючи з v 7.0, вимагають запуску ввести пароль, щоб переконатися, що ваш пристрій повністю шифрується. Спільні рішення, щоб увімкнути автозавантаження PIN-код або повністю зашифрувати пристрою. Огляд [цей документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) для отримання додаткової інформації.
  
 **Пристрої не заглядати Intune служби або відобразити як "Нездорових" в консолі адміністратора Intune:** Деякі Samsung 4.4 і 5,5 пристроїв не можуть перевірити на службу. Існує 3 можливих рішень цієї проблеми:
  
1. Вручну відкрити портал компанії Intune програма, яка буде автоматично ініціювати пристрій синхронізації.

2. Оновити пристрій Android 6.0 або вище.

3. Вимкнути Samsung смарт-менеджер з управління портал компанії Intune. Огляд [цей документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) для більш докладної інформації з цих питань і резолюцій.

 **Користувача ліцензії типу неприпустимий** або **користувач ім'я не розпізнано помилка:** що користувачеві необхідно призначити Intune або EMS ліцензії. Перегляньте ці документи до призначите ліцензію через: офіс центру адміністрування або Azure порталу.
  
Додаткові ресурси, щоб допомогти вирішити вашу проблему:
  
1. Використовувати [Intune виправлення неполадок портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) діагностувати та усунути поширені зарахування невдач. Огляд [цей документ](https://docs.microsoft.com/intune/help-desk-operators) для більш докладної інформації.

2. Огляд [цей документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) список поширених помилок, які заважають заявки на участь та постанов до кожного.

3. [Дізнайтеся, як записатися Android пристроїв у Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
