---
title: Увімкнути зворотний запис пароля в Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560461"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="067b9-102">Увімкнути зворотний запис пароля в Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="067b9-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="067b9-103">Щоб увімкнути самостійний зворотний запис пароля, спочатку ввімкніть параметр зворотного запису в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="067b9-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="067b9-104">Виконайте наведені далі кроки на сервері Azure AD Connect:</span><span class="sxs-lookup"><span data-stu-id="067b9-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="067b9-105">Увійдіть на свій сервер Azure AD Connect і запустіть майстер налаштування **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="067b9-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="067b9-106">На сторінці **привітання** натисніть кнопку **Налаштувати**.</span><span class="sxs-lookup"><span data-stu-id="067b9-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="067b9-107">На сторінці **Додаткові завдання** виберіть **Налаштувати параметри синхронізації**, а потім натисніть **Далі**.</span><span class="sxs-lookup"><span data-stu-id="067b9-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="067b9-108">На сторінці **Підключення до Azure AD** введіть облікові дані адміністратора для свого осередку Azure, а потім натисніть **Далі**.</span><span class="sxs-lookup"><span data-stu-id="067b9-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="067b9-109">На сторінках фільтрування **Підключення каталогів** і **Domain/OU**, натисніть **Далі**.</span><span class="sxs-lookup"><span data-stu-id="067b9-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="067b9-110">На сторінці **Додаткові функції** установіть прапорець **Зворотний запис пароля** та натисніть **Далі**.</span><span class="sxs-lookup"><span data-stu-id="067b9-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="067b9-111">На сторінці **Готово до налаштування** натисніть **Налаштувати** та дочекайтеся на завершення процесу.</span><span class="sxs-lookup"><span data-stu-id="067b9-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="067b9-112">Коли налаштування завершиться, натисніть **Вийти**.</span><span class="sxs-lookup"><span data-stu-id="067b9-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="067b9-113">Коли зворотний запис пароля ввімкнуто в Azure AD Connect, налаштуйте зворотний запис у самостійному скиданні пароля Azure AD.</span><span class="sxs-lookup"><span data-stu-id="067b9-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="067b9-114">Щоб увімкнути зворотний запис для самостійного скидання пароля, виконайте наведені далі кроки:</span><span class="sxs-lookup"><span data-stu-id="067b9-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="067b9-115">Увійдіть на портал Azure за допомогою облікового запису адміністратора.</span><span class="sxs-lookup"><span data-stu-id="067b9-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="067b9-116">Знайдіть і виберіть **Azure Active Directory**, натисніть **Скидання пароля**, а потім – **Локальна інтеграція**.</span><span class="sxs-lookup"><span data-stu-id="067b9-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="067b9-117">Установіть для параметра **Виконувати зворотний запис до локального каталогу?** значення **Так**.</span><span class="sxs-lookup"><span data-stu-id="067b9-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="067b9-118">Установіть для параметра **Дозволяти користувачам розблоковувати облікові записи без скидання пароля?** значення **Так**.</span><span class="sxs-lookup"><span data-stu-id="067b9-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="067b9-119">Завершивши, натисніть кнопку **Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="067b9-119">When ready, click **Save**.</span></span>

<span data-ttu-id="067b9-120">Докладні відомості наведено в статті [Увімкнення зворотного запису для самостійного скидання пароля в Enable Azure Active Directory в локальному середовищі](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="067b9-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="067b9-121">Коли адміністратор скидає на порталі Azure пароль федеративного користувача або пароль із синхронізованим гешем, цей пароль записується локально.</span><span class="sxs-lookup"><span data-stu-id="067b9-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="067b9-122">Цей функціонал зараз не підтримується на порталі адміністрування Office.</span><span class="sxs-lookup"><span data-stu-id="067b9-122">This functionality is currently not supported in the Office Admin portal.</span></span>