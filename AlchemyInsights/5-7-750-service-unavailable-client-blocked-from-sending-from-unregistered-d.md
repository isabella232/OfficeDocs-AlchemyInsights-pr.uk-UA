---
title: 1048 служба 5.7.750 недоступна. Клієнт заблоковано з надсилання незареєстрованих доменів
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676734"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="8ac26-103">5.7.750 клієнт заблокований від відправки з незареєстрованого домену</span><span class="sxs-lookup"><span data-stu-id="8ac26-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="8ac26-104">Помилка виникає, коли великий обсяг повідомлень надсилається з доменів, які не підготовлено до клієнта (Додано як допустимі домени та перевіряються).</span><span class="sxs-lookup"><span data-stu-id="8ac26-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="8ac26-105">Щоб уникнути цієї помилки, можна скористатися сертифікатом потоку пошти, на основі сертифіката, де домен, який ініціалізпідготовлено домену, або можна підготувати всі надсилання доменів.</span><span class="sxs-lookup"><span data-stu-id="8ac26-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
