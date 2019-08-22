---
title: DLP не працює належним чином
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530321"
---
# <a name="dlp-not-working-as-expected"></a>DLP не працює належним чином

Виникли проблеми із **Запобігання втрати даних (DLP)** у службі Office 365, не працює належним чином? Якщо це так, переконайтеся, що ваш **DLP політики** налаштовано правильно, і що дані містять що **DLP політики** є шукає, коли вона виконується оцінка.
  
 **Настроювання DLP**
  
DLP політики дає змогу визначити та захисту конфіденційної інформації в організації. Щоб налаштувати DLP політики, використовувати інформацію [тут](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Що шукати DLP політики**
  
При використанні **типи вбудованих конфіденційну інформацію** в Office 365 Безпека та відповідність вимогам центр, DLP політики Шукайте конкретні моделі та елементів при виявленні таких чутливих типів.
  
- **Типи вбудованих конфіденційної інформації**

    Докладніше про вбудованих чутливих типів і те, що політика DLP шукає при виявленні чутливі типу, дивіться: [шукати того, що вводить конфіденційну інформацію](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Типи настроюваних конфіденційної інформації**

    Якщо ви маєте намір створити настроювані конфіденційну інформацію типів, використовувати наступну статтю відомості про те, як створити користувальницький чутливі тип: [Створити тип настроюваного конфіденційну інформацію](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Перевірити DLP політики**

Перевірити ваші дані за допомогою вбудованих і настроюваних конфіденційної інформації типу, скористайтеся параметром **перевірити тип** під **класифікацій** > **типи конфіденційну інформацію**. Докладніше перегляньте [тест типи настроюваних конфіденційну інформацію](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Звіти**
  
- Отримати конфіденційні дані insights з [звіти DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Переглянути конкретні деталі заходу з [Звіт про інцидент](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
