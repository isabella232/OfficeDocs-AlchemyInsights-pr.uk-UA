---
title: Підтримка Microsoft EDGE для охоронця програм Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584006"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Підтримка Microsoft EDGE для охоронця програм Microsoft Defender

Для Windows 10 і Microsoft EDGE програма Guard використовує апаратно-ізольований підхід, який дає змогу користувачам переходити від ненадійного сайту в ізольованому, гіпер-V – контейнері, відокремленому від операційної системи хоста.

Адміністратор підприємства визначає список надійних веб-сайтів, хмарних ресурсів і внутрішніх мереж. Коли користувач відвідує сайт, який немає в списку, Microsoft EDGE відкриє сайт в контейнері. Це означає, що якщо сайт стане зловмисним, хост-ПК залишиться захищеним, а зловмисник не отримає корпоративні дані.

Інсталяція розширень у контейнері підтримується як Microsoft EDGE Version 81, і його можна керувати за допомогою політики. Адреса Updationeurl, що використовується в політиці розширення, має бути доданий як нейтральний ресурс у політиці мережної ізоляції, що використовується програмою "охоронець".

Докладні відомості наведено в статті [підтримка Microsoft EDGE для охоронця програм Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).
