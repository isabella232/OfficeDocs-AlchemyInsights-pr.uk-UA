---
title: 932 оновлення AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806060"
---
# <a name="upgrade-azure-ad-connect"></a>Оновлення "Azure AD Connect"

За замовчуванням автоматичне оновлення ввімкнуто для Azure AD Connect, що допомагає забезпечити роботу найновішої версії. Щоб перевірити параметри автоматичного оновлення, скористайтеся командлетом **Get-ADSyncAutoUpgrade** в ЛАЗУРКОМУ AD PowerShell. Командлет поверне одне з наведених нижче значень.

- **Увімкнуто**: функція автоматичного оновлення ввімкнена.

- **Вимкнуто**: автоматичне оновлення вимкнуто.

- **Призупинено**: система більше не має права на отримання автоматичних оновлень. Не можна настроїти це значення; це встановлено системою.

Докладні відомості наведено в статті [Автоматичне оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Щоб завантажити найновішу версію служби Azure AD Connect, перейдіть на сторінку [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
