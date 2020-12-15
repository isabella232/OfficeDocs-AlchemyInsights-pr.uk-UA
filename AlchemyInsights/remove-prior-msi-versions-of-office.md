---
title: Видалення попередньої версії пакета Office MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680780"
---
# <a name="remove-prior-msi-versions-of-office"></a>Видалення попередньої версії пакета Office MSI

Перш ніж інсталювати пакет Office 365 ProPlus, я рекомендую видалити попередні версії пакета Office Installer (MSI). Ось як це зробити:

1. Якщо ви використовували MSI для інсталяції пакета Office, можна видалити пакет Office за допомогою засобу розгортання Office (ODT). Ви можете використовувати елемент RemoveMSI у файлі **configuration.xml** .
1. Виконайте вказівки в цій статті: [центр відповідності системи безпеки Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)