---
title: Використання засобу розгортання Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794932"
---
# <a name="using-the-office-deployment-tool-odt"></a>Використання засобу розгортання Office (ODT)

Ви використовуєте засіб розгортання Office (ODT), щоб розгорнути версії Office 365. Засіб розгортання Office (setup.exe) запускається з командного рядка та використовує XML-файл конфігурації, щоб визначити, які настройки слід застосувати під час розгортання Office.
  
1. Завантажте найновішу версію засобу розгортання Office в [центрі завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Скористайтеся [засобом настроювання Office (жовтень)](https://config.office.com) , щоб вибрати параметри розгортання та створити XML-файл конфігурації. Експортуйте файл конфігурації та розмістіть його локально в тій самій папці, де знаходиться setup.exe.

    **Примітка.** Проблеми з інсталяцією Office зазвичай виникають через неправильне настроювання або файли конфігураційних файлів. Щоб уникнути таких проблем, радимо використовувати засіб настроювання Office, щоб створити файл конфігурації. Ви також можете імпортувати доступні файли конфігурації до засобу настроювання Office.

3. У командному рядку зі підвищеними параметрами перейдіть до розташування, у якому setup.exe розташовано та запустіть засіб розгортання Office у режимі завантаження та вкажіть щойно збережений файл конфігурації. У цьому прикладі файл конфігурації має назву Configuration.xml:

```setup.exe /download Configuration.xml```

4. запустіть засіб розгортання Office у режимі настроювання та вкажіть файл конфігурації.

```setup.exe /configure Configuration.xml```

**Примітка.** Потрібно виконати цей крок із клієнтського комп'ютера, на якому потрібно інсталювати Office, і на цьому комп'ютері потрібно мати дозволи локального адміністратора.

Щоб дізнатися більше про використання засобу розгортання Office для програм Microsoft 365 для сценаріїв розгортання підприємств, ознайомтеся [зі статтею огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Докладні відомості про використання засобу настроювання Office наведено в розділі [Огляд засобу настроювання Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
