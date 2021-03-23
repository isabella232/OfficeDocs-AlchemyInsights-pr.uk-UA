---
title: У мене заблоковано умовний доступ до пристрою, до якого приєднується домен
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038107"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>У мене заблоковано умовний доступ до пристрою, до якого приєднується домен

**Високорекомендовані інструменти**

Засіб [вирішення проблем із реєстрацією пристроїв](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – засіб, який допомагає у виправленні неполадок із найпоширенішим питанням реєстрації пристроїв.

[Сценарій підключення пристрою для тестування](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : сценарій, який допомагає забезпечити, щоб пристрій міг отримати доступ до кінцевих точок реєстрації пристрою в системному обліковому записі.

[Скрипт очищення пристрою в Лазур](https://github.com/mzmaili/AzureADDeviceCleanup) – скрипт, який дає змогу шукати та керувати застарілою пристроями в навколишньому середовищі.

Нижче наведено кілька типових причин, через які умовний доступ може не працювати з пристроєм, який приєднався до домену (гібридне блакитне AD).

1. **На пристрої немає лазуроної реклами** – потрібно переконатися, що на пристрої є маркер первинного оновлення «AZURE AD» (PRT). Щоб отримати докладніші відомості про PRT, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Щоб перевірити, чи є у вас блакитний AD PRT, ви можете запустити `dsregcmd/status` команду на пристрої та перевірити, чи "AzureAdPrt" дорівнює "так".

Якщо "AzureAdPrt" є "ні", перевірте таке:

- **Незалежно від того, чи є у вас федеративне середовище з AD FS, і вона недоступна в домашніх мережах користувачів**: у цьому випадку переконайтеся, що кінцеві точки usernamemed доступні в мережі екстранет. Якщо ваше AD FS знаходиться позаду віртуальної приватної мережі, переконайтеся, що користувачі підключаються до мережі VPN і повторно Увійдіть на пристрій. Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Незалежно від того, що TPM пристрою несправний, і таким чином не можна автентифікувати пристрій**: установіть прапорець "TPM. msc", щоб дізнатися, чи стан модуля TPM "Готово". Якщо це не так, запустіть `dsregcmd/leave` і дайте пристрою повторно приєднатися до Azure AD. Потім повторіть спробу. Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Ви використовуєте постачальника посвідчень 3rd Party, який не підтримує протокол WS-Trust**. Як описано в наших документах, у цьому випадку не можна працювати з гібридним пристроями, підключеному до AD-пристроїв. Ви можете працювати з постачальником посвідчень для підтримки.

2. **Користувачі, які використовують браузер Chrome без облікових записів Windows 10** або розширення Office, не можуть **автоматично використовувати ГВП на пристроях aad, підключених до мережі або гібридних-aad**. це призводить до провалу будь-яких політик умовного доступу на основі пристрою, у якому відображається повідомлення про помилку "незареєстрований пристрій". Щоб правильно використовувати браузер Chrome, потрібно інсталювати "облікові записи Windows 10" або "розширення Office до браузера Chrome" за допомогою SCCM або Inune. Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Якщо ви не можете натиснути розширення віддалено, повідомте користувачів, щоб вручну інсталювати один із наведених вище розширень, щоб отримати доступ до програм за допомогою умовного доступу на основі пристрою. Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Пристрій був належним чином видалений, але його було видалено або вимкнуто через синхронізацію в AZURE AD Connect або на порталі Azure**: якщо це станеться, об'єкт пристрою більше не розпізнається як повністю підключений пристрій, хоча стан "AzureAdJoined" і "PRT" відображається як дійсний на пристрої.

Щоб вирішити цю проблему, запустіть `dsregcmd/leave` їх на уражених пристроях і дайте їм змогу повторно приєднатися до "Azure AD". Щоб отримати докладніші відомості, перегляньте цей [документ](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Якщо ваші пристрої знаходяться в ОС Windows 10, 1809 Update, з проксі-сервером VPN/Cloud і в разі виникнення проблем із "AzureAdPrt" або будь-якою програмою з помилкою єдиного входу (програма Outlook не підключається до поштової скриньки, навіть якщо у вас є PRT), переконайтеся, що ви маєте цей патч [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) або квітня накопичувальне оновлення [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , щоб запобігти появі збоїв ГВП на цих машинах

















