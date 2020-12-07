---
title: Піктограма календаря не відображається в клієнті команд Microsoft
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583931"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="6e6b3-102">Піктограма календаря не відображається в клієнті команд Microsoft</span><span class="sxs-lookup"><span data-stu-id="6e6b3-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="6e6b3-103">Вкладка " **календар** " в командах потребує доступу до поштової скриньки Exchange за допомогою веб-служб Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="6e6b3-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="6e6b3-104">Поштова скринька Exchange може перебувати в Інтернеті або в локальній мережі.</span><span class="sxs-lookup"><span data-stu-id="6e6b3-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="6e6b3-105">Для користувачів Online, які не бачать вкладку **календар** , переконайтеся, що вони [ліцензовані для поштової скриньки Exchange Online, а поштова скринька увімкнена](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="6e6b3-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="6e6b3-106">Якщо користувачі перебувають на локальному комп'ютері, потрібно підтвердити, що ваша Гібридна конфігурація здорова.</span><span class="sxs-lookup"><span data-stu-id="6e6b3-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="6e6b3-107">Щоб вирішити проблему, скористайтеся [майстром гібридної конфігурації](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="6e6b3-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="6e6b3-108">Зверніть увагу, що [для Teams необхідно інсталювати Exchange 2016 CU3 або новішої версії](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="6e6b3-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="6e6b3-109">Щоб отримати докладніші відомості та вказівки з виправлення неполадок, перегляньте статтю [Виправлення неполадок із командами Microsoft і даними взаємодії сервера Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="6e6b3-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
