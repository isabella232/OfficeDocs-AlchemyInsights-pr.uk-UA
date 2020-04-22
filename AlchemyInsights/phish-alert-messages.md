---
title: 2491 оповіщення електронної пошти з Phish доставлено через політику клієнта або перевизначення користувача
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758955"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="41fc7-102">Оповіщення електронної пошти від ' Phish доставлено через політику клієнта або перевизначення користувачів</span><span class="sxs-lookup"><span data-stu-id="41fc7-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="41fc7-103">Політика оповіщення за промовчанням під назвою "Phish доставлено через клієнта або перевизначення користувача" була розгорнута орендарям з Office 365 АТФ P1 і P2 ліцензій.</span><span class="sxs-lookup"><span data-stu-id="41fc7-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="41fc7-104">Якщо ви отримали це оповіщення, Ось кроки для розслідування:</span><span class="sxs-lookup"><span data-stu-id="41fc7-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="41fc7-105">У сповіщенні повідомлення натисніть кнопку **Переглянути оповіщення** , щоб перейти на сторінку **оповіщень** у центрі дотримання безпеки &.</span><span class="sxs-lookup"><span data-stu-id="41fc7-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="41fc7-106">Виберіть оповіщення, щоб побачити опцію **перегляду списку повідомлень** або **перегляду повідомлень у провіднику**.</span><span class="sxs-lookup"><span data-stu-id="41fc7-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="41fc7-107">Обидва ці параметри, можна отримати відомості про повідомлення, який містить ІДЕНТИФІКАТОР повідомлення.</span><span class="sxs-lookup"><span data-stu-id="41fc7-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="41fc7-108">Зауважте, що посилання на провідник загроз автоматично відфільтровувати повідомлення, які відповідають умовам оповіщення.</span><span class="sxs-lookup"><span data-stu-id="41fc7-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="41fc7-109">Можливо, потрібно буде відкоригувати фільтр дат у провіднику загроз.</span><span class="sxs-lookup"><span data-stu-id="41fc7-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="41fc7-110">Фішингове повідомлення доставлено через настроєне вручну заміщення:</span><span class="sxs-lookup"><span data-stu-id="41fc7-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="41fc7-111">Дозволений відправник або домен, встановлений користувачем.</span><span class="sxs-lookup"><span data-stu-id="41fc7-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="41fc7-112">Дозволений відправник або домен, встановлений адміністратором, у політиці захисту від спаму.</span><span class="sxs-lookup"><span data-stu-id="41fc7-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="41fc7-113">Дозволена IP-адреса у політиці фільтрування підключень.</span><span class="sxs-lookup"><span data-stu-id="41fc7-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="41fc7-114">Правило потоку пошти (також відоме як правило транспортування), настроєного для надання повідомлень.</span><span class="sxs-lookup"><span data-stu-id="41fc7-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="41fc7-115">Якщо ви вважаєте, що повідомлення помилково позначено як phish, використовуйте [надбудову повідомлення звіту](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook для надсилання зразків повідомлень до корпорації Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="41fc7-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
