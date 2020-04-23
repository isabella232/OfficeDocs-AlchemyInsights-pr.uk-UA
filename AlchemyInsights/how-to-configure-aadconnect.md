---
title: 646 як налаштувати AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722584"
---
# <a name="configure-sync-features"></a><span data-ttu-id="838c9-102">Настроювання функцій синхронізації</span><span class="sxs-lookup"><span data-stu-id="838c9-102">Configure sync features</span></span>

<span data-ttu-id="838c9-103">Azure AD-підключення, містить кілька функцій, які ввімкнуто за промовчанням або можна ввімкнути пізніше.</span><span class="sxs-lookup"><span data-stu-id="838c9-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="838c9-104">Деякі функції потребують додаткової конфігурації в певних середовищах.</span><span class="sxs-lookup"><span data-stu-id="838c9-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="838c9-105">[Фільтрування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обмеження об'єкти СИНХРОНІЗУЮТЬСЯ Azure AD.</span><span class="sxs-lookup"><span data-stu-id="838c9-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="838c9-106">За промовчанням синхронізуються всі користувачі, контакти, групи та комп'ютерні облікові записи Windows 10.</span><span class="sxs-lookup"><span data-stu-id="838c9-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="838c9-107">Можна включити або виключити об'єкти на основі доменів, OUs або інших атрибутів.</span><span class="sxs-lookup"><span data-stu-id="838c9-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="838c9-108">[Геш-синхронізація пароля](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронізує геш-пароль з локальної служби Active Directory для Azure AD.</span><span class="sxs-lookup"><span data-stu-id="838c9-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="838c9-109">Це дозволяє Керування паролями в одному розташуванні, але використання одного і того ж пароля в локальних і хмарних середовищах.</span><span class="sxs-lookup"><span data-stu-id="838c9-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="838c9-110">Оскільки Active Directory є авторитетним джерелом, ви можете використовувати свої власні політики паролів.</span><span class="sxs-lookup"><span data-stu-id="838c9-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="838c9-111">[Самостійне скидання пароля (sсрп)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) дозволяє користувачам скидати свої власні паролі в хмарі, а ще застосування вашої локальної політики паролів.</span><span class="sxs-lookup"><span data-stu-id="838c9-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="838c9-112">[Пристрій writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) дозволяє зареєстровані пристрої в Azure AD, щоб бути написана на локальному Active Directory, щоб вони могли бути використані для умовного доступу.</span><span class="sxs-lookup"><span data-stu-id="838c9-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="838c9-113">[Запобігання випадковому видалення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) увімкнуто за промовчанням, щоб запобігти занадто багато одночасних видалення об'єктів (більше 500 об'єктів на синхронізацію).</span><span class="sxs-lookup"><span data-stu-id="838c9-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="838c9-114">Ви можете змінити цей параметр, щоб задовольнити потреби вашої організації.</span><span class="sxs-lookup"><span data-stu-id="838c9-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="838c9-115">[Автоматичне оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) увімкнуто за промовчанням для Експрес-інсталяції та гарантує, що ваша версія Azure AD-підключення завжди поточного.</span><span class="sxs-lookup"><span data-stu-id="838c9-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
