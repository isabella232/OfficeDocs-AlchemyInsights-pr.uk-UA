---
title: Видалення кореневого сайту SharePoint
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
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815492"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="eaeac-102">Видалення кореневого сайту SharePoint</span><span class="sxs-lookup"><span data-stu-id="eaeac-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="eaeac-103">Видалення кореневого сайту SharePoint  **не підтримується.**</span><span class="sxs-lookup"><span data-stu-id="eaeac-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="eaeac-104">Якщо кореневий сайт уже видалено, під час спроби отримати доступ до сайту з'являється помилка 404 File Not Found (Не знайдено файлу 404).</span><span class="sxs-lookup"><span data-stu-id="eaeac-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="eaeac-105">Щоб вирішити цю проблему, відновіть сайт із [](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) нового Центру адміністрування SharePoint на сторінці Видалені сайти, виберіть кореневий сайт і натисніть кнопку Відновити.</span><span class="sxs-lookup"><span data-stu-id="eaeac-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="eaeac-106">Замість того, щоб видаляти кореневий сайт, використовуйте заміну сайту з нового Центру адміністрування SharePoint після відновлення кореневого сайту. [](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)</span><span class="sxs-lookup"><span data-stu-id="eaeac-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="eaeac-107">Докладні відомості див. в [розділах Модернізування кореневого сайту.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="eaeac-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>