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
# <a name="configure-mim-sync-service"></a>Настроювання служби синхронізації МІМ

Служба синхронізації ідентифікації Microsoft (МІМ) – це компонент МІМ. Це централізоване локальна служба, яка зберігає та інтегрує інформацію для організацій, які мають кілька локальних каталогів і баз даних. Можливо, ви зможете вирішити проблему з синхронізацією МІМ, якщо проблему було розглянуто в недавньому оновленні до МІМ або є одним з інших проблем, наведених у розділі нижче.

**Рекомендовані дії**

1. Щоб визначити, чи вирішено проблему в оновленні, переконайтеся, що ви використовуєте останнє оновлення для МІМ-повідомлення, [а також перевірте](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , чи не усунено неполадку.
2. Якщо проблема пов'язана з загальним протоколом LDAP, загальним засобом SQL, Lotus Domino або веб-службами, переконайтеся, що ви використовуєте останнє оновлення [загальних сполучних ліній](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Якщо не вдається виконати синхронізацію МІМ-повідомлення з помилкою, зверніться до таблиці про [помилки](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) під час запуску, щоб визначити потенційні причини.
4. Якщо запуск припиняється з **розширенням-DLL-за винятком**, а потім клацніть ці слова, щоб відкрити вікно **властивостей сполучної лінії** , а потім натисніть кнопку **трасування стека...** , щоб переглянути докладні відомості про основну причину, як описано в [розширенні-DLL-виняток](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Якщо в журналі подій повідомлення про помилку, у якому **6025 сталася помилка** під час синхронізації пароля, у програмі [6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)Project
6. Якщо повна синхронізація з агентом керування службою FIM працює повільно, установіть прапорець **автоматично зростати** для бази даних TempDB, як описано в розділі [Виправлення неполадок із повільною або зависла повна синхронізація](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Якщо ви зустрічся з помилкою зупинити-сервер не вдалося-створення-через-веб-служби, використовуючи агент керування службою FIM, перегляньте статтю [support-info: Failed-Web-Services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) для огляду причин.

