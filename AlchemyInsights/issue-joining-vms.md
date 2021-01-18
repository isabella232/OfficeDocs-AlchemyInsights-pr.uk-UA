---
title: Проблеми з приєднанням віртуальних машин
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885657"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="c02f8-102">Проблеми з приєднанням віртуальних машин</span><span class="sxs-lookup"><span data-stu-id="c02f8-102">Issue joining VMs</span></span>

<span data-ttu-id="c02f8-103">Щоб вирішити проблеми, які виникають під час спроби приєднатися до віртуальних машин, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="c02f8-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="c02f8-104">Виконайте вхід за допомогою формату **UPN** (наприклад, "joeuser@contoso.com") замість формату **SAMAccountName** ("CONTOSO\joeuser").</span><span class="sxs-lookup"><span data-stu-id="c02f8-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="c02f8-105">Переконайтеся, що ви ввімкнули синхронізацію паролів відповідно до інструкцій, наведених у посібнику з *початку роботи* .</span><span class="sxs-lookup"><span data-stu-id="c02f8-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="c02f8-106">Переконайтеся, що обліковий запис користувача не є зовнішнім обліковим записом у клієнті Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c02f8-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="c02f8-107">Зовнішні користувачі не можуть входити в керований домен, оскільки служби домену Azure AD не мають облікових даних для таких облікових записів користувачів.</span><span class="sxs-lookup"><span data-stu-id="c02f8-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="c02f8-108">Якщо обліковий запис користувача – це лише хмарний обліковий запис, переконайтеся, що користувачі змінили свій пароль після ввімкнення служб домену Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c02f8-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="c02f8-109">Цей крок спричиняє створення хеш-суми облікових даних, потрібних для створення служб домену Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c02f8-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="c02f8-110">Якщо облікові записи користувачів синхронізовано з локального каталогу, переконайтеся, що для виконання повної синхронізації було настроєно рекомендований випуск підключення Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c02f8-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="c02f8-111">Якщо проблему не вирішено після підтвердження кроку 4, виконайте наведені нижче команди з вашого комп'ютера синхронізації.</span><span class="sxs-lookup"><span data-stu-id="c02f8-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="c02f8-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="c02f8-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>