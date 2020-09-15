---
title: Помилка Attribueоцінюем"унікальні"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709172"
---
# <a name="error-attributevaluemustbeunique"></a>Помилка: функція Attributeоціню"унікальні"

Найпоширеніша причина для атрибута Attributeempleunique – це два об'єкти з різним опорним якорем (immutableId) мають однакові значення для атрибутів ProxyAddresses та/або UserPrincipalName. Щоб вирішити цю помилку, виконайте наведені нижче дії.
  
1. Визначення дубльованих адрес, userPrincipalName або іншого значення атрибута, яке спричиняє помилку. Також визначте, які два (або більше) об'єкти беруть участь у конфлікті. У звіті, створеному для синхронізації, може допомогти визначити два об'єкти.
    
2. Визначення об'єкта, який має надалі мати дубльовне значення, а об'єкт, який не має перевищувати.
    
3. Видалення дубльованого значення з об'єкта, який не має цього значення. Зверніть увагу, що ви повинні внести зміни до каталогу, у якому буде отриманий об'єкт. У деяких випадках, можливо, знадобиться видалити один із об'єктів у конфлікті.
    
4. Якщо ви внесли зміни в локальний рекламний ролик, повідомте про помилку "Azure AD Connect", щоб почати синхронізацію.
    

