---
title: Настроювання служби синхронізації МІМ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482893"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="4e6bd-102">Настроювання служби синхронізації МІМ</span><span class="sxs-lookup"><span data-stu-id="4e6bd-102">Configure MIM Sync service</span></span>

<span data-ttu-id="4e6bd-103">Служба синхронізації ідентифікації Microsoft (МІМ) – це компонент МІМ.</span><span class="sxs-lookup"><span data-stu-id="4e6bd-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="4e6bd-104">Це централізоване локальна служба, яка зберігає та інтегрує інформацію для організацій, які мають кілька локальних каталогів і баз даних.</span><span class="sxs-lookup"><span data-stu-id="4e6bd-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="4e6bd-105">Можливо, ви зможете вирішити проблему з синхронізацією МІМ, якщо проблему було розглянуто в недавньому оновленні до МІМ або є одним з інших проблем, наведених у розділі нижче.</span><span class="sxs-lookup"><span data-stu-id="4e6bd-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="4e6bd-106">**Рекомендовані дії**</span><span class="sxs-lookup"><span data-stu-id="4e6bd-106">**Recommended steps**</span></span>

1. <span data-ttu-id="4e6bd-107">Щоб визначити, чи вирішено проблему в оновленні, переконайтеся, що ви використовуєте останнє оновлення для МІМ-повідомлення, [а також перевірте](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , чи не усунено неполадку.</span><span class="sxs-lookup"><span data-stu-id="4e6bd-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="4e6bd-108">Якщо проблема пов'язана з загальним протоколом LDAP, загальним засобом SQL, Lotus Domino або веб-службами, переконайтеся, що ви використовуєте останнє оновлення [загальних сполучних ліній](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="4e6bd-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="4e6bd-109">Якщо не вдається виконати синхронізацію МІМ-повідомлення з помилкою, зверніться до таблиці про [помилки](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) під час запуску, щоб визначити потенційні причини.</span><span class="sxs-lookup"><span data-stu-id="4e6bd-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="4e6bd-110">Якщо запуск припиняється з **розширенням-DLL-за винятком**, а потім клацніть ці слова, щоб відкрити вікно **властивостей сполучної лінії** , а потім натисніть кнопку **трасування стека...** , щоб переглянути докладні відомості про основну причину, як описано в [розширенні-DLL-виняток](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="4e6bd-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="4e6bd-111">Якщо в журналі подій повідомлення про помилку, у якому **6025 сталася помилка** під час синхронізації пароля, у програмі [6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)Project</span><span class="sxs-lookup"><span data-stu-id="4e6bd-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="4e6bd-112">Якщо повна синхронізація з агентом керування службою FIM працює повільно, установіть прапорець **автоматично зростати** для бази даних TempDB, як описано в розділі [Виправлення неполадок із повільною або зависла повна синхронізація](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="4e6bd-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="4e6bd-113">Якщо ви зустрічся з помилкою зупинити-сервер не вдалося-створення-через-веб-служби, використовуючи агент керування службою FIM, перегляньте статтю [support-info: Failed-Web-Services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) для огляду причин.</span><span class="sxs-lookup"><span data-stu-id="4e6bd-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

