---
title: Помилка входу в OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982550"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="460ee-102">Помилка входу в OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="460ee-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="460ee-103">Якщо з'являється повідомлення про помилку "AADSTS50011: URL-адреса, вказана в запиті, не збігається з відповіддю" під час входу в програму OneDrive, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="460ee-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="460ee-104">Ваша версія OneDrive має бути дорівнює або новішої версії 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="460ee-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="460ee-105">Щоб перевірити свою версію, клацніть синю піктограму OneDrive в області сповіщень, виберіть посилання **довідка & настройки > настройки > про програму**.</span><span class="sxs-lookup"><span data-stu-id="460ee-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="460ee-106">Ваша мережа може блокувати трафік на **g.Live.com** і **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="460ee-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="460ee-107">Якщо цей трафік заблоковано, його не можна оновити.</span><span class="sxs-lookup"><span data-stu-id="460ee-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="460ee-108">Працюйте з адміністратором мережі, щоб забезпечити доступ до цих URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="460ee-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="460ee-109">[Ці кінцеві точки](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) мають бути доступні для клієнтів за допомогою планів Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="460ee-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="460ee-110">Якщо вам потрібно вручну отримати поточну версію OneDrive, перейдіть на веб-сайті [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="460ee-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
