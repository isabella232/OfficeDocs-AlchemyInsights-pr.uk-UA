---
title: Можливо, вам знадобиться спеціальний тип даних
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446712"
---
# <a name="dlp-might-need-a-custom-type"></a>Можливо, вам знадобиться спеціальний тип даних

**Важливо**: у ці безпрецедентні часи ми докладаємо всіх зусиль до того, щоб служби SharePoint Online і OneDrive були завжди доступні. Докладні відомості надано у статті [Тимчасові коригування функцій SharePoint Online](https://aka.ms/ODSPAdjustments).

**Для зв'яжіться з інформацією, можливо, знадобитися настроюваний тип даних**

Політику захисту від втрати даних (DLP) можна визначати й захищати в організації. У деяких випадках може знадобитися створити власний настроюваний тип чутливої інформації, щоб захистити дані організації. Докладні відомості див. [в](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) цих відомостях. [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Докладні відомості про створення настроюваних типів і політик конфіденційності див. в статтях: 

**Настроювання вбудованого типу чутливих відомостей**

Відомості про те, як налаштувати вбудований тип чутливої інформації, можна знайти в розділі Настроювання вбудованого типу [відомостей.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Наприклад, можна додати або видалити ключові слова, а також додати або видалити допоміжні допоміжні докази, наприклад дату чи адресу.

**Створення спеціального типу чутливої інформації**

Але якщо потрібно знайти й захистити інший тип чутливих відомостей, можна створити настроюваний тип в області Центр відповідності Microsoft 365. Докладні відомості див. в [цьому письмовій інформації.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Створення настроюваного типу в центрі безпеки & відповідності PowerShell**

Нарешті, якщо в інтерфейсі користувача не надано всі необхідні параметри, можна створити настроюваний тип непотребної інформації в Центрі безпеки & відповідності PowerShell. Починаючи з файлу XML, можна використовувати всі доступні параметри. Докладні відомості див. в відомості про створення спеціального [типу особистих відомостей за допомогою PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Щоб спочатку перевірити політику в [](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) режимі тестування, див. номери Реалізація політики в режимі тестування та Створення, тестування та настроювання [політики DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 