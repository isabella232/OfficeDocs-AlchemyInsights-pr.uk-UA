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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002147"
---
# <a name="error-attributevaluemustbeunique"></a>Помилка: AttributeValueMustBeUnique

Найпоширеніша причина помилки AttributeValueMustBeUnique – це два об'єкти з різними атрибутами SourceAnchor (immutableId) і ProxyAddresses і/або UserPrincipalName. Виправлення помилки AttributeValueMustBeUnique:
  
1. Визначте повторюване значення proxyAddresses, userPrincipalName або інше значення атрибута, що виникає через помилку. Також визначте, до яких трьох (або більше) об'єктів залучено конфлікт. Звіт, створений в Azure AD Підключення Health для синхронізації, може допомогти визначити два об'єкти.
    
2. Визначте, який об'єкт має і надалі мати повторюване значення, а який об'єкт не має бути.
    
3. Видаліть значення, що повторюється, з об'єкта, який не має містити це значення. Зверніть увагу, що потрібно внести зміни в каталозі, з якого об'єкт джерелом. У деяких випадках може знадобитися видалити один з об'єктів, які конфліктують.
    
4. Якщо ви вніс зміни в локальній службі AD, Підключення azure AD синхронізувати зміни, щоб виправити помилку.
    

