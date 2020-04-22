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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703447"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ef78e-102">Увімкнути розширений захист від загроз Office 365 для SharePoint Online, OneDrive і Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="ef78e-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ef78e-103">Перейдіть до https://protection.office.com входу та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="ef78e-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ef78e-104">Виберіть**безпечне вкладення** > **політики** >  **керування загрозами**.</span><span class="sxs-lookup"><span data-stu-id="ef78e-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="ef78e-105">Виберіть **Увімкнути АТФ для SharePoint, OneDrive і Microsoft teams**і натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="ef78e-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="ef78e-106">Рекомендується Як Глобальний адміністратор або адміністратор SharePoint Online, запустити командлет [Set-Споживнент](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) з параметром **DisallowInfectedFileDownload** , встановлений на *True*.</span><span class="sxs-lookup"><span data-stu-id="ef78e-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="ef78e-107">Рекомендується [Налаштуйте оповіщення](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.</span><span class="sxs-lookup"><span data-stu-id="ef78e-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ef78e-108">АТФ буде НТО сканувати кожен файл у SharePoint Online, OneDrive або Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="ef78e-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ef78e-109">Файли скануються асинхронно через процес, який використовує події спільного використання та гостьової активності, а також смарт-евристики та сигнали загрози для ідентифікації шкідливих файлів.</span><span class="sxs-lookup"><span data-stu-id="ef78e-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ef78e-110">Бачити [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ef78e-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>