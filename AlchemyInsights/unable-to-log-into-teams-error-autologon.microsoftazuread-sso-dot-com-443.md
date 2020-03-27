---
title: Не вдається ввійти в Teams через помилку autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932284"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Не вдається ввійти в Teams через помилку autologon.microsoftazuread-sso dot com:443

Якщо як автентифікацію O365 увімкнуто функцію простого єдиного входу, можливо, до сайтів інтрамережі доведеться додати URL-адресу autologon.microsoftazuread-sso.com.  Якщо її вже додано до сайтів інтрамережі та використовується функція простого єдиного входу, вилучіть цю URL-адресу.

Ознайомтеся з [контрольним списком із виправлення помилок простого єдиного входу](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Щоб додати URL-адресу до списку сайтів інтрамережі, виконайте наведені нижче дії.

1. Відкрийте Internet Explorer, натиснувши кнопку **Пуск**. У полі пошуку введіть Internet Explorer, а потім у списку результатів виберіть **Internet Explorer**.
2. Виберіть **Знаряддя**, а потім – **Властивості браузера**.
3. Перейдіть на вкладку **Безпека**.
4. Виберіть **Локальна інтрамережа**, натисніть кнопку **Сайти**, а потім – **Додатково**.
5. Введіть URL-адресу веб-сайту та виберіть **Додати**.
6. Після завершення натисніть кнопку **Закрити**.

Щоб отримати докладні відомості, див. статтю [Документація з розгортання функції простого єдиного входу для O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (містить інформацію про процес на основі політик, за допомогою якого можна додати URL-адресу до сайтів інтрамереж на кроці 3).
