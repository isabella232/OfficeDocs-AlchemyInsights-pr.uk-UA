---
title: Вимкнення зовнішнього груп
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399684"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="fa619-102">Вимкнення зовнішнього груп</span><span class="sxs-lookup"><span data-stu-id="fa619-102">How to disable External Groups</span></span>

<span data-ttu-id="fa619-103">Нити зовнішніх повідомленнями застосовує біржі правила транспортування (ETRs), набір Проактивний контролю з метою недопущення компанія інформації.</span><span class="sxs-lookup"><span data-stu-id="fa619-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="fa619-104">Для того, щоб заборонити користувачам створення зовнішніх груп, вам потрібно налаштувати правила транспортування Exchange (ОПК) а потім настроїти Yammer використовувати правила транспортування Exchange Блокувати зовнішні обміну повідомленнями.</span><span class="sxs-lookup"><span data-stu-id="fa619-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="fa619-105">Після того, як правило було створено в Exchange Online Центр адміністрування, виконайте такі дії, щоб встановити ЕТР вносити Yammer</span><span class="sxs-lookup"><span data-stu-id="fa619-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="fa619-106">Увійти до Yammer як перевірені адміністратора а в **нити Центр адміністрування**, перейдіть на C **ontent і безпеки \> настройки безпеки.**</span><span class="sxs-lookup"><span data-stu-id="fa619-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="fa619-107">У розділі **Зовнішні обміну повідомленнями**, виберіть **забезпечити дотримання ваш Exchange Online Exchange правил транспортування (ETRs) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="fa619-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="fa619-108">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="fa619-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="fa619-109">Для отримання додаткових відомостей див. [керування зовнішніх служб обміну повідомленнями Yammer мережі з правил транспортування Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="fa619-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

