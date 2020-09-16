---
title: Надсилання користувацьких сповіщень на InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720667"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="e071d-102">Надсилання власних сповіщень користувачам керованих пристроїв із iOS і Android</span><span class="sxs-lookup"><span data-stu-id="e071d-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="e071d-103">Користувацькі сповіщення для Inune обробляються програмою "портал компанії" на пристрої користувача.</span><span class="sxs-lookup"><span data-stu-id="e071d-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="e071d-104">Після цього програма створить сповіщення про Push-повідомлення на цьому пристрої.</span><span class="sxs-lookup"><span data-stu-id="e071d-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="e071d-105">Нижче наведено попередні вимоги до пристрою, щоб підтримувати отримання власних сповіщень, а також для програми, щоб створити сповіщення про Push-повідомлення:</span><span class="sxs-lookup"><span data-stu-id="e071d-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="e071d-106">На пристрої має бути інстальовано програму "портал компанії".</span><span class="sxs-lookup"><span data-stu-id="e071d-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="e071d-107">Пристрій має дозволити програмі "портал компанії" передавати Push-сповіщення.</span><span class="sxs-lookup"><span data-stu-id="e071d-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="e071d-108">Коли програму інстальовано або оновлено, буде запропоновано користувачу дозволяти сповіщення.</span><span class="sxs-lookup"><span data-stu-id="e071d-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="e071d-109">На пристроях з Android має бути інстальовано служби Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="e071d-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="e071d-110">Пристрій має бути зареєстровано в програмі Inune.</span><span class="sxs-lookup"><span data-stu-id="e071d-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="e071d-111">Щоб отримати докладні відомості, зокрема про те, як відправити повідомлення, ознайомтеся з [документацією для функцій](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="e071d-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
