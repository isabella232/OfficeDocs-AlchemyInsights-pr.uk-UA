---
title: Виправлення неполадок із згодою користувача
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901625"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="32472-102">Виправлення неполадок із згодою користувача</span><span class="sxs-lookup"><span data-stu-id="32472-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="32472-103">Ви можете налаштувати спосіб згоди користувачів на програми за допомогою порталу "Лазурний" або PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32472-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="32472-104">Щоб отримати докладніші відомості, ознайомтеся з [настройками згоди користувача](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="32472-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="32472-105">Адміністратор також може використовувати [Microsoft GRAPH API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , щоб надати згоду на делеговані дозволи від імені одного користувача.</span><span class="sxs-lookup"><span data-stu-id="32472-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="32472-106">Докладні відомості наведено в статті [отримати доступ від імені користувача](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="32472-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="32472-107">[Помилки згоди користувачів](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): у цій статті розглядаються помилки, які можуть виникати під час процесу згоди на програму.</span><span class="sxs-lookup"><span data-stu-id="32472-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="32472-108">Якщо ви не маєте права на запити про неочікувані згоди, які не містять повідомлень про помилки, ознайомтеся [з сценаріями автентифікації для Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="32472-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>