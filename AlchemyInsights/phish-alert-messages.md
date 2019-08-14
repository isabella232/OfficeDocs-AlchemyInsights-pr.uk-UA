---
title: 2491 оповіщення електронної пошти від Phish доставлені через орендар або користувач перевизначити політики
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391612"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7c4de-102">Оповіщення електронної пошти від Phish доставлені через орендар або користувач перевизначити політики</span><span class="sxs-lookup"><span data-stu-id="7c4de-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7c4de-103">Політика за промовчанням оповіщення названий "Phish доставлено за рахунок орендаря або користувач перевизначити" була розгорнута орендарям з Office 365 АТФ P1, P2 і ліцензій.</span><span class="sxs-lookup"><span data-stu-id="7c4de-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7c4de-104">Якщо ви отримали це попередження, Ось кроки для розслідування:</span><span class="sxs-lookup"><span data-stu-id="7c4de-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7c4de-105">Це повідомлення натисніть кнопку **Вигляд оповіщення** , щоб перейти на сторінку **оповіщення** в безпеки & центрі дотримання.</span><span class="sxs-lookup"><span data-stu-id="7c4de-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7c4de-106">Виберіть оповіщення, щоб знайти опцію для **подання списку повідомлень** або **Перегляд повідомлень у провіднику**.</span><span class="sxs-lookup"><span data-stu-id="7c4de-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7c4de-107">Обидва ці варіанти взяти вас відомості про повідомлення, яке містить ідентифікатор повідомлення.</span><span class="sxs-lookup"><span data-stu-id="7c4de-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7c4de-108">Зверніть увагу, що загроза Explorer посилання автоматично відфільтровує повідомленнями, які вдовольняють умовам оповіщення.</span><span class="sxs-lookup"><span data-stu-id="7c4de-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7c4de-109">Може знадобитися відрегулювати загрозу Explorer, фільтр Дата.</span><span class="sxs-lookup"><span data-stu-id="7c4de-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7c4de-110">Фішингові повідомлення було доставлено через вручну перевизначити:</span><span class="sxs-lookup"><span data-stu-id="7c4de-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7c4de-111">Дозволених відправника або в домені користувачем.</span><span class="sxs-lookup"><span data-stu-id="7c4de-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7c4de-112">Дозволених відправника або в домені адміністратором в анти-спам політика.</span><span class="sxs-lookup"><span data-stu-id="7c4de-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7c4de-113">Дозволених ІР-адреси в зв'язок політики фільтру.</span><span class="sxs-lookup"><span data-stu-id="7c4de-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7c4de-114">Пошта потоку правило (також відомі як правила транспортування), настроєного дозволяє обробляти повідомлення в.</span><span class="sxs-lookup"><span data-stu-id="7c4de-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7c4de-115">Якщо ви вважаєте, що повідомлення було помилково позначено як рибка спіймана, скористатися в Outlook, [надбудова звіт повідомлення](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) повідомлення зразки до корпорації Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7c4de-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
