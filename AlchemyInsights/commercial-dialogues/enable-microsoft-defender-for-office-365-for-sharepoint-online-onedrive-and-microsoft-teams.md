---
title: Активація програми Microsoft Defender для Office 365 для SharePoint Online, OneDrive та команд Microsoft
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747736"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1c586-102">Активація програми Microsoft Defender для Office 365 для SharePoint Online, OneDrive та команд Microsoft</span><span class="sxs-lookup"><span data-stu-id="1c586-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="1c586-103">За допомогою облікових даних глобального адміністратора або адміністратора безпеки Увійдіть у [Центр безпеки та відповідності Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1c586-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="1c586-104">Виберіть елемент **керування загрозою** в області ліворуч, а потім виберіть пункт   >  [надійні вкладення](https://protection.office.com/safeattachment)політики.</span><span class="sxs-lookup"><span data-stu-id="1c586-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="1c586-105">Виберіть **Увімкнути Microsoft Defender для Office 365 для SharePoint, OneDrive і команд Microsoft**, а потім натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="1c586-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="1c586-106">Як Глобальний адміністратор або адміністратор служби SharePoint Online запустіть наведений нижче командлет PowerShell із параметром **DisallowInfectedFileDownload** (значення *True*): [Set-spotenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="1c586-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="1c586-107">Настроювання оповіщень для виявлених файлів</span><span class="sxs-lookup"><span data-stu-id="1c586-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="1c586-108">Щоб отримати докладніші відомості, ознайомтеся з [програмою Microsoft Defender для Office 365 для SharePoint, OneDrive та командами Microsoft](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="1c586-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
