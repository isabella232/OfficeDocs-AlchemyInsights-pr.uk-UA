---
title: Настроювання служби доменів
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885683"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Не вдається ввімкнути AAD-DS або розгортання не вдається

Щоб вирішити проблему, яка не активується (AAD-DS) не ввімкнуто або не вдається розгорнути, виконайте наведені нижче дії.

1. Якщо ви використовуєте вже наявну віртуальну мережу, перевірте свої правила, які блокують порти, необхідні для синхронізації в AAD-DS на порталі https://aka.ms/aadds-networking .
2. Перевірте, чи відповідь на повідомлення про помилку в цьому посібнику з виправлення неполадок, доступний у програмі  https://aka.ms/aadds-troubleshoot-enable .
3. У новій віртуальній мережі можна виконати розгортання служб для домену Azure AD.
4. Виконайте інструкції з початку роботи з розгортання AAD-DS: [створення та настроювання служб ДОМЕНУ aad](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Якщо у вас виникли проблеми з розгортанням служб домену Azure AD, перегляньте статтю [Виправлення неполадок служби "Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) " для вирішення поширених помилок, щоб допомогти вам знову працювати з ними. 

**Не вдається вимкнути AAD-DS**

AAD-DS не може бути призупинено. Якщо ви хочете припинити використовувати керований домен, його потрібно видалити.
Щоб видалити керований домен, ознайомтеся з елементом [Видалити службу доменів AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



