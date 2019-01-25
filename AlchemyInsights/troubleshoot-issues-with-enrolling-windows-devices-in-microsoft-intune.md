---
title: Усунення несправностей із зарахування пристроїв Windows у корпорації Майкрософт Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495891"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Усунення несправностей із зарахування пристроїв Windows у корпорації Майкрософт Intune

Огляд ресурсів, перераховані нижче, щоб вирішити проблему, ваш тепер. 
  
Деякі поширені повідомлення про помилки та резолюції кроки:
  
 **Не вдалося інсталювати програмне забезпечення, 0x80cf4017:** Ваш обліковий запис сертифіката закінчився. Повторно завантажити пакет програмного забезпечення ПК клієнта в консолі адміністратора Intune. Огляд цієї документації для отримання додаткової інформації. 
  
 **Код помилки 0x801c0003:** Помилка може виникнути у таких випадках: 
  
1. Користувач має додаткові пристрої вступив ніж пристрою обмеження. Перегляньте ці документи до [зняття пристрою](https://docs.microsoft.com/en-us/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Користувачі можуть приєднатися до пристроїв блакитні об'яви" встановлено значення "немає". Встановіть його на всіх, або виберіть користувачів. Огляд [цієї документації](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) для отримання додаткової інформації. 
    
3. Пристрою вже зареєстровано іншим користувачем. Якщо це так, видалити пристрій з Azure Intune консоль або вручну unenroll пристрій, перш ніж повторити спробу.
    
4. Становить 10 Windows Home. Тільки Windows 10 Pro, освіти та рішенню щодо підприємства можуть приєднатися до Azure Active Directory.
    
Додаткові ресурси, щоб допомогти вирішити вашу проблему:
  
1. Використовувати [Intune виправлення неполадок портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) діагностувати та усунути поширені зарахування невдач. Огляд [цей документ](https://docs.microsoft.com/en-us/intune/help-desk-operators) для більш докладної інформації. 
    
2. Перегляньте ці документи список поширених помилок, які заважають заявки на участь та постанов до кожного: [усунення несправностей керівництво](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) та [усунення несправностей doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Дізнайтеся, як записатися пристроїв Windows у корпорації Майкрософт Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

