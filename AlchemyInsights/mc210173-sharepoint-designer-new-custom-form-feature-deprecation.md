---
title: MC210173. Скасування нової функції спеціальних форм у SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831827"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="fa0f3-102">MC210173. Скасування нової функції спеціальних форм у SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="fa0f3-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="fa0f3-103">Ми визначили проблему, яка впливає на [створення спеціальних форм](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) у SharePoint Online за допомогою SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="fa0f3-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="fa0f3-104">Після ретельного аналізу ми визначили, що неможливо усунути цю проблему, і вирішили вимкнути функцію створення спеціальних форм у суботу, 25 квітня 2020 р., о 15:00 за Гринвічем (UTC).</span><span class="sxs-lookup"><span data-stu-id="fa0f3-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="fa0f3-105">Ця зміна не впливає на можливість редагувати попередньо створені форми або на інші наявні функції в SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="fa0f3-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="fa0f3-106">Після цієї зміни користувачі могли отримувати помилку, що не вдається зберегти зміни на сервері під час створення форми.</span><span class="sxs-lookup"><span data-stu-id="fa0f3-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="fa0f3-107">Користувачі, які раніше створювали спеціальні форми в SharePoint Designer, тепер можуть робити це в [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="fa0f3-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="fa0f3-108">PowerApps – це простий і потужний засіб, який дає змогу користувачам використовувати сучасний інтерфейс SharePoint Online, щоб створювати й редагувати спеціальні форми для списків SharePoint і бібліотек документів безпосередньо у вікні браузера.</span><span class="sxs-lookup"><span data-stu-id="fa0f3-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="fa0f3-109">Для роботи в PowerApps не потрібно мати жодних навичок програмування та завантажувати додаткові програми, як-от InfoPath.</span><span class="sxs-lookup"><span data-stu-id="fa0f3-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="fa0f3-110">**Примітка.** Користувачам класичної версії SharePoint Online потрібно тимчасово використовувати сучасний інтерфейс, щоб отримати доступ до PowerApps і працювати в цій програмі. Усі спеціальні форми, створені в PowerApps, доступні для користувачів із класичною версією інтерфейсу SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fa0f3-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
