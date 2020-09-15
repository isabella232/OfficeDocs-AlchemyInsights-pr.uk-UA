---
title: Вимкнення зовнішніх груп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704149"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="333f6-102">Вимкнення зовнішніх груп</span><span class="sxs-lookup"><span data-stu-id="333f6-102">How to disable External Groups</span></span>

<span data-ttu-id="333f6-103">Зовнішні повідомлення Yammer застосовуються правила транспортування Exchange (ETRs), набір активних елементів керування, щоб заборонити спільний доступ до інформації про компанію.</span><span class="sxs-lookup"><span data-stu-id="333f6-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="333f6-104">Щоб обмежити користувачам створювати зовнішні групи, потрібно настроїти правило транспортування Exchange (ETR), а потім настроїти Yammer на використання правила транспортування Exchange, щоб заблокувати зовнішні повідомлення.</span><span class="sxs-lookup"><span data-stu-id="333f6-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="333f6-105">Після створення правила в центрі адміністрування Exchange Online виконайте наведені нижче дії, щоб указати ETR, щоб застосувати в Yammer:</span><span class="sxs-lookup"><span data-stu-id="333f6-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="333f6-106">Увійдіть у Yammer як перевірений адміністратор і в **центрі адміністрування Yammer**перейдіть до розділу " **вміст вмісту" та " \> Параметри безпеки безпеки".**</span><span class="sxs-lookup"><span data-stu-id="333f6-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="333f6-107">У розділі **зовнішні повідомлення**виберіть пункт **застосувати правила транспортування Exchange Online (Etrs) у Yammer.**</span><span class="sxs-lookup"><span data-stu-id="333f6-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="333f6-108">Натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="333f6-108">Choose **Save**.</span></span>

<span data-ttu-id="333f6-109">Докладні відомості наведено в статті [вимкнення зовнішніх повідомлень у мережі Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="333f6-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  