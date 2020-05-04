---
title: Використання засобу розгортання Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010894"
---
# <a name="using-the-office-deployment-tool-odt"></a>Використання засобу розгортання Office (ODT)

Для розгортання Office 365 версії Office використовується засіб розгортання Office (ODT). Засіб розгортання Office (Setup. exe) запускається з командного рядка та використовує XML-файл конфігурації, щоб визначити, які параметри застосовувати під час розгортання Office.
  
1. Завантажити останню версію засобу розгортання Office, з [центру завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Скористайтеся [засобом настроювання Office (Oct)](https://config.office.com) , щоб вибрати параметри розгортання та створити XML-файл конфігурації. Експортуйте конфігураційний файл і розмістіть його локально в тій самій теці, де знаходиться програма Setup. exe.

    **Примітка:** Проблеми з інсталяцією Office зазвичай виникають через неправильно налаштовані або неформатовані файли конфігурації. Щоб уникнути таких проблем, рекомендовано використовувати засіб настроювання Office для створення файлу конфігурації. Ви також можете імпортувати наявні файли конфігурації в засіб настроювання Office.

3. У командному рядку в режимі адміністратора перейдіть до розташування, де Setup. exe розміщено та запустіть засіб розгортання Office у режим завантаження та вкажіть щойно збережений файл конфігурації. У цьому прикладі файл конфігурації має ім'я конфігурації. XML:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Запустіть засіб розгортання Office, у режимі настроювання та вкажіть файл конфігурації.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Примітка:** Цей крок слід запускати з клієнтського комп'ютера, на якому потрібно інсталювати Office, і потрібно мати дозволи локального адміністратора на цьому комп'ютері.

Щоб дізнатися більше про використання засобу розгортання Office для програм Microsoft 365 для сценаріїв корпоративного розгортання, перегляньте [Огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Докладніші відомості про використання засобу настроювання Office наведено в [огляді засобу настроювання Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
