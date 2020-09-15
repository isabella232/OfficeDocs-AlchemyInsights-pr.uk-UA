---
title: Початок роботи зі службою SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700728"
---
# <a name="workflows-in-sharepoint"></a>Робочі цикли в SharePoint

Якщо робочі цикли SharePoint не надсилають повідомлення електронної пошти, можливо, ваша організація виявила обмеження відправника в службі Exchange Online.

Повідомлення про помилку "робочий цикл призупинено" може виникати, якщо у вас є один із таких способів:

- Ви маєте робочий цикл у службі SharePoint Online, який використовує тип платформи робочого циклу SharePoint 2010 або SharePoint 2013.

- Робочий цикл настроєно для надсилання настроюваного повідомлення електронної пошти для більш ніж 200 користувачів за один раз, понад 10 000 одержувачів на день або понад 30 повідомлень за хвилину.

Під час запуску робочого циклу повідомлення електронної пошти не надсилається, і ви помітите повідомлення про помилку, внутрішній стан має значення призупинено або не вдається надіслати одержувачу.

Щоб отримати докладніші відомості, ознайомтеся з наведеними нижче [статтею](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

