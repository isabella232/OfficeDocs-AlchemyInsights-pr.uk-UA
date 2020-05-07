---
title: Керування глобальним списком адрес і автономною адресною книгою організації
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022668"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="b9611-102">Керування глобальним списком адрес (GAL) і автономною адресною книгою (OAB) організації</span><span class="sxs-lookup"><span data-stu-id="b9611-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="b9611-103">Глобальний список адрес (GAL) – це список об'єктів із підтримкою пошти (усі типи одержувачів, які можуть отримувати електронні листи) в організації.</span><span class="sxs-lookup"><span data-stu-id="b9611-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="b9611-104">У кожній організації автоматично створюється один список GAL.</span><span class="sxs-lookup"><span data-stu-id="b9611-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="b9611-105">Ви можете створити додаткові списки GAL, щоб розділити користувачів за організацією або розташуванням, але один користувач може бачити й використовувати лише один список одночасно.</span><span class="sxs-lookup"><span data-stu-id="b9611-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="b9611-106">У деяких клієнтах електронної пошти, як-от Outlook для Windows, можна завантажити GAL для автономного використання.</span><span class="sxs-lookup"><span data-stu-id="b9611-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="b9611-107">Така версія відома як автономна адресна книга (OAB).</span><span class="sxs-lookup"><span data-stu-id="b9611-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="b9611-108">В Exchange Online автономна адресна книга оновлюється лише раз на 8 годин, а потім клієнти мають завантажити її, щоб оновити локальну копію OAB.</span><span class="sxs-lookup"><span data-stu-id="b9611-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="b9611-109">Будь-яка зміна одержувачів спочатку відображається в GAL, а пізніше вноситься до OAB.</span><span class="sxs-lookup"><span data-stu-id="b9611-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="b9611-110">Нижче наведено деякі поширені процедури для GAL і OAB.</span><span class="sxs-lookup"><span data-stu-id="b9611-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="b9611-111">З багатьох причин вам може знадобитися приховати деякі об'єкти в GAL.</span><span class="sxs-lookup"><span data-stu-id="b9611-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="b9611-112">Див. статтю [Приховування одержувачів у списках адрес](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="b9611-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="b9611-113">Щоб надати певним групам користувачів настроювані подання GAL організації, див. статтю [Політики адресної книги в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="b9611-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="b9611-114">Відомості про [створення глобального списку адрес в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) і використання дозволів GAL див. в статті [Списки адрес в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="b9611-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="b9611-115">Зверніть увагу, що створивши нові списки GAL, ви, можливо, також захочете створити нову автономну адресну книгу.</span><span class="sxs-lookup"><span data-stu-id="b9611-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="b9611-116">Див. статтю [Процедури для автономної адресної книги](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="b9611-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
