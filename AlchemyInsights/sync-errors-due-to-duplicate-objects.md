---
title: 902 (помилки синхронізації через повторювані об'єкти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708083"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="7f4de-102">Помилки синхронізації через повторювані об'єкти</span><span class="sxs-lookup"><span data-stu-id="7f4de-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="7f4de-103">Після завершення синхронізації служби каталогів у Microsoft 365 може з'явитися одне з таких повідомлень про помилку:</span><span class="sxs-lookup"><span data-stu-id="7f4de-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="7f4de-104">Не вдалося оновити цей об'єкт у службах Microsoft Online Services, оскільки наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які вже можуть бути пов'язані з іншим об'єктом у локальному каталозі.</span><span class="sxs-lookup"><span data-stu-id="7f4de-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="7f4de-105">Синхронізований об'єкт із тією самою адресою проксі-сервера, що вже існує в каталозі служб Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="7f4de-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="7f4de-106">Не вдалося оновити цей об'єкт, оскільки наведені нижче атрибути, пов'язані з цим об'єктом, мають значення, які вже можуть бути пов'язані з іншим об'єктом у службах локальної служби каталогів: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7f4de-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="7f4de-107">Щоб визначити та вирішити цю проблему, завантажте та запустіть [засіб виправлення помилок Idfix DirSync](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="7f4de-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="7f4de-108">Щоб отримати докладніші відомості, ознайомтеся з [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="7f4de-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
