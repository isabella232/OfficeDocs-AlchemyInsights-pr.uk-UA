---
title: ЗВД не працює належним чином
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507499"
---
# <a name="dlp-not-working-as-expected"></a>ЗВД не працює належним чином

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Налаштування ЗВД**

У вас виникли проблеми з **запобігання втрати даних (звд)** в Office 365 не працює належним чином? Якщо це так, переконайтеся, що ваша **політика звд** настроєно належним чином, і що дані, містить те, **що, якщо** вона шукає.
  
ЗВД правила дає змогу виявляти та захищати конфіденційну інформацію в організації. Щоб налаштувати ЗВД політики, скористайтеся інформацією [тут](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Що шукати ЗВД політики**
  
Під час використання **вбудованих типів конфіденційної інформації** в центрах безпеки та КОМПЛАЄНСУ, звд політики шукають конкретні візерунки та елементи під час виявлення цих чутливих типів.
  
- **Вбудовані типи конфіденційних даних**

    Відомості про вбудовані типи конфіденційних даних і те, що політика ЗВД шукає при виявленні чутливого типу, див.: [які типи конфіденційної інформації шукати](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Користувацькі типи конфіденційних відомостей**

    Якщо ви намагаєтесь створити спеціальні типи конфіденційних відомостей, використайте таку статтю, щоб отримати відомості про те, як створити користувацький чутливий тип: [створити користувацький тип конфіденційної інформації](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Перевірка ЗВД політика**

Щоб перевірити дані за допомогою вбудованого або настроюваного типу даних делікатного характеру, скористайтеся параметром **Test Type** **у розділі**  >  **типи конфіденційних**відомостей. Щоб [отримати додаткові відомості див.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Звіти**
  
- Отримуйте конфіденційні аналітичні дані за допомогою [звітів звд.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Ознайомтеся з конкретними відомостями про подію у [звіті про інцидент](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
