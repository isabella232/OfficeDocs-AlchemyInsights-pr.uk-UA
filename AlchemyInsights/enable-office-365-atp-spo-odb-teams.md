---
title: Увімкнути АТФ Office 365 для SharePoint, OneDrive і Microsoft команд
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031134"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4be35-102">Увімкнути Office 365 передові загроза захист для SharePoint онлайн, OneDrive і Microsoft команд</span><span class="sxs-lookup"><span data-stu-id="4be35-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="4be35-103">Перейти до https://protection.office.com та виконайте вхід.</span><span class="sxs-lookup"><span data-stu-id="4be35-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="4be35-104">Вибрати **загрозу управління** > **політика** > **Безпечний вкладення**.</span><span class="sxs-lookup"><span data-stu-id="4be35-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="4be35-105">Виберіть **Увімкнути АТФ для SharePoint, OneDrive та команди Microsoft**і натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="4be35-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="4be35-106">(Рекомендовано) Як глобальна адміністратора або адміністратор SharePoint Online запустити командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) із параметром **DisallowInfectedFileDownload** , встановіть значення *true*.</span><span class="sxs-lookup"><span data-stu-id="4be35-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="4be35-107">(Рекомендовано) [Настроювання оповіщень](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) на виявлені файли.</span><span class="sxs-lookup"><span data-stu-id="4be35-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="4be35-108">АТФ буде НТО сканування кожен окремий файл у SharePoint Online, OneDrive або Microsoft команд.</span><span class="sxs-lookup"><span data-stu-id="4be35-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="4be35-109">Перевіряються при асинхронно, через процес, який використовує обміну і гостьова події діяльності, поряд з smart евристики і загроза сигнали для ідентифікації шкідливі файли.</span><span class="sxs-lookup"><span data-stu-id="4be35-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="4be35-110">Див [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="4be35-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>