---
title: Затримки в отриманні сповіщень SharePoint і OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563531"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="e79f3-102">Затримки в отриманні сповіщень SharePoint і OneDrive</span><span class="sxs-lookup"><span data-stu-id="e79f3-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="e79f3-103">Спочатку перевірте папку небажаної або спаму в електронному листі.</span><span class="sxs-lookup"><span data-stu-id="e79f3-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="e79f3-104">Якщо **затримка всіх оповіщень із кількох файлів або бібліотек**, відвідайте [приладну дошку служби охорони здоров'я](https://portal.office.com/adminportal/home?ref=/servicehealth) , щоб перевірити наявність попереджень і інцидентів, які можуть трапитися з SharePoint або Exchange.</span><span class="sxs-lookup"><span data-stu-id="e79f3-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="e79f3-105">Ця проблема може бути у SharePoint оповіщення про можливості або затримки в електронній пошті через Exchange.</span><span class="sxs-lookup"><span data-stu-id="e79f3-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="e79f3-106">Також зверніть увагу на те, чи інша електронна пошта доставляється, якщо ні, то проблема, ймовірно, з затримками обміну.</span><span class="sxs-lookup"><span data-stu-id="e79f3-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="e79f3-107">Якщо **окреме оповіщення від певного файлу або бібліотеки не доставлено**, спробуйте видалити та відтворити його.</span><span class="sxs-lookup"><span data-stu-id="e79f3-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="e79f3-108">Перегляньте [сповіщення про керування, перегляд або видалення SharePoint оповіщення](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) для відтворення оповіщення.</span><span class="sxs-lookup"><span data-stu-id="e79f3-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="e79f3-109">Оповіщення не надсилатимуться до групи розсилки.</span><span class="sxs-lookup"><span data-stu-id="e79f3-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="e79f3-110">Підтримуються лише групи безпеки та O365.</span><span class="sxs-lookup"><span data-stu-id="e79f3-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="e79f3-111">Не вдається настроїти оповіщення електронної пошти шаблони.</span><span class="sxs-lookup"><span data-stu-id="e79f3-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="e79f3-112">Щоб досягти цих, слід використовувати Microsoft Flow або Конструктор конструктора SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e79f3-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
