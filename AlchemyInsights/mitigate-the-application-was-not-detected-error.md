---
title: Виправлення помилки "Програму не виявлено"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666999"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="12591-102">Виправлення помилки "Програму не виявлено"</span><span class="sxs-lookup"><span data-stu-id="12591-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="12591-103">Помилка інсталяції програми "Програму не виявлено після успішної інсталяції", про яку повідомляє Intune, може статися на всіх основних платформах ОС (Windows, iOS і Android).</span><span class="sxs-lookup"><span data-stu-id="12591-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="12591-104">Найпоширеніші сценарії, які призводять до цієї помилки:</span><span class="sxs-lookup"><span data-stu-id="12591-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="12591-105">Після початкового розгортання програму оновлено за межами Intune (зі стороннього магазину програм).</span><span class="sxs-lookup"><span data-stu-id="12591-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="12591-106">Деякі програми, як-от Google Chrome, можуть оновлюватись автоматично.</span><span class="sxs-lookup"><span data-stu-id="12591-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="12591-107">Користувач видалив програму після початкової інсталяції.</span><span class="sxs-lookup"><span data-stu-id="12591-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="12591-108">Щоб вирішити цю проблему, спершу перевірте уражені пристрої, щоб визначити сценарій, у якому сталася помилка.</span><span class="sxs-lookup"><span data-stu-id="12591-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="12591-109">Якщо програму оновлено за межами Intune, у налаштуваннях розгортання програми можна вказати, що версію програми слід ігнорувати.</span><span class="sxs-lookup"><span data-stu-id="12591-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="12591-110">Для цього клацніть **Конфігурація програми > Відомості про програму** й виберіть для параметра **Ігнорувати версію програми** значення **Так**.</span><span class="sxs-lookup"><span data-stu-id="12591-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="12591-111">Для певних цільових клієнтів програму доцільно розгорнути як "обов’язкову" й вимагати, щоб використовувалася її найновіша версія.</span><span class="sxs-lookup"><span data-stu-id="12591-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="12591-112">Крім того, на платформі iOS можна використовувати функцію **автооновлення**, пов’язану з програмою придбання Apple Volume Purchase Program, для якої можна налаштувати автоматичне оновлення до нових версій програм, коли вони стануть доступними.</span><span class="sxs-lookup"><span data-stu-id="12591-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="12591-113">Докладні відомості про виправлення помилок під час інсталяції програм див. в статті [Виправлення неполадок під час інсталяції програм](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="12591-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
