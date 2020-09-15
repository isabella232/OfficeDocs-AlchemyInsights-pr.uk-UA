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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679714"
---
# <a name="dlp-not-working-as-expected"></a>DLP не працює належним чином

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Налаштування DLP**

У вас виникли проблеми з **запобіганням втрати даних (DLP)** у службі Office 365, які не працюють належним чином? Якщо так, переконайтеся, що **політику DLP** настроєно правильно, і дані, що містяться в **політиці DLP** , шукають, коли її буде оцінено.
  
Політики DLP дають змогу виявляти та захищати конфіденційну інформацію в організації. Щоб налаштувати політики DLP, скористайтеся інформацією [тут](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Що таке політики DLP, які шукають**
  
Під час використання **вбудованих типів даних** у центрах безпеки та відповідності, політики DLP шукають певні структури та елементи під час виявлення цих чутливих типів.
  
- **Вбудовані типи конфіденційної інформації**

    Щоб отримати відомості про вбудовані типи, а також про те, що таке політика DLP, під час виявлення чутливим типом, ознайомтеся з відомостями про [типи чутливих даних](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Спеціальні типи конфіденційної інформації**

    Якщо ви намагаєтеся створити спеціальні конфіденційні типи даних, скористайтеся наведенною нижче статтею, щоб отримати відомості про те, як створити настроюваний чутливий тип: [створити настроюваний тип конфіденційної інформації](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Перевірка політики DLP**

Щоб перевірити дані з вбудованим або настроюваним типом конфіденційної інформації, скористайтеся параметром **тип тесту** в розділі **класифікації**  >  **конфіденційних відомостей про типи**даних. Докладні відомості наведено в статті [перевірка користувацьких чутливих типів даних](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Звіти**
  
- Отримуйте чутливі дані про результати пошуку за допомогою [звітів DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Перегляньте докладні відомості про подію з [звітом про інцидент](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
