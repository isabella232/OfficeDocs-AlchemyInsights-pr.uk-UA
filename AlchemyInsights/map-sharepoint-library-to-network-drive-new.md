---
title: Підключення бібліотеки SharePoint з мережевим диском
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
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 4eae45992d3fe6b31ae4d1aed02484cf20cb2260
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315569"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Підключення бібліотеки SharePoint з мережевим диском

Замість підключення мережевого диска синхронізуйте файли SharePoint з новим клієнтом синхронізатор OneDrive, який надає доступ до файлів без вимоги. Отримуйте доступ до всіх файлів у OneDrive, не використовуючи локальний простір для зберігання. Докладні відомості див. в [розділах Синхронізація файлів SharePoint Teams](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) комп'ютера та Заощадження дискового простору за [допомогою OneDrive](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)"Доступ до файлів Windows 10".

Якщо ви вирішили зіставити диск, а не новий [клієнт синхронізатор OneDrive,](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)обов'язково виконайте такі дії:

- [Усунення несправностей підключених мережевих дисків, підключених SharePoint Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Помилки автентифікації, коли клієнт не підтримує протокол TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**ПРИМІТКА.** Якщо ви використовуєте Internet Explorer 10 зі Windows 8 або Windows 7 і вам  не вдається  отримати доступ або Шлях недоступний під час зіставлення диска, усуньте цю проблему, інсталювши це [виправлення.](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)