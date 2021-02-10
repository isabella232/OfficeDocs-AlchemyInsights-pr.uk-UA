---
title: Синхронізація хеш-пароля для служби domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177617"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="0cc26-102">Синхронізація хеш-пароля для служби domain</span><span class="sxs-lookup"><span data-stu-id="0cc26-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="0cc26-103">**Якщо у вашому екземплярі Azure AD DS з'являється запит на ввімкнення функції гешування паролів**</span><span class="sxs-lookup"><span data-stu-id="0cc26-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="0cc26-104">Ви зіткнулися з сценарієм, у якому ви працюєте з гібридним середовищем, щоб користувачі могли синхронізувати їх із локального середовища служб домену Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="0cc26-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="0cc26-105">Цей сценарій трапляється, незважаючи на те, що під час синхронізації пароля в локальній службі AD DS для свого клієнта Azure відображається синхронізація паролів.</span><span class="sxs-lookup"><span data-stu-id="0cc26-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="0cc26-106">**Спричиняють**</span><span class="sxs-lookup"><span data-stu-id="0cc26-106">**Cause**</span></span>

<span data-ttu-id="0cc26-107">Ця дія відбувається через те, що за замовчуванням для Azure AD Connect не синхронізуватиметься новий Диспетчер технологій LAN Manager (NTLM) і пароль протоколу Kerberos, необхідні для Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="0cc26-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="0cc26-108">**Спосіб вирішення**</span><span class="sxs-lookup"><span data-stu-id="0cc26-108">**Workaround**</span></span> 

<span data-ttu-id="0cc26-109">Щоб синхронізувати ці хеш-суми, необхідні для автентифікації NTLM та Kerberos, потрібно настроїти підключення Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0cc26-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="0cc26-110">Після настроювання служби Azure AD Connect, створення локального облікового запису або подія змінення пароля також синхронізує дані про застарілі паролі в лазуркому ОГОЛОШЕННІ.</span><span class="sxs-lookup"><span data-stu-id="0cc26-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="0cc26-111">Щоб отримати докладніші відомості про це та вказівки про те, як увімкнути синхронізацію паролів у гібридному середовищі Azure AD DS, ознайомтеся з наведеними [нижче](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) відомостями.</span><span class="sxs-lookup"><span data-stu-id="0cc26-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>