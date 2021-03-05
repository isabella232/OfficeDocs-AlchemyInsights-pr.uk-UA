---
title: Проблема зі здоров'ям AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483124"
---
# <a name="problem-with-aad-connect-health"></a>Проблема зі здоров'ям AAD Connect

- Переконайтеся, що ви маєте право виконати операцію. Глобальні адміністратори мають доступ за замовчуванням. Крім того, можна використовувати [елемент керування доступом на основі ролей](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , щоб отримати дозвіл на реєстрацію представника.
- Переконайтеся, що потрібні кінцеві точки ввімкнуто, а не заблоковано через брандмауер. Докладні відомості наведено в статті [вимоги](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Реєстрація може не відповідно до вихідних повідомлень, які піддаються перевірці SSL через мережевий рівень.
- Переконайтеся, що ви підтвердили параметри сповіщень для справності для Azure AD Connect. Ознайомтеся з вашим параметром. Цей [посібник](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) допоможе вам дізнатися, як настроїти параметри сповіщень для сповіщень про справність служби AZURE AD Connect.
- Щоб дізнатися більше про звіт про синхронізацію служби AAD Connect, а також про те, як завантажити його, перегляньте статтю [звіт про синхронізацію на рівні об'єкта](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Щоб виправити неполадки з оповіщеннями в службі AAD Connect для справності, виконайте вказівки [з виправлення неполадок для сповіщень про стан справності та відповіді](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) на поширені запитання в розділі [Загальні запитання про інсталяцію СПРАВНОСТІ служби aad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
