---
title: Zarządzanie globalną listą adresową i książką adresową trybu offline w organizacji
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794842"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="8cdf9-102">Zarządzanie globalną listą adresową (GAL) i książką adresową trybu offline w organizacji (OAB)</span><span class="sxs-lookup"><span data-stu-id="8cdf9-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="8cdf9-103">Globalna lista adresowa (GAL) to lista wszystkich obiektów mogących otrzymywać wiadomości e-mail (odbiorcy dowolnego typu) w organizacji.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="8cdf9-104">Globalna lista adresowa (GAL) jest tworzona automatycznie w każdej organizacji.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="8cdf9-105">Możesz utworzyć dodatkowe globalne listy adresowe (GAL), aby podzielić użytkowników według organizacji lub lokalizacji, ale pojedynczy użytkownik może wyświetlać tylko jedną listę GAL i z niej korzystać.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="8cdf9-106">Niektóre klienty poczty elektronicznej, takie jak program Outlook dla systemu Windows, pobierają listę GAL do użytku w trybie offline.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="8cdf9-107">Jest to tzw. książka adresowa trybu offline (OAB).</span><span class="sxs-lookup"><span data-stu-id="8cdf9-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="8cdf9-108">W aplikacji Exchange online książka adresowa trybu offline (OAB) jest aktualizowana raz na osiem godzin, a później klienty muszą pobrać ją, aby zaktualizować swoja lokalną kopię OAB.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="8cdf9-109">Każda zmiana adresata musi najpierw pojawić się na liście GAL, aby mogła trafić do OAB.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="8cdf9-110">Poniżej podajemy kilka często wykorzystywanych procedur dotyczących GAL i OAB:</span><span class="sxs-lookup"><span data-stu-id="8cdf9-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="8cdf9-111">Z różnych powodów możesz chcieć, aby niektóre obiekty były ukryte na liście GAL.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="8cdf9-112">Zobacz [Ukrywanie adresatów na liście adresów](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="8cdf9-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="8cdf9-113">Jeżeli chcesz umożliwić określonym grupom użytkowników korzystanie z niestandardowego widoku globalnej listy adresowej (GAL) organizacji, zobacz [Zasady dotyczące książki adresowej w aplikacji Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="8cdf9-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="8cdf9-114">[Aby stworzyć globalną listę adresową w aplikacji Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) i nauczyć się, jak korzystać z uprawnień GAL, zobacz [Listy adresowe w aplikacji Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="8cdf9-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="8cdf9-115">Pamiętaj, że jeżeli tworzysz nową globalną listę adresową GAL, możesz również zechcieć stworzyć nową książkę adresową trybu offline (OAB).</span><span class="sxs-lookup"><span data-stu-id="8cdf9-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="8cdf9-116">Zobacz [Procedury dotyczące książki adresowej trybu offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="8cdf9-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
