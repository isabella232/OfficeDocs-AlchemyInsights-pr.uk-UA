---
title: Помилка AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916545"
---
# <a name="error-attributevaluemustbeunique"></a>Помилка: AttributeValueMustBeUnique

Найпоширеніша причина AttributeValueMustBeUnique помилка в два об'єкти з різними SourceAnchor (immutableId) мають однакове значення для атрибутів ProxyAddresses та/або UserPrincipalName. Виправити помилки AttributeValueMustBeUnique:
  
1. Визначити дубльованого proxyAddresses, userPrincipalName або інші значення атрибута, яке викликає появу помилки. Також визначити, які об'єкти два (або більше) беруть участь в конфлікті. У доповіді породжених Azure оголошення підключення здоров'я для синхронізації може допомогти визначити два об'єкти.
    
2. Визначити, які об'єкти повинні продовжувати, які дублюються виконання і які об'єкти.
    
3. Видаліть дубльовані значення з об'єкта, який не може мати значення. Зверніть увагу, що ви повинні зробити зміни в каталог, де об'єкт був здобутий з. У деяких випадках може знадобитися видалити один з об'єктів в конфлікті.
    
4. Після внесення змін в приміщенні на оголошення, дайте Azure оголошення підключення синхронізувати зміни помилок отримати фіксовані.
    

