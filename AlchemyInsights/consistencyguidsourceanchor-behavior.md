---
title: ConsistencyGuid / sourceAnchor поведінка
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927704"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor поведінка

Блакитні оголошення підключення (версії 1.1.524.0 і після) тепер полегшує використання msDS-ConsistencyGuid як атрибут sourceAnchor. При використанні цієї функції, Azure оголошення підключитися автоматично настроює правил синхронізації, щоб:
  
- Для користувача об'єкти за допомогою msDS-ConsistencyGuid як атрибут sourceAnchor. ObjectGUID використовується для інших типів об'єктів.
    
- Для будь-якого з огляду на локальному Оголошень користувача назад об'єкт, чиї msDS-ConsistencyGuid атрибут не заселені, Azure оголошення підключення пише його objectGUID значення для msDS-ConsistencyGuid атрибут у локальній службі Active Directory. Після того, як населені атрибут msDS-ConsistencyGuid, Azure оголошення підключення експортує об'єкт в блакитні оголошення.
    
 **Примітка:** Одного разу локальні оголошення об'єкт буде імпортовано до Azure оголошення підключення (тобто, імпортовані в Рекламний простір з'єднувача та прогнозовані в метавселенной), не можна змінити його sourceAnchor значення більше. Вкажіть значення sourceAnchor для з огляду на локальному оголошення об'єкт, налаштувати його атрибут msDS-ConsistencyGuid, перш ніж вона буде імпортовано до Azure оголошення підключитися. 
  
Більш докладну інформацію про SourceAnchor та ConsistencyGuid, Докладніше: [Azure оголошення підключитися: дизайн концепції](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

