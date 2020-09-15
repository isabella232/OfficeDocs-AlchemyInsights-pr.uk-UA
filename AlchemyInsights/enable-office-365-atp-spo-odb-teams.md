---
title: Увімкнення АТФ Office 365 для SharePoint, OneDrive та команд Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709928"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="176fb-102">Увімкнення захисту від розширених загроз в Office 365 для служби SharePoint Online, OneDrive і команд Microsoft</span><span class="sxs-lookup"><span data-stu-id="176fb-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="176fb-103">Перейдіть на сторінку https://protection.office.com та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="176fb-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="176fb-104">Виберіть **Threat management**пункт  >  **Policy**  >  **безпечні вкладення**політики керування загрозою.</span><span class="sxs-lookup"><span data-stu-id="176fb-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="176fb-105">Виберіть **Увімкнути АТФ для SharePoint, OneDrive і команд Microsoft**, а потім натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="176fb-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="176fb-106">Рекомендовані Як Глобальний адміністратор або адміністратор служби SharePoint Online запустіть командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) за допомогою параметра **DisallowInfectedFileDownload** (значення *True*).</span><span class="sxs-lookup"><span data-stu-id="176fb-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="176fb-107">Рекомендовані [Настроювання оповіщень](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.</span><span class="sxs-lookup"><span data-stu-id="176fb-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="176fb-108">АТФ буде nЩоб сканувати кожен файл у службі SharePoint Online, OneDrive або Microsoft.</span><span class="sxs-lookup"><span data-stu-id="176fb-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="176fb-109">Файли, відскановані в асинхронному режимі, за допомогою процесу, який використовує події спільного доступу та дії гостей, а також розумні евристики та сигнали загроз для ідентифікації зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="176fb-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="176fb-110">Переглянути [АТФ для SharePoint, OneDrive і команд Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="176fb-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>