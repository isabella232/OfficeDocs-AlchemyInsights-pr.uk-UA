---
title: Увімкнення АТФ для Office 365 для SharePoint, OneDrive і Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506939"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3abff-102">Увімкнути розширений захист від загроз Office 365 для SharePoint Online, OneDrive і Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="3abff-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="3abff-103">Перейдіть до https://protection.office.com входу та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="3abff-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="3abff-104">Виберіть **Threat management**  >  **Policy**  >  **безпечне вкладення**політики керування загрозами.</span><span class="sxs-lookup"><span data-stu-id="3abff-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="3abff-105">Виберіть **Увімкнути АТФ для SharePoint, OneDrive і Microsoft teams**і натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="3abff-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="3abff-106">Рекомендується Як Глобальний адміністратор або адміністратор SharePoint Online, запустити командлет [Set-Споживнент](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) з параметром **DisallowInfectedFileDownload** , встановлений на *True*.</span><span class="sxs-lookup"><span data-stu-id="3abff-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="3abff-107">Рекомендується [Налаштуйте оповіщення](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.</span><span class="sxs-lookup"><span data-stu-id="3abff-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="3abff-108">АТФ буде НТО сканувати кожен файл у SharePoint Online, OneDrive або Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="3abff-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="3abff-109">Файли скануються асинхронно через процес, який використовує події спільного використання та гостьової активності, а також смарт-евристики та сигнали загрози для ідентифікації шкідливих файлів.</span><span class="sxs-lookup"><span data-stu-id="3abff-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="3abff-110">Дивіться [АТФ для SharePoint, OneDrive і Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3abff-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>