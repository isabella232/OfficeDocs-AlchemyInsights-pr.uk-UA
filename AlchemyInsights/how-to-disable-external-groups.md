---
title: Вимкнення зовнішнього груп
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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384846"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="794fc-102">Вимкнення зовнішнього груп</span><span class="sxs-lookup"><span data-stu-id="794fc-102">How to disable External Groups</span></span>

<span data-ttu-id="794fc-103">Нити зовнішніх повідомленнями застосовує біржі правила транспортування (ETRs), набір Проактивний контролю з метою недопущення компанія інформації.</span><span class="sxs-lookup"><span data-stu-id="794fc-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="794fc-104">Для того, щоб заборонити користувачам створення зовнішніх груп, вам потрібно налаштувати правила транспортування Exchange (ОПК) а потім настроїти Yammer використовувати правила транспортування Exchange Блокувати зовнішні обміну повідомленнями.</span><span class="sxs-lookup"><span data-stu-id="794fc-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="794fc-105">Після того, як правило було створено в Exchange Online Центр адміністрування, виконайте такі дії, щоб встановити ЕТР вносити Yammer</span><span class="sxs-lookup"><span data-stu-id="794fc-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="794fc-106">Увійти до Yammer як перевірені адміністратора а в **нити Центр адміністрування**, перейдіть на C **зміст і безпеки \> настройки безпеки.**</span><span class="sxs-lookup"><span data-stu-id="794fc-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="794fc-107">У розділі **Зовнішні обміну повідомленнями**, виберіть **забезпечити дотримання ваш Exchange Online Exchange правил транспортування (ETRs) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="794fc-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="794fc-108">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="794fc-108">Choose **Save**.</span></span>

<span data-ttu-id="794fc-109">Для отримання додаткових відомостей див. [керування зовнішніх служб обміну повідомленнями Yammer мережі з правил транспортування Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="794fc-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  