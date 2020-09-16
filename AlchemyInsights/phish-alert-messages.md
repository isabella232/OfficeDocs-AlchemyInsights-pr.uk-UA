---
title: 2491 оповіщення електронної пошти з "Phpish доставлено через політику клієнта або" Перезаписати користувача "
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728632"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7bccc-102">Оповіщення електронної пошти з "Phpish доставлено через політику клієнта або" перевизначення користувача "</span><span class="sxs-lookup"><span data-stu-id="7bccc-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7bccc-103">Для орендарів із ліцензіями на Office 365 АТФ P1 і P2 можна використовувати політику оповіщення за замовчуванням під назвою "Phish доставлено за рахунок клієнта або перевизначення користувачем".</span><span class="sxs-lookup"><span data-stu-id="7bccc-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7bccc-104">Якщо ви отримали це оповіщення, Ось кроки, які потрібно дослідити:</span><span class="sxs-lookup"><span data-stu-id="7bccc-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7bccc-105">У сповіщенні виберіть пункт **Переглянути оповіщення** , щоб перейти на сторінку **оповіщення** в центрі відповідності & безпеки.</span><span class="sxs-lookup"><span data-stu-id="7bccc-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7bccc-106">Виберіть оповіщення, щоб переглянути **список повідомлень** або **Переглянути повідомлення в провіднику**.</span><span class="sxs-lookup"><span data-stu-id="7bccc-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7bccc-107">Обидва ці варіанти містять відомості про повідомлення, яке включає ІДЕНТИФІКАТОР повідомлення.</span><span class="sxs-lookup"><span data-stu-id="7bccc-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7bccc-108">Зверніть увагу, що посилання провідник загроз буде автоматично відфільтровувати повідомлення, які відповідають умовам оповіщення.</span><span class="sxs-lookup"><span data-stu-id="7bccc-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7bccc-109">Можливо, знадобиться настроїти фільтр дат у провіднику загроз.</span><span class="sxs-lookup"><span data-stu-id="7bccc-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7bccc-110">Фішингове повідомлення доставлено через те, що настроєні вручну перевизначити:</span><span class="sxs-lookup"><span data-stu-id="7bccc-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7bccc-111">Дозволений відправник або домен, встановлений користувачем.</span><span class="sxs-lookup"><span data-stu-id="7bccc-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7bccc-112">Дозволений відправник або домен, встановлений адміністратором в політиці захисту від спаму.</span><span class="sxs-lookup"><span data-stu-id="7bccc-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7bccc-113">Дозволена ІР-адреса в політиці фільтра підключення.</span><span class="sxs-lookup"><span data-stu-id="7bccc-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7bccc-114">Правило потоку пошти (також відомий як правило транспортування), який настроєно для надання повідомленням.</span><span class="sxs-lookup"><span data-stu-id="7bccc-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7bccc-115">Якщо ви вважаєте, що повідомлення неправильно позначено як phpish, скористайтеся [надбудовою повідомлення звіту](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook, щоб надсилати зразки повідомлень до корпорації Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7bccc-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
