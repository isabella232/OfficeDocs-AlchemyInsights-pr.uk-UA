---
title: Чи ваші користувачі отримували зловмисні електронні листи
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815267"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="70a6a-102">Чи ваші користувачі отримували зловмисні електронні листи?</span><span class="sxs-lookup"><span data-stu-id="70a6a-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="70a6a-103">Тепер ви можете повідомити корпорації Майкрософт про зловмисні електронні листи за допомогою [надходжень від адміністратора в Центрі безпеки та відповідності](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="70a6a-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="70a6a-104">Повідомлення, надіслані до [надходжень від адміністратора](https://sip.protection.office.com/reportsubmission), скануються, і в спливаючому меню **відомостей** відображаються такі результати:</span><span class="sxs-lookup"><span data-stu-id="70a6a-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="70a6a-105">Чи сталася помилка автентифікації електронного листа відправника під час доставки.</span><span class="sxs-lookup"><span data-stu-id="70a6a-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="70a6a-106">Інформація про збіги з політиками, які могли вплинути на вердикт для повідомлення або перевизначити його.</span><span class="sxs-lookup"><span data-stu-id="70a6a-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="70a6a-107">Поточні результати знешкодження, які дають змогу побачити, чи URL-адреси або файли, які містить повідомлення, були зловмисними, чи ні.</span><span class="sxs-lookup"><span data-stu-id="70a6a-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="70a6a-108">Відгуки оцінювачів</span><span class="sxs-lookup"><span data-stu-id="70a6a-108">Feedback from graders</span></span>

<span data-ttu-id="70a6a-109">Якщо знайдено перевизначення, потрібно провести повторне сканування через кілька хвилин.</span><span class="sxs-lookup"><span data-stu-id="70a6a-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="70a6a-110">Якщо не виникало проблем з автентифікацією електронного листа і перевизначення не вплинуло на доставку, обробка відгуків оцінювачів може зайняти до одного дня.</span><span class="sxs-lookup"><span data-stu-id="70a6a-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="70a6a-111">Якщо ви не згідні з остаточним вердиктом для повідомлення, URL-адреси або файлу (заблоковано чи не заблоковано), надішліть повідомлення знову для повторного сканування через день.</span><span class="sxs-lookup"><span data-stu-id="70a6a-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="70a6a-112">Вірогідність того, що вердикт зміниться після повторного надсилання повідомлення, висока.</span><span class="sxs-lookup"><span data-stu-id="70a6a-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="70a6a-113">Тим часом, зловмисні електронні листи можна вилучити з поштових скриньок користувачів, дотримуючись вказівок із [цієї статті](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="70a6a-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="70a6a-114">Клієнти, у яких є Microsoft Defender для Office 365, можуть:</span><span class="sxs-lookup"><span data-stu-id="70a6a-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="70a6a-115">використовувати [Викривальник загроз для пошуку та видалення підозрілих електронних листів](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered);</span><span class="sxs-lookup"><span data-stu-id="70a6a-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="70a6a-116">[використовувати Безпеку посилань для блокування доступу](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) до зловмисних URL-адрес;</span><span class="sxs-lookup"><span data-stu-id="70a6a-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="70a6a-117">відстежувати користувачів, які клацнули зловмисні URL-адреси й отримали доступ до них: [Перегляд URL-адрес фішингу та клацання даних вердикту](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace);</span><span class="sxs-lookup"><span data-stu-id="70a6a-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="70a6a-118">уручну [запустити автоматичну перевірку](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).</span><span class="sxs-lookup"><span data-stu-id="70a6a-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="70a6a-119">Ви також можете захистити себе від зловмисних файлів і URL-адрес, дотримуючись вказівок зі статті [Захист від зловмисних URL-адрес і файлів](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="70a6a-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>