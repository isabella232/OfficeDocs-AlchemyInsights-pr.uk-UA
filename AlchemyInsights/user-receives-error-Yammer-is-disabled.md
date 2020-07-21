---
title: Користувач отримує, помилка AADSTS7000112 Yammer вимкнуто
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198367"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="f626d-102">Користувач отримує, помилка AADSTS7000112 Yammer вимкнуто</span><span class="sxs-lookup"><span data-stu-id="f626d-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="f626d-103">Якщо з'являється повідомлення про помилку "AADSTS7000112: застосунок" 00000005-0000-0ff1-ce00-000000000000 "(Yammer) вимкнуто", виникає проблема з принципалом служби в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f626d-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="f626d-104">Можливо, адміністратор вимкнув принципал служби для блокування доступу до Yammer.</span><span class="sxs-lookup"><span data-stu-id="f626d-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="f626d-105">Вимкнення основної служби не рекомендується і може спричинити додаткові проблеми.</span><span class="sxs-lookup"><span data-stu-id="f626d-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="f626d-106">Для отримання додаткових відомостей про підтримуваний підхід до блокування доступу користувачів до Yammer зверніться [до служби підтримки Yammer для користувачів Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="f626d-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="f626d-107">Щоб вирішити цю проблему, на порталі Azure і відновлення доступу користувачів до Yammer:</span><span class="sxs-lookup"><span data-stu-id="f626d-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="f626d-108">Відкрийте сторінку Azure Active Directory і виберіть **корпоративні програми** в області **керування** в лівій навігаційній панелі.</span><span class="sxs-lookup"><span data-stu-id="f626d-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="f626d-109">Введіть **Office 365 Yammer** , у полі пошуку та виберіть ім'я програми, щоб відкрити параметри.</span><span class="sxs-lookup"><span data-stu-id="f626d-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="f626d-110">Виберіть **Властивості** під **керування** в області переходів ліворуч.</span><span class="sxs-lookup"><span data-stu-id="f626d-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="f626d-111">Встановити значення **увімкнуто для входу в систему?** щоб **так**, а потім виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="f626d-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="f626d-112">Увійдіть у Yammer знову.</span><span class="sxs-lookup"><span data-stu-id="f626d-112">Sign in to Yammer again.</span></span> <span data-ttu-id="f626d-113">Можливо, потрібно буде очистити файли cookie.</span><span class="sxs-lookup"><span data-stu-id="f626d-113">You might need to clear cookies.</span></span>

<span data-ttu-id="f626d-114">Крім того, запустити команди PowerShell, щоб установити значення.</span><span class="sxs-lookup"><span data-stu-id="f626d-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="f626d-115">Щоб отримати додаткові відомості, див ["Вибачте, але у нас виникли проблеми з входом" помилка під час натискання кнопки Yammer плитки в Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f626d-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 