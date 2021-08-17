---
title: DLP не працює належним чином
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079723"
---
# <a name="dlp-not-working-as-expected"></a>DLP не працює належним чином

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Налаштування DLP**

Виникли проблеми із захистом від втрати даних **(DLP)** Office 365 не працює належним чином? Якщо так, переконайтеся, що політику **DLP** налаштовано правильно, і що в даних міститься потрібна політика **DLP** під час її оцінювання.
  
Політики захисту від захисту від даних дасть змогу визначати й захищати в організації особисті відомості. Щоб налаштувати політики DLP, скористайтеся відомостями [тут.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Які політики DLP шукають?**
  
Якщо використовується вбудовані типи відомостей у Центрах безпеки та відповідності, політики DLP виявляються певними шаблонами й елементами, коли виявляються такі типи. 
  
- **Вбудовані типи відомостей**

    Відомості про вбудовані типи й типи даних, які виявляє політика DLP, див. в [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)цьому політиці.

- **Настроювані типи відомостей, що чутливі**

    Якщо ви намагаєтеся створити настроювані типи особистих відомостей, відомості про створення спеціального типу враховуються в цій [статті:](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)Створення спеціального типу особистих відомостей.

**Перевірка політики DLP**

Щоб перевірити дані за допомогою вбудованого або настроюваного типу,  скористайтеся параметром Тип перевірки в розділі Класифікації.  >   Докладні відомості див. в [довідці з перевірки спеціальних типів чутливих відомостей.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Звіти**
  
- Отримуйте хибні дані за допомогою звітів [DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Докладні відомості про подію див. у звіті про [інцидент.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
