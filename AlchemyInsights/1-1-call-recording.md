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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886160"
---
# <a name="11-call-recording"></a>Запис викликів: 1:1

Якщо кнопка **Почати записування** неясна під час виклику о 1:1, потрібно змінити параметри політики для потрібного користувача. Щоб перевірити параметр політики, запустіть запис діагностики для цього користувача, ввівши вище **параметр Diag: Teams 1:1 Call Recording** (Діагностичний).     

З 31 травня 202 Teams 1 року ми почнемо застосовувати нову політику викликів *AllowCloudRecordingForCalls*. До цієї зміни записування викликів о 1:1 контролюється політикою *нарад AllowCloudRecording* Teams нарад. Ця зміна документується в дописі в Центрі повідомлень: [(Оновлено) 1:1 Вступ до політики записування викликів.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   Параметр "Політика викликів" установлено **$False** за замовчуванням. Щоб заборонити всім користувачам записувати одновиклик, не потрібно нічого робити.  

Щоб увімкнути записування викликів для всіх користувачів в цілодобовому оболонці [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) виконайте такий командлет: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Крім того, ви можете створити політику та вибрати **параметр -AllowCloudRecordingForCalls** $true призначити цю політику користувачам.  

Докладні відомості див. в дописі 1:1 Елементи керування політикою записування [викликів (майже!) Тут](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
