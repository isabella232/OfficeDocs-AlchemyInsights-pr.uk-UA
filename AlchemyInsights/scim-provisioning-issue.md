---
title: Проблема підготовки SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949952"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="cac3c-102">Проблема підготовки SCIM</span><span class="sxs-lookup"><span data-stu-id="cac3c-102">SCIM provisioning issue</span></span>

<span data-ttu-id="cac3c-103">Функція автоматичного підготовки відповідає за створення посвідчень та ролей користувачів у хмарних програмах, до яких користувачам потрібен доступ.</span><span class="sxs-lookup"><span data-stu-id="cac3c-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="cac3c-104">Крім створення посвідчень користувачів, функція автоматичного підготовки включає в себе обслуговування та видалення посвідчень користувачів як зміни стану або ролей.</span><span class="sxs-lookup"><span data-stu-id="cac3c-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="cac3c-105">Перш ніж почати розгортання, можна переглянути, [як працює підготовка](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) , щоб дізнатися, як працює положення Azure Active Directory (AD), а також отримати рекомендації з конфігурації.</span><span class="sxs-lookup"><span data-stu-id="cac3c-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="cac3c-106">Як розробник програми, ви можете використовувати систему для керування обліковими записами для перехресного домену (SCIM), щоб активувати автоматичну підготовку користувачів і груп між вашою програмою та Лазуровою ОБ'ЯВАМИ.</span><span class="sxs-lookup"><span data-stu-id="cac3c-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="cac3c-107">У статті [створення кінцевої точки SCIM і настроювання підготовки користувачів за допомогою служби AZURE AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) . описується, як створити кінцеву точку SCIM і інтегрувати її в службу підготовки Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cac3c-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



