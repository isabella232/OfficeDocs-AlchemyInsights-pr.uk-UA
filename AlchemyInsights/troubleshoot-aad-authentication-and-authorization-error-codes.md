---
title: Усунення несправностей із кодами помилок автентифікації Azure AD і авторизації (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037843"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="7b7b6-102">Усунення несправностей із кодами помилок автентифікації Azure AD і авторизації (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="7b7b6-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="7b7b6-103">Щоб вирішити помилки автентифікації AAD і коди помилок авторизації (AADSTS), виконайте наведені нижче Рекомендовані дії.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="7b7b6-104">**Оброблення кодів помилок у програмі**</span><span class="sxs-lookup"><span data-stu-id="7b7b6-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="7b7b6-105">Функція **OAuth 2.0 Spec** https://tools.ietf.org/html/rfc6749#section-5.2 дає вказівки про те, як обробляти помилки під час автентифікації за допомогою частини помилки під час відповіді на помилку.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="7b7b6-106">**Помилка**: рядок коду помилки, який можна використовувати для класифікації типів помилок, які трапляються, і їх слід використовувати для реагування на помилки.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="7b7b6-107">У полі " **Помилка** " є кілька можливих значень: огляд посилань на протоколи документації та "oauth 2,0 специфікації" для отримання додаткових відомостей про певні помилки та способи їх реагування на них.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="7b7b6-108">Нижче наведено зразок відповіді про помилку:</span><span class="sxs-lookup"><span data-stu-id="7b7b6-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="7b7b6-109">**Підстановка поточних відомостей про код помилки**</span><span class="sxs-lookup"><span data-stu-id="7b7b6-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="7b7b6-110">Коди помилок і повідомлення можуть змінюватися.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="7b7b6-111">Щоб отримати найактуальніші відомості, перегляньте https://login.microsoftonline.com/error сторінку, щоб знайти описи помилок AADSTS, виправлення та деякі запропоновані способи вирішення.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="7b7b6-112">Ви також можете шукати та усувати [коди помилок Aadsts](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , перелічені в розділі [коди автентифікації в статті Azure AD і помилки авторизації](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="7b7b6-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="7b7b6-113">**Отримання довідки**</span><span class="sxs-lookup"><span data-stu-id="7b7b6-113">**Get Help**</span></span>

- <span data-ttu-id="7b7b6-114">[Варіанти підтримки та довідки для розробників](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – якщо вам потрібна відповідь на запитання або довідку з вирішення проблем, не охоплених нашою документацією, можливо, настав час охопити фахівців для довідки.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="7b7b6-115">У цій статті наведено кілька порад, які допоможуть отримати відповіді на запитання, коли ви розробляєте програми, які інтегруються з платформою ідентифікації Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b7b6-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








