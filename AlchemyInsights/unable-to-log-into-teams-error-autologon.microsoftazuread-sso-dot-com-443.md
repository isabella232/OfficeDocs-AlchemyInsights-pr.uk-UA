---
title: Не вдається ввійти в Teams через помилку autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038421"
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
