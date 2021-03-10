---
title: Виправлення неполадок із сертифікатом для підпису в SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694454"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Виправлення неполадок із сертифікатом для підпису в SAML

Щоб вирішити проблему сертифіката підпису, виконайте наведені нижче Рекомендовані дії.

1. Під час додавання корпоративної програми, яка підтримує SSO, Azure створить сертифікат, який називається [сертифікатом підпису SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Цей сертифікат має термін дії 3 роки. Щоб змінити дату завершення терміну дії сертифіката, перегляньте статтю [Настроювання дати завершення терміну дії сертифіката Федерації та прокрутіть його до нового сертифіката](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. За допомогою цього сертифіката буде використано цей сертифікат, щоб підписати маркери SAML, які просили програма, і відправить його до програми для успішного входу. Щоб виконати цю дію, завантажте сертифікат із порталу "Лазурний" та відправте його постачальнику програм, щоб завершити процес єдиного входу.

Після завершення цього процесу програма буде довіряти цьому сертифікату, і всі маркери SAML, підписані цим сертифікатом, прийматимуться програмою.

3. Якщо термін дії цього сертифіката завершився, створіть новий сертифікат, оновіть її до постачальника програм, а потім зробіть його активним на Лазурому боці. Щоб отримати додаткові відомості, перегляньте статтю [поновити сертифікат, який незабаром завершиться](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Якщо сертифікат завершується, користувач не заблокуватиметься.

4. [Додайте адресу електронної пошти для сповіщень](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , які потрібно отримати, перш ніж закінчиться термін дії поточного сертифіката.

> [!NOTE]
> Крок – 4 – необов'язковий.

5. Змінення параметрів підпису сертифіката в програмі SAML і алгоритм підпису сертифіката. Докладні відомості наведено в статті [змінення параметрів підпису сертифіката та алгоритму підпису](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

