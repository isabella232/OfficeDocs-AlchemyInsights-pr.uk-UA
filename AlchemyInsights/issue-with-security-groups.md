---
title: Проблема з групами безпеки
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177637"
---
# <a name="issue-with-security-groups"></a>Проблема з групами безпеки

**Якщо ви одержуєте помилки в мережі AADDS104**

Неприпустимі правила групи безпеки мережі – це найпоширеніша причина помилок мережі для служб домену Azure Active Directory (AD DS). Група безпеки мережі для віртуальної мережі має дозволити доступ до певних портів і протоколів. Якщо ці порти блокуються, платформа Azure не може відстежувати або оновлювати керований домен. Це також впливає на синхронізацію між Лазуроним оголошенням і Лазуроним ОГОЛОШЕННЯМ DS. Переконайтеся, що ви зберігаєте відкриті порти за замовчуванням, щоб уникнути переривання обслуговування.

Щоб зрозуміти та вирішити поширені проблеми з конфігурацією мережної системи безпеки, перегляньте статтю [Додавання та перевірка груп безпеки](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
