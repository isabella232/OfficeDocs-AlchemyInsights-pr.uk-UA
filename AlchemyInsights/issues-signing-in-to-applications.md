---
title: Проблеми з входом у програми
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901321"
---
# <a name="issues-signing-in-to-applications"></a>Проблеми з входом у програми

Щоб виявити причину або діагностику проблем, пов'язаних із входом користувача, виконайте наведені нижче дії.

1. Запустіть [діагностику для входу](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Знайти подію для аналізу, ввівши відомості про користувача, програму, час входу, ідентифікатор запиту або ідентифікатор кореляції.
3. Перегляньте результати діагностики, що містить відомості про те, що сталося, і які дії ви можете внести зміни, якщо необхідні зміни.

Нижче наведено кілька поширених проблем, які можуть виникнути під час входу в програму.

1. Ви або користувач **має завершити вхід у вигляді лазуровий, але відображається неочікувана Підказка** – перегляньте статті [несподівані згоди під час входу в програму](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) та [Несподівана помилка під час виконання згоди на програму](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Ви або користувач **ввійшли безпосередньо в програму, але не можете ввійти в нього з delelink на користувацькому порталі або на панелі Access**: перегляньте [Виправлення неполадок під час входу в програму з веб-програми Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Ви або користувач **завершили вхід у ЛАЗУРНЕ AD, але програма відобразить повідомлення про помилку, і не дозволяє користувачу завершити потік входу**: проблема полягає в тому, що програма не прийме відповідь, що видав Azure AD. Щоб виправити неполадку, виконайте наведені нижче [дії](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) .
4. Ви або користувач **не можете ввійти в програму, яка не є колекцією, настроєною для входу в один пароль**: дотримуйтеся вказівок, наведених у статті [, щоб виправити](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) неполадки.
5. Ви або користувач **не можете ввійти в програму Azure Gallery, настроєну для входу в один пароль**: виконайте наведені нижче [дії](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , щоб виправити неполадки.
6. Ви або користувач **не можете ввійти в програму Microsoft**: виконайте наведені нижче [дії](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) , щоб виправити неполадки.
7. Ви або користувач **не можете ввійти в програму, яка не належить до колекції, настроєна для інтегрованого компонента "єдиний вхід**": виконайте наведені нижче [дії](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) , щоб виправити неполадки.
8. Ви або користувач **не можете ввійти в програму Azure AD Gallery, настроєну для компонента "єдиний вхід**": виконайте наведені нижче [дії](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , щоб виправити неполадки.
9. Ви або користувач **не можете ввійти в спеціальну програму, що розробляється**: виконайте наведені нижче [дії](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , щоб виправити неполадки.
10. Ви або користувач **не можете ввійти в локальну програму за допомогою проксі-сервера програми Azure AD**: виконайте [наведені нижче дії](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) , щоб виправити неполадки.

