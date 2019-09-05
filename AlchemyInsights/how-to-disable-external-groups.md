---
title: Як відключити зовнішні групи
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739514"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="f645b-102">Як відключити зовнішні групи</span><span class="sxs-lookup"><span data-stu-id="f645b-102">How to disable External Groups</span></span>

<span data-ttu-id="f645b-103">За зовнішнім повідомленнями Yammer застосовуються правила транспортування Exchange (ETRs), набір проактивних елементів керування, які забороняють спільний доступ до інформації про компанію.</span><span class="sxs-lookup"><span data-stu-id="f645b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="f645b-104">Для того, щоб заборонити користувачам створювати зовнішні групи, потрібно настроїти правило транспортування Exchange (ETR), а потім настроїти Yammer для використання правила транспортування Exchange для блокування зовнішніх повідомлень.</span><span class="sxs-lookup"><span data-stu-id="f645b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="f645b-105">Після того, як ви створили правило в Exchange Online центру адміністрування, виконайте такі дії, щоб установити ETR для застосування в Yammer:</span><span class="sxs-lookup"><span data-stu-id="f645b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="f645b-106">Увійдіть до Yammer як перевірений адміністратор, а в **центрі адміністрування Yammer**перейдіть до розділу \*\* \> вміст і параметри безпеки.\*\*</span><span class="sxs-lookup"><span data-stu-id="f645b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="f645b-107">У розділі **зовнішні повідомлення**виберіть елемент **застосувати правила транспортування Exchange Online (etrs) у Yammer.**</span><span class="sxs-lookup"><span data-stu-id="f645b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="f645b-108">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="f645b-108">Choose **Save**.</span></span>

<span data-ttu-id="f645b-109">Для отримання додаткових відомостей див. [вимкнення зовнішніх повідомлень у мережі Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="f645b-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  