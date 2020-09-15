---
title: 646 як настроїти AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704510"
---
# <a name="configure-sync-features"></a><span data-ttu-id="dd0ae-102">Настроювання функцій синхронізації</span><span class="sxs-lookup"><span data-stu-id="dd0ae-102">Configure sync features</span></span>

<span data-ttu-id="dd0ae-103">Azure AD Connect містить кілька функцій, які ввімкнуто за замовчуванням, або які можна ввімкнути згодом.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="dd0ae-104">Деякі функції потребують додаткової конфігурації в певних середовищах.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="dd0ae-105">[Фільтрування](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обмежує об'єкти, синхронізовані з ЛАЗУРОЧНИМ оголошенням.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="dd0ae-106">За замовчуванням для всіх користувачів, контактів, груп і комп'ютерів із Windows 10 синхронізуються облікові записи.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="dd0ae-107">Ви можете включити або виключити об'єкти на основі доменів, OUs та інших атрибутів.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="dd0ae-108">[Синхронізація гешування паролів](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронізує хеш пароля з локального Active Directory на ЛАЗУРНЕ AD.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="dd0ae-109">Це дає змогу керувати паролем в одному розташуванні, але використовувати той самий пароль в локальних і хмарних середовищах.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="dd0ae-110">Оскільки служба Active Directory – це авторитетний джерело, ви можете використовувати власні політики паролів.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="dd0ae-111">Для [самостійного скидання пароля (sspr)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) користувачі можуть скинути власні паролі в хмарі, а також застосовувати локальну політику паролів.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="dd0ae-112">[Пристрій writback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) дає змогу реєструвати пристрої в AZURE AD, які повертаються в локальну службу Active Directory, щоб їх можна було використовувати для умовного доступу.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="dd0ae-113">[Запобігання випадковому вилученням](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) за замовчуванням для запобігання занадто багатьох одночасних видалень об'єктів (понад 500 об'єктів на синхронізацію).</span><span class="sxs-lookup"><span data-stu-id="dd0ae-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="dd0ae-114">Ви можете змінити цей параметр, щоб відповідно до потреб вашої організації.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="dd0ae-115">[Автоматичне оновлення](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) активовано за замовчуванням для Експрес-інсталяцій і допомагає забезпечити свою версію AZURE AD Connect завжди поточна.</span><span class="sxs-lookup"><span data-stu-id="dd0ae-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
