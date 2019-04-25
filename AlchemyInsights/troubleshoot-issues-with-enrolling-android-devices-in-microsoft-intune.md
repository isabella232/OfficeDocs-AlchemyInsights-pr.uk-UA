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
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420613"
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
    

