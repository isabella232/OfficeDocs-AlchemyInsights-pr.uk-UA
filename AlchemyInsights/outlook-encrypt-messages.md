---
title: S/MIME у інтернет-версія Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010745"
---
# <a name="encrypt-email-messages-in-outlook"></a>Шифрування повідомлень електронної пошти у Outlook

Microsoft 365 Шифрування повідомлень побудовано на платформі Microsoft Azure Rights Management (Azure RMS), який входить до складу захисту даних в Azure. Якщо передплата включає Azure Rights Management або Захист даних в **Azure,** не потрібно виконувати жодних дій, щоб активувати або активувати службу керування правами вручну.

На основі відгуків клієнтів ми більше не вмикаємо правила Exchange пошти, щоб автоматично шифрувати вихідні повідомлення електронної пошти з певним типом чутливої інформації у вашому клієнті за замовчуванням. Натомість ми надамо докладні вказівки щодо того, як це зробити. Докладні відомості про те, як створити правило транспортування для шифрування особистих відомостей, див. [в цій статті.](https://aka.ms/OmeEtr)

- Якщо ви Outlook в Інтернеті (колишня частина **– OWA),** просто натисніть кнопку Захист у **веб-програмі** OWA. Після цього буде застосовано дозвіл "Не пересилати". Натисніть **кнопку Змінити дозвіл** і виберіть пункт **Шифрувати,** щоб зашифрувати повідомлення.

- Якщо використовується **клієнт Outlook:** щоб надіслати зашифроване повідомлення з програми Outlook 2013 чи 2016 або Outlook 2016 для Mac, виберіть Параметри Дозволи , а потім виберіть потрібний параметр  >  захисту.

- Щоб **автоматично шифрувати** всі електронні листи, надіслані певним одержувачам або зовнішнім партнерським організаціям, потрібно створити правило транспортування пошти Exchange адміністрування. Докладні вказівки наведено в [цій статті служби підтримки.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

