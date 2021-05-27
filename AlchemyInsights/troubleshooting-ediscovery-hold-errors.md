---
title: Виправлення помилок служби ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676531"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Виправлення помилок служби ediscovery

Виникли проблеми з утриманням витребування електронної даних? Нижче наведено кілька порад, які слід врахувати.

- Перевірте стан розподілу утримання.  Якщо стан **Увімкнуто (очікує)** або Вимк. **(Очікує),** зачекайте, доки не завершиться розподіл утримання.
- Об'єднайте оновлення для витребування електронної інформації, щоб проводити оновлення в один груповий запит, а не постійно оновлювати політику для кожної транзакції.
- Запустіть Set-CaseHoldPolicy <policyname> -RetryDistribution в PowerShell Центру безпеки та відповідності. Докладні відомості [див. в Підключення PowerShell & безпеки та відповідності.](/powershell/exchange/connect-to-scc-powershell)

Указівки з перевірки цих параметрів і додаткові практичні поради з виправлення неполадок утримання витребування електронної пошти див. в цій [статті.](/microsoft-365/compliance/hold-distribution-errors)
Відомості про виправлення інших поширених проблем витребування електронної інформації див. в розділах Дослідження, усунення несправностей і вирішення поширених проблем витребування [електронної інформації.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
