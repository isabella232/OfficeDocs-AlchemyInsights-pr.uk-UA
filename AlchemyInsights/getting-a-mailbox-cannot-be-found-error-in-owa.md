---
title: 126 Не вдалося знайти поштову скриньку в OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426683"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="40fd5-102">Сталася помилка поштової скриньки в інтернет-версії Outlook?</span><span class="sxs-lookup"><span data-stu-id="40fd5-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="40fd5-103">Якщо під час використання інтернет-версії Outlook  не вдалося знайти поштову скриньку, це означає, що обліковий запис, який використовувався для підключення до інтернет-версії Outlook, не має ліцензії на Exchange Online, тому з обліковим записом не пов'язано жодної поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="40fd5-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="40fd5-104">Адміністратор може призначити ліцензію для вашого облікового запису, виконавши такі дії:</span><span class="sxs-lookup"><span data-stu-id="40fd5-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="40fd5-105">Відкрийте  [Центр адміністрування Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) у  розділі Користувачі перейдіть до розділу Активні користувачі та виберіть користувача, який побачить помилку.</span><span class="sxs-lookup"><span data-stu-id="40fd5-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="40fd5-106">На сторінці користувача, що відкриється, перейдіть до розділу Ліцензії  та програми, виберіть відповідне значення розташування та призначте ліцензію, яка містить Exchange Online (розгорніть ліцензію, щоб переглянути відомості про неї). </span><span class="sxs-lookup"><span data-stu-id="40fd5-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="40fd5-107">Завершивши, натисніть кнопку **Зберегти зміни.**</span><span class="sxs-lookup"><span data-stu-id="40fd5-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="40fd5-108">У деяких випадках, якщо ліцензію вже призначено обліковому запису користувача, видалення та повторне призначення ліцензії допомагає вирішити цю проблему та належним чином підготувати її в системі:</span><span class="sxs-lookup"><span data-stu-id="40fd5-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="40fd5-109">Перевірте, чи не закінчуються передплати на план M365 Exchange Online (та інші передплати, якщо у вас є).</span><span class="sxs-lookup"><span data-stu-id="40fd5-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="40fd5-110">Коли ви переконаєтеся, що термін дії передплати не минув і обліковому запису користувача призначено дійсну ліцензію, ліцензію може тривати до 24 годин, тому, можливо, доведеться зачекати, доки проблему не буде вирішено.</span><span class="sxs-lookup"><span data-stu-id="40fd5-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="40fd5-111">Докладні відомості див. [в розділі Призначення ліцензій і керування ними.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="40fd5-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>