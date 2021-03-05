---
title: Синхронізація пароля
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483088"
---
# <a name="password-synchronization"></a><span data-ttu-id="83202-102">Синхронізація пароля</span><span class="sxs-lookup"><span data-stu-id="83202-102">Password synchronization</span></span>

<span data-ttu-id="83202-103">**Синхронізація гешування паролів не працює взагалі**</span><span class="sxs-lookup"><span data-stu-id="83202-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="83202-104">Деякі поширені проблеми, які можуть виникати, коли Синхронізація хеш-пароля не працює:</span><span class="sxs-lookup"><span data-stu-id="83202-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="83202-105">Обліковий запис Active Directory, який використовується для зв'язку з локальною службою Active Directory, не надається **Копіювати зміни в каталозі** та **Копіювати каталог змінює всі** дозволи, необхідні для синхронізації пароля – потрібно виправити це, надавши їм дозволи для облікового запису Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83202-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="83202-106">Синхронізація хеш-пароля вимкнута після того, як адміністратор змінював метод Sign-In користувача від **синхронізації пароля** до іншого параметра, наприклад **Федерації з AD FS** в майстрі "Лазурний", можна виправити це, повторно Увімкнувши функцію **синхронізації ПАРОЛЯ** в майстрі Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="83202-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="83202-107">Неполадка підключення з локальною службою Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83202-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="83202-108">Наприклад, деякі контролери доменів недоступні за допомогою служби Azure AD Connect, або [потрібні порти](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) блокуються брандмауером – це потрібно виправити, гарантуючи, що підключення між сервером Azure AD Connect і локальною службою Active Directory працює належним чином.</span><span class="sxs-lookup"><span data-stu-id="83202-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="83202-109">Сервер Azure AD Connect зараз перебуває в режимі постановки, що призведе до того, що сервер не зможе отримати хеш-значення, щоб усунути цю проблему, виконайте вказівки, описані в розділі [Виправлення неполадок під час синхронізації пароля в Azure AD Connect Sync – паролі не синхронізуються](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="83202-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="83202-110">**Синхронізація хеш-пароля не працює для деяких користувачів**</span><span class="sxs-lookup"><span data-stu-id="83202-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="83202-111">Якщо ви помітили, що хеш пароля не синхронізується з користувачем, за допомогою завдання **Виправлення неполадок** у ЛАЗУРНЕ AD Connect для дослідження та вирішення цієї проблеми.</span><span class="sxs-lookup"><span data-stu-id="83202-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="83202-112">Виконайте такі завдання:</span><span class="sxs-lookup"><span data-stu-id="83202-112">Perform the following tasks:</span></span>

    <span data-ttu-id="83202-113">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="83202-113">a.</span></span> [<span data-ttu-id="83202-114">Запуск завдання виправлення неполадок у майстрі</span><span class="sxs-lookup"><span data-stu-id="83202-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="83202-115">b.</span><span class="sxs-lookup"><span data-stu-id="83202-115">b.</span></span> [<span data-ttu-id="83202-116">Використання командлета "виправлення неполадок" для дослідження проблеми синхронізації хеш-пароля для певного використання</span><span class="sxs-lookup"><span data-stu-id="83202-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="83202-117">Для користувача, який використовується для локального користувача служби Active Directory, **користувач має змінити пароль під час наступної функції входу** .</span><span class="sxs-lookup"><span data-stu-id="83202-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="83202-118">Якщо цей параметр увімкнуто, користувачу призначається тимчасовий пароль, і буде запропоновано змінити пароль під час наступного входу.</span><span class="sxs-lookup"><span data-stu-id="83202-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="83202-119">Azure AD Connect не синхронізуватиме тимчасові паролі в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="83202-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="83202-120">Щоб вирішити цю проблему, виконайте одну з наведених нижче дій.</span><span class="sxs-lookup"><span data-stu-id="83202-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="83202-121">Попросіть користувача ввійти в локальну програму (наприклад, на комп'ютері з Windows) і змінити пароль.</span><span class="sxs-lookup"><span data-stu-id="83202-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="83202-122">Новий пароль буде синхронізовано з Azure AD.</span><span class="sxs-lookup"><span data-stu-id="83202-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="83202-123">Оновіть пароль користувача, не дозволяючи користувачу, який **має змінити пароль під час наступного входу**, а також надати спільний доступ до нового пароля користувачу.</span><span class="sxs-lookup"><span data-stu-id="83202-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="83202-124">Локальний об'єкт користувача служби Active Directory **не настроєно належним чином** для синхронізації об'єкта або синхронізації пароля.</span><span class="sxs-lookup"><span data-stu-id="83202-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="83202-125">Щоб вирішити цю проблему, виконайте вказівки, описані в статті [Виправлення неполадок із використанням гешування паролів за допомогою синхронізації Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="83202-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







