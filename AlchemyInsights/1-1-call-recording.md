---
title: 'Запис викликів: 1:1'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314405"
---
# <a name="11-call-recording"></a>Запис викликів: 1:1

Якщо кнопка **Почати записування** неясна під час виклику о 1:1, потрібно змінити параметри політики для потрібного користувача. Щоб перевірити параметр політики, запустіть діагностичну для цього користувача, ввівши вище **параметр Diag: Teams 1:1 Call Recording** (Діагностичний).     

З 31 травня 2021 року ми почнемо застосовувати нову політику викликів Teams *AllowCloudRecordingForCalls.* До цієї зміни записування викликів о 1:1 контролюється політикою *нарад AllowCloudRecording* Teams нарад. Ця зміна документується в дописі в Центрі повідомлень: [(Оновлено) 1:1 Вступ до політики записування викликів.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   Параметр "Політика викликів" установлено **$False** за замовчуванням. Щоб заборонити всім користувачам записувати одновиклик, не потрібно нічого робити.  

Щоб увімкнути записування викликів для всіх користувачів в цілодобовому оболонці, виконайте цей командлет Teams [PowerShell:](https://docs.microsoft.com/microsoftteams/teams-powershell-install) 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Крім того, ви можете створити політику та вибрати **параметр -AllowCloudRecordingForCalls** $true призначити цю політику користувачам.  

Докладні відомості див. в дописі 1:1 Елементи керування політикою записування [викликів (майже!) Тут](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
