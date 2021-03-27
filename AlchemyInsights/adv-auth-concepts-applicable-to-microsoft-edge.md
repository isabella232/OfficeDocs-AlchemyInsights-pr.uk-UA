---
title: Поняття розширеної автентифікації, що застосовуються до Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398606"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="02962-102">Поняття розширеної автентифікації, що застосовуються до Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="02962-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="02962-103">Нижче наведено поняття розширеної автентифікації, які застосовуються до Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="02962-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="02962-104">**Proactive Authentication**</span><span class="sxs-lookup"><span data-stu-id="02962-104">**Proactive Authentication**</span></span>

<span data-ttu-id="02962-105">Якщо ввімкнути політику [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge спробує завибачливо автентифікувати користувачів, які ввійшли в службу Microsoft.</span><span class="sxs-lookup"><span data-stu-id="02962-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="02962-106">Через регулярні проміжки часу вона використовуватиме онлайнову службу, щоб перевіряти наявність оновлених маніфестів, які містять конфігурацію, що регулює proactive Authentication (Проактивна автентифікація).</span><span class="sxs-lookup"><span data-stu-id="02962-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="02962-107">Переваги. Завбачлива автентифікація активує автентифікацію для ключових служб, таких як сторінка Office New Tab Page (Нова вкладка Office).</span><span class="sxs-lookup"><span data-stu-id="02962-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="02962-108">Крім того, якщо Bing використовується як пошуковий система, Proactive Authentication покращує продуктивність рядка адреси та допомагає генерувати результати пошуку, персоналізовані за потреби компанії.</span><span class="sxs-lookup"><span data-stu-id="02962-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="02962-109">**Автентифікація Windows Hello CredUI для автентифікації NTLM**</span><span class="sxs-lookup"><span data-stu-id="02962-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="02962-110">Якщо єдиний вхід (SSO) недоступний, якщо веб-сайт намагається ввійти в користувача через механізм NTLM або вести переговори, ця функція дасть змогу користувачу надати доступ до облікових даних ОС із веб-сайту та задовольнити проблему автентифікації за допомогою інтерфейсу користувача Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="02962-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="02962-111">Цей процес входу відображатиметься лише у Windows 10 і лише для користувачів, які не отримують єдиного входу під час NTLM або домовленості.</span><span class="sxs-lookup"><span data-stu-id="02962-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="02962-112">**Використання збережених паролів для автоматичного входу**</span><span class="sxs-lookup"><span data-stu-id="02962-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="02962-113">Користувачі, які зберігають паролі в Microsoft Edge, можуть активувати автоматичний вхід на веб-сайти, на яких збережено облікові дані.</span><span class="sxs-lookup"><span data-stu-id="02962-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="02962-114">Користувачі можуть увімкнути або вимкнути цю функцію в edge://settings/passwords, а також налаштувати її в [політиках диспетчера паролів.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="02962-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
