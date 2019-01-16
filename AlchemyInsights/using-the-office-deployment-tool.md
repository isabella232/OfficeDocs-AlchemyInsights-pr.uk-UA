---
title: За допомогою Office виконання засобу розгортання
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319539"
---
# <a name="using-the-office-deployment-tool-odt"></a>За допомогою засобу розгортання Office (у форматі ODT)

Ви використовуєте в офісі розгортання інструмент (у форматі ODT) розгортати Office 365 у версіях Office. Розгортання засобу Office (setup.exe) запустити з командного рядка і використовує XML-файлі конфігурації, щоб визначити, які параметри для застосування під час розгортання Office.
  
1. Завантажити останню версію Office виконання засобу розгортання з [Центру завантажень Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. За допомогою [Office на приладі (жовтень)](https://config.office.com) виберіть ваші уподобання розгортання і створити XML-файл конфігурації. Експортувати файл конфігурації і пок локально ж папку, де проживає на setup.exe. 
    
    **Примітка:** Зазвичай виникають проблеми через до неправильно налаштований інсталяції Office або malformatted конфігураційних файлів. Щоб уникнути таких проблем, рекомендовано використовувати Office приладі створити файл конфігурації. Ви також можете імпортувати наявні файли конфігурації в приладі Office. 
    
3. Від підвищеної командного рядка перейдіть до розташування, де setup.exe проживає і запустити засіб розгортання офіс в режим завантаження і вказати щойно збережений файл конфігурації. У цьому прикладі файл конфігурації називається Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Запуск засобу розгортання офіс в налаштування режиму та вкажіть відповідний файл конфігурації.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Примітка:** Ви повинні запустити цей крок з клієнтського комп'ютера, на якому потрібно інсталювати Office і дозвіл місцевого адміністратора на цьому комп'ютері. 
    
Щоб дізнатися більше про інструментом Office розгортання для Office 365 ProPlus сценаріїв розгортання, переглянути [Огляд розгортання засобу Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Для більш докладної інформації про те, як використовувати засіб настройок Office переглянути [Огляд Office приладі](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

