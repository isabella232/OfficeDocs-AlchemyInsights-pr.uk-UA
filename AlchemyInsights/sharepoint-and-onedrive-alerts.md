---
title: Затримки в отриманні сповіщень SharePoint і OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785686"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="aa3f2-102">Затримки в отриманні сповіщень SharePoint і OneDrive</span><span class="sxs-lookup"><span data-stu-id="aa3f2-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="aa3f2-103">Спочатку перевірте папку "Небажана пошта" або "спам" у повідомленні електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="aa3f2-104">Якщо **всі оповіщення з кількох файлів або бібліотек затримуються**, перейдіть на [приладну дошку справність служби](https://portal.office.com/adminportal/home?ref=/servicehealth) , щоб перевірити наявність будь-яких інших або інцидентів, які можуть виникнути в службі SharePoint або Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="aa3f2-105">Ця проблема може бути з функцією оповіщення служби SharePoint або затримками в повідомленнях електронної пошти за допомогою Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="aa3f2-106">Зверніть увагу, чи доставлятимуться інші повідомлення електронної пошти (якщо ні, то проблема може бути затримка Exchange).</span><span class="sxs-lookup"><span data-stu-id="aa3f2-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="aa3f2-107">Якщо **окреме оповіщення з певного файлу або бібліотеки не доставлено**, спробуйте видалити та відтворити його повторно.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="aa3f2-108">У статті [керування, перегляд і видалення оповіщень SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) для повторного створення оповіщення.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="aa3f2-109">Оповіщення не можна надіслати до групи розсилки.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="aa3f2-110">Підтримуються лише групи безпеки та O365.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="aa3f2-111">Ви не можете настроювати шаблони сповіщень електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="aa3f2-112">Щоб досягти цих документів, потрібно скористатися робочим циклом Microsoft Flow або конструктора SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="aa3f2-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
