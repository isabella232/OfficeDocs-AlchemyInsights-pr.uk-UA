---
title: Використання засобу Office розгортання
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083791"
---
# <a name="using-the-office-deployment-tool-odt"></a>Використання засобу Office розгортання (ODT)

Засіб розгортання Office (ODT) використовується для Office 365 версій Office. Засіб Office розгортання (setup.exe) запускається з командного рядка та використовує XML-файл конфігурації, щоб визначити параметри, які потрібно застосувати під час розгортання Office.
  
1. Завантажте найновішу версію засобу Office розгортання з [Центру завантажень Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Скористайтеся [засобом Office настроювання (OCT),](https://config.office.com) щоб вибрати параметри розгортання та створити XML-файл конфігурації. Експортуйте файл конфігурації та розмістіть його локально в тій самій папці, де setup.exe файл.

    **Примітка.** Office проблеми інсталяції зазвичай виникають через неправильно настроєні або неправильно відформатовані файли конфігурації. Щоб уникнути таких проблем, радимо створити файл конфігурації Office засобу настроювання. Ви також можете імпортувати наявні файли конфігурації до засобу Office настроювання.

3. У командному рядку в режимі адміністратора перейдіть до розташування, де setup.exe, запустіть засіб розгортання Office у режимі завантаження та вкажіть щойно збережений файл конфігурації. У цьому прикладі файл конфігурації має ім'я Configuration.xml:

```setup.exe /download Configuration.xml```

4.Запустіть засіб Office розгортання в режимі настроювання та вкажіть файл конфігурації.

```setup.exe /configure Configuration.xml```

**Примітка.** Цей крок потрібно виконати з клієнтського комп'ютера, на якому потрібно інсталювати програму Office і ви повинні мати дозволи локального адміністратора на цьому комп'ютері.

Докладні відомості про використання засобу Office розгортання для Програми Microsoft 365 для підприємств сценаріїв розгортання див. в цій [Office.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Докладні відомості про використання засобу Office настроювання див. в статті Огляд засобу [Office настроювання.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
