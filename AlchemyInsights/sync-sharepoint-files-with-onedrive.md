---
title: Синхронізація файлів SharePoint за допомогою нового клієнта синхронізації OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757840"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="5b6e0-102">Синхронізація файлів SharePoint за допомогою нового клієнта синхронізації OneDrive</span><span class="sxs-lookup"><span data-stu-id="5b6e0-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="5b6e0-103">Команда «Відкрити у провіднику» відкриває локальний екземпляр провідника Windows, який відображає структуру папок на сервері, де розміщено сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="5b6e0-104">Тому, ми радимо [синхронізувати файли SharePoint за допомогою нового клієнта синхронізації OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, який надає доступ до [файлів на вимогу](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), оскільки він також надає локальний доступ до файлів і більшу продуктивність.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="5b6e0-105">Якщо ж ви вирішили використовувати подання провідника, а не новий клієнт синхронізації, скористайтеся інструкціями та практичними порадами, наведеними в статтях нижче.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="5b6e0-106">Виправлення неполадок у службі SharePoint Online за допомогою команди «Відкрити у провіднику»</span><span class="sxs-lookup"><span data-stu-id="5b6e0-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="5b6e0-107">Копіювання та переміщення файлів бібліотеки за допомогою команди «Відкрити у провіднику»</span><span class="sxs-lookup"><span data-stu-id="5b6e0-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="5b6e0-108">Примітка. Кнопка «Відкрити у провіднику» не відображається в новому поданні бібліотеки.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="5b6e0-109">Клацніть розкривний список «Вигляд» вгорі справа (назва розкривного списку залежить від поточного подання), а потім натисніть «Вигляд» у Файловому провіднику.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="5b6e0-110">Команда SharePoint «Відкрити у провіднику» використовує елементи керування ActiveX, тому її підтримують лише в Internet Explorer 10 або 11.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="5b6e0-111">Команда «Відкрити у провіднику» не працює в ОС Windows з Microsoft Edge, Google Chrome, Mozilla Firefox або на платформі Mac.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="5b6e0-112">Через це, параметр подання Провідника може бути неактивним.</span><span class="sxs-lookup"><span data-stu-id="5b6e0-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="5b6e0-113">[Причини, з яких кнопки на стрічці SharePoint недоступні або неактивні](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="5b6e0-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

