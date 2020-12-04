---
title: Розширені концепції автентифікації, застосовні до Microsoft EDGE
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573781"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="9daac-102">Розширені концепції автентифікації, застосовні до Microsoft EDGE</span><span class="sxs-lookup"><span data-stu-id="9daac-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="9daac-103">Нижче наведено додаткові концепції автентифікації, застосовні до Microsoft EDGE:</span><span class="sxs-lookup"><span data-stu-id="9daac-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="9daac-104">**Активна автентифікація**</span><span class="sxs-lookup"><span data-stu-id="9daac-104">**Proactive Authentication**</span></span>

<span data-ttu-id="9daac-105">Коли ви активували політику [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft EDGE спробує автентифікувати користувачів, підписані користувачами через служби Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9daac-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="9daac-106">Через певні проміжки часу вона використовуватиме онлайнову службу, щоб перевірити наявність оновленого Маніфесту, що містить конфігурацію, що регулює активну автентифікацію.</span><span class="sxs-lookup"><span data-stu-id="9daac-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="9daac-107">Переваги: активна автентифікація дає можливість автентифікації на ключові служби, наприклад на сторінці "Нова вкладка Office".</span><span class="sxs-lookup"><span data-stu-id="9daac-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="9daac-108">Крім того, якщо використовується Бінг в якості пошукової системи, функція активної автентифікації покращує продуктивність рядка адреси та допомагає генерувати результати пошуку персоналізованої для потреб вашого бізнесу.</span><span class="sxs-lookup"><span data-stu-id="9daac-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="9daac-109">**Windows Hello CredUI для автентифікації NTLM**</span><span class="sxs-lookup"><span data-stu-id="9daac-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="9daac-110">Якщо єдиний вхід (SSO) недоступний, коли веб-сайт спробує ввійти на користувача через механізм NTLM або домовитися, ця функція дозволить користувачу надавати спільний доступ до облікових даних ОС із веб-сайтом і відповідно до завдання автентифікації за допомогою інтерфейсу користувача Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="9daac-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="9daac-111">Цей потік входу відображатиметься лише в ОС Windows 10, і лише для користувачів, які не отримують єдиного входу під час виклику NTLM або завдання під час переговорів.</span><span class="sxs-lookup"><span data-stu-id="9daac-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="9daac-112">**Використання збережених паролів для автоматичного входу**</span><span class="sxs-lookup"><span data-stu-id="9daac-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="9daac-113">Користувачі, які зберігають паролі в Microsoft EDGE, можуть увімкнути автоматичний вхід на веб-сайти, де зберігаються облікові дані.</span><span class="sxs-lookup"><span data-stu-id="9daac-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="9daac-114">Користувачі можуть ввімкнути або вимкнути цю функцію в edge://settings/passwords, а також настроїти його в політиці [диспетчера паролів](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="9daac-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
