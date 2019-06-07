---
title: Пересунути повідомлення електронної пошти до поштової скриньки архіву
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762386"
---
# <a name="move-email-to-the-archive-mailbox"></a>Переміщення електронної пошти до поштової скриньки архіву
 
1. Переконайтеся, що **архівувати поштової скриньки** ввімкнено. Якщо ні, скориставшись вказівками в [цій статті](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) увімкнення поштової скриньки архіву.

2. Щоб заархівувати повідомлення автоматично до поштової скриньки архіву, тег збереження з **перемістити до архіву** дії слід установити **застосовуються автоматично до всієї поштової скриньки (за замовчуванням) тег**. Виконайте дії тут, щоб створити тег: [Тег архіву за промовчанням](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Далі, додати **Архів** тегів політики збереження. У центру адміністрування Exchange виберіть **Політики збереження** > доповнити **перемістити до архіву тег** політики > **зберегти**. 
    
4. Тепер [призначити політику збереження](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) конкретного користувача поштової скриньки. Ту ж політику буде застосовано до **первинної** і поштової скриньки **архіву** . 
    
Можливо, буде необхідно для примусового Керовані папки помічник (МЗС) для запуску і застосувати нові параметри для поштової скриньки користувача. Запустіть таку команду під час [підключення до EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , щоб запустити помічник із керованих папок для певної поштової скриньки: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Щоб отримати додаткові відомості про налаштування політику архівування переглянути [набір до архіву і видалення політики поштових скриньок](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

