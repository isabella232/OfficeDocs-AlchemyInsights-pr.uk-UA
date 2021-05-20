---
title: Увімкнення Office 365 ЛОС для SharePoint, OneDrive та Microsoft Teams
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543949"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3d616-102">Увімкнення Microsoft Defender для Office 365 для SharePoint Online, OneDrive і Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3d616-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="3d616-103">Перейдіть до входу https://protection.office.com та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="3d616-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="3d616-104">Виберіть **Політика керування**  >    >  **загрозами Сейф вкладеннях.**</span><span class="sxs-lookup"><span data-stu-id="3d616-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="3d616-105">Установіть **прапорець Увімкнути Захисник для Office 365 для SharePoint, OneDrive і Microsoft Teams**, а потім натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="3d616-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="3d616-106">(Рекомендовано) Якщо ви глобальний адміністратор або адміністратор служби SharePoint Online, запустіть командлет [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) із для параметра **DisallowInfectedFileDownload** значення *TRUE.*</span><span class="sxs-lookup"><span data-stu-id="3d616-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="3d616-107">(Рекомендовано) [Настроювання оповіщень](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) про виявлені файли.</span><span class="sxs-lookup"><span data-stu-id="3d616-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="3d616-108">Microsoft Defender для Office 365 не скануватиме кожен окремий файл у SharePoint Online, OneDrive або Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3d616-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="3d616-109">Файли скануються асинхронно в процесі, який використовує події спільного доступу та гостьових дій, а також інтелектуальні евристичні сигнали та сигнали загроз для виявлення зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="3d616-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="3d616-110">Докладні [відомості див. в статті Office 365 Захисник Microsoft SharePoint, OneDrive і Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3d616-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>