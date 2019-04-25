---
title: Установка office сервера терміналів - неліцензійне
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410143"
---
# <a name="installing-office-on-a-terminal-server"></a>Установка Office сервера терміналів

Для розгортання Office 365 ProPlus на сервері Windows за допомогою віддалений робочий стіл служб (РДС), раніше названий служб терміналів:
  
- Ви повинні мати Office 365 план, який включає в себе Office 365 ProPlus, таких як Office 365 підприємство E3 або E5 підприємства. Office 365 бізнесу та Office 365 бізнес преміум плани, не включають Office 365 ProPlus.
    
- Вам необхідно ввімкнути [спільний комп'ютер активації](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Якщо потрібно інсталювати Office 365 ProPlus RDS на порталі Office 365, * * *який використовує за замовчуванням установки* * *, виконайте такі дії: 
  
1. Перевірте, що плану Office 365. [Дізнайтеся, як](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Якщо необхідно, переключитися на різних Office 365 плану. [Дізнайтеся, як](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Якщо Office уже інстальовано на сервері RDS, використовуючи будь-які інші плани Office 365, видалити цей пакет оновлень. Наприклад, перейшовши до панелі керування \> видалити програму. Видаляється за допомогою [служби підтримки Microsoft і помічник відновлення](https://aka.ms/SARA-OfficeUninstall-Alchemy) , якщо ви працюєте в питаннях. 
    
4. На сервері RDS ввійдіть до порталу Office 365 з вашим обліковим записом адміністратора і [установки Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Після інсталяції Office, * * *не відкрити або увійдіть* * * до будь-якої програми Office. 
    
6. На сервері RDS увімкнути загальний комп'ютер активації за допомогою редагування реєстру, виконавши такі дії:
    
1. Клацніть правою кнопкою миші кнопку Windows в нижній лівий кут екрана та виберіть пункт запустити. У полі Відкрити введіть **regedit**а потім виберіть ОК. 
    
2. Виберіть так коли з'явиться запит на дозвіл редактор реєстру для внесення змін до пристрою.
    
3. У редакторі реєстру, додати Рядкове значення **SharedComputerLicensing** з настройкою 1 під HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. На сервері RDS * * *увійдіть як кінцевого користувача* * * і [Переконайтеся, що активація загальний комп'ютер увімкнуто для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Для більш докладної інформації про передумови, інструкції з установки а також Указівки щодо налаштувати установки за допомогою засобу розгортання Office будь ласка, дивіться [Розгортати Office 365 ProPlus за допомогою служби віддалених робочих столів](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Щоб виправити помилки, пов'язані з загальний комп'ютер активації, будь ласка, дивіться [питання виправлення неполадок з активацією загальний комп'ютер для Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

