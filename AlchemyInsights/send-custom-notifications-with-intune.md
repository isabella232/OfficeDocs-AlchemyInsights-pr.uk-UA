---
title: Надсилання користувацьких сповіщень за допомогою InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992333"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="44623-102">Як надсилати користувацькі сповіщення користувачам керованих iOS та Android пристроїв</span><span class="sxs-lookup"><span data-stu-id="44623-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="44623-103">Настроювані сповіщення для InTune обробляються застосунок порталу компанії на пристрої користувача.</span><span class="sxs-lookup"><span data-stu-id="44623-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="44623-104">Потім програма створює Push-сповіщення на цьому пристрої.</span><span class="sxs-lookup"><span data-stu-id="44623-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="44623-105">Нижче наведено передумови пристрою для підтримки отримання користувацьких сповіщень, а також для програми, щоб створити Push-сповіщення:</span><span class="sxs-lookup"><span data-stu-id="44623-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="44623-106">Пристрій повинен мати програму порталу компанії, встановленої.</span><span class="sxs-lookup"><span data-stu-id="44623-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="44623-107">Пристрій повинен дозволяти програмі "портал компанії" надсилати Push-сповіщення.</span><span class="sxs-lookup"><span data-stu-id="44623-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="44623-108">Коли програма інсталюється або оновлюється, він запропонує користувачу дозвіл на отримання сповіщень.</span><span class="sxs-lookup"><span data-stu-id="44623-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="44623-109">На пристроях Android потрібно встановити сервіси Google Play.</span><span class="sxs-lookup"><span data-stu-id="44623-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="44623-110">Пристрій має бути зареєстровано з InTune.</span><span class="sxs-lookup"><span data-stu-id="44623-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="44623-111">Докладніші відомості про надсилання повідомлення наведено в [документації до функції](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="44623-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
