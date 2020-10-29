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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801096"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="b0d35-102">Активація програми Microsoft Defender для Office 365 для SharePoint Online, OneDrive та команд Microsoft</span><span class="sxs-lookup"><span data-stu-id="b0d35-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="b0d35-103">Перейдіть на сторінку https://protection.office.com та ввійдіть.</span><span class="sxs-lookup"><span data-stu-id="b0d35-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="b0d35-104">Виберіть **Threat management** пункт  >  **Policy**  >  **безпечні вкладення** політики керування загрозою.</span><span class="sxs-lookup"><span data-stu-id="b0d35-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="b0d35-105">Виберіть **Увімкнути АТФ для SharePoint, OneDrive і команд Microsoft** , а потім натисніть кнопку **зберегти** .</span><span class="sxs-lookup"><span data-stu-id="b0d35-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="b0d35-106">Рекомендовані Як Глобальний адміністратор або адміністратор служби SharePoint Online запустіть командлет [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) за допомогою параметра **DisallowInfectedFileDownload** (значення *True* ).</span><span class="sxs-lookup"><span data-stu-id="b0d35-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="b0d35-107">Рекомендовані [Настроювання оповіщень](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) для виявлених файлів.</span><span class="sxs-lookup"><span data-stu-id="b0d35-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="b0d35-108">АТФ буде nЩоб сканувати кожен файл у службі SharePoint Online, OneDrive або Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b0d35-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="b0d35-109">Файли, відскановані в асинхронному режимі, за допомогою процесу, який використовує події спільного доступу та дії гостей, а також розумні евристики та сигнали загроз для ідентифікації зловмисних файлів.</span><span class="sxs-lookup"><span data-stu-id="b0d35-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="b0d35-110">Переглянути [АТФ для SharePoint, OneDrive і команд Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="b0d35-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>