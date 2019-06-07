---
title: 646 як налаштувати AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752582"
---
# <a name="configure-sync-features"></a><span data-ttu-id="3adb1-102">Настроювання синхронізації функцій</span><span class="sxs-lookup"><span data-stu-id="3adb1-102">Configure sync features</span></span>

<span data-ttu-id="3adb1-103">Блакитні оголошення підключення включає кілька функцій, що включений за замовчуванням або яку можна ввімкнути пізніше.</span><span class="sxs-lookup"><span data-stu-id="3adb1-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="3adb1-104">Деякі функції вимагають додаткових налаштувань в конкретних умовах.</span><span class="sxs-lookup"><span data-stu-id="3adb1-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="3adb1-105">[Фільтрування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) межі об'єкти синхронізуються блакитні оголошення.</span><span class="sxs-lookup"><span data-stu-id="3adb1-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="3adb1-106">За замовчуванням, всі користувачі, контакти, групи та версії 10 синхронізуються комп'ютер облікових записів.</span><span class="sxs-lookup"><span data-stu-id="3adb1-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="3adb1-107">Ви можете додати або вилучити об'єктів на основі доменів, підрозділи та інші атрибути.</span><span class="sxs-lookup"><span data-stu-id="3adb1-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="3adb1-108">[Пароль хеш синхронізацію](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронізація пароля хеш із локальної служби Active Directory до блакитні оголошення.</span><span class="sxs-lookup"><span data-stu-id="3adb1-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="3adb1-109">Це дозволяє Керування паролями в одному місці, але використовувати однаковий пароль в обох локальні та хмарними.</span><span class="sxs-lookup"><span data-stu-id="3adb1-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="3adb1-110">Тому, що Active Directory надійного джерела, ви можете використовувати свій власний політики паролів.</span><span class="sxs-lookup"><span data-stu-id="3adb1-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="3adb1-111">[Скидання пароля самообслуговування (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) дозволяє користувачам можливість скидати паролі у хмарі при застосуванні як і раніше ваш пароль локальною політикою.</span><span class="sxs-lookup"><span data-stu-id="3adb1-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="3adb1-112">[Пристрій writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) надає змогу зареєстрованим у блакитній оголошення, щоб записати назад до локальної служби Active Directory так що вони можуть бути використані для умовного доступу.</span><span class="sxs-lookup"><span data-stu-id="3adb1-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="3adb1-113">[Випадкове ю видалення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ввімкнуто за промовчанням, щоб запобігти забагато видалень синхронний об'єкта (більш ніж 500 об'єктів на синхронізацію).</span><span class="sxs-lookup"><span data-stu-id="3adb1-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="3adb1-114">Можна змінити цей параметр для задоволення потреб вашої організації.</span><span class="sxs-lookup"><span data-stu-id="3adb1-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="3adb1-115">[Автоматичні оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ввімкнуто за промовчанням для Експрес установок і допомагає забезпечити вашу версію Azure оголошення Коннект актуальний завжди.</span><span class="sxs-lookup"><span data-stu-id="3adb1-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
