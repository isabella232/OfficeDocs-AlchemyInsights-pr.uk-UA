---
title: Атрибут помилкиValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813781"
---
# <a name="error-attributevaluemustbeunique"></a>Помилка: AttributeValueMustBeUnique

Найпоширеніша причина помилки AttributeValueMustBeUnique – це два об'єкти з різними атрибутами SourceAnchor (immutableId) і ProxyAddresses і/або UserPrincipalName. Виправлення помилки AttributeValueMustBeUnique:
  
1. Визначте повторюване значення proxyAddresses, userPrincipalName або інше значення атрибута, що виникає через помилку. Також визначте, до яких трьох (або більше) об'єктів залучено конфлікт. Звіт, створений службою Azure AD Connect Health для синхронізації, може допомогти визначити два об'єкти.
    
2. Визначте, який об'єкт має і надалі мати повторюване значення, а який об'єкт не має бути.
    
3. Видаліть значення, що повторюється, з об'єкта, який не має містити це значення. Зверніть увагу, що потрібно внести зміни в каталозі, з якого об'єкт джерелом. У деяких випадках може знадобитися видалити один з об'єктів, які конфліктують.
    
4. Якщо ви вніс зміни в локальній службі AD, запустіть засіб Azure AD Connect, щоб виправити цю помилку.
    

