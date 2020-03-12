---
title: Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600389"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="83665-102">Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="83665-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="83665-103">W wyniku nowej i ulepszonej funkcji zbierania elektronicznych materiałów dowodowych w centrum zgodności usługi Microsoft 365 w nadchodzących miesiącach zostaną wycofane następujące starsze narzędzia i polecenia zbierania elektronicznych materiałów dowodowych:</span><span class="sxs-lookup"><span data-stu-id="83665-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="83665-104">[W miejscu zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [blokad miejscowych](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="83665-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="83665-105">Polecenia cmdlet programu Exchange Online programu PowerShell obsługujące zbieranie elektronicznych materiałów dowodowych i blokady miejscowe.</span><span class="sxs-lookup"><span data-stu-id="83665-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="83665-106">(Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet \*-MailboxSearch). Obejmuje to następujące polecenia cmdlet:</span><span class="sxs-lookup"><span data-stu-id="83665-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="83665-107">Wyszukiwanie skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="83665-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="83665-108">Wyszukiwanie skrzynki pocztowej start</span><span class="sxs-lookup"><span data-stu-id="83665-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="83665-109">Wyszukiwanie skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="83665-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="83665-110">Wyszukiwanie skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="83665-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="83665-111">Polecenie cmdlet [Skrzynki wyszukiwania](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="83665-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="83665-112">Następujące operacje w interfejsie API usług sieci Web programu Exchange:</span><span class="sxs-lookup"><span data-stu-id="83665-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="83665-113">GetSearchableSkrzynki pocztowe</span><span class="sxs-lookup"><span data-stu-id="83665-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="83665-114">SetHoldOnSkrzynki pocztowe</span><span class="sxs-lookup"><span data-stu-id="83665-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="83665-115">Skrzynki pocztowe GetHoldOn</span><span class="sxs-lookup"><span data-stu-id="83665-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="83665-116">Zaawansowane zbieranie elektronicznych materiałów dowodowych usługi Office 365 w 1.0</span><span class="sxs-lookup"><span data-stu-id="83665-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="83665-117">**Harmonogram przejścia na emeryturę**:</span><span class="sxs-lookup"><span data-stu-id="83665-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="83665-118">Kwiecień 1, 2020: Nie będziesz mógł tworzyć nowych wyszukiwań i blokad, ale nadal możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko.</span><span class="sxs-lookup"><span data-stu-id="83665-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="83665-119">Pomoc techniczna firmy Microsoft nie będzie już obsługiwać zbierania elektronicznych materiałów dowodowych & w witrynie EAC.</span><span class="sxs-lookup"><span data-stu-id="83665-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="83665-120">1 lipca 2020 r.: Funkcja zbierania elektronicznych materiałów dowodowych & w trybie EAC zostanie umieszczona w trybie tylko do odczytu.</span><span class="sxs-lookup"><span data-stu-id="83665-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="83665-121">Oznacza to, że możesz usuwać tylko istniejące wyszukiwania i blokady.</span><span class="sxs-lookup"><span data-stu-id="83665-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="83665-122">**Aby uzyskać więcej informacji, zobacz:**</span><span class="sxs-lookup"><span data-stu-id="83665-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="83665-123">Migrowanie starszych wyszukiwań zbierania elektronicznych materiałów dowodowych i blokad do centrum zgodności usługi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="83665-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="83665-124">Wycofywanie starszych narzędzi zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="83665-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="83665-125">Często zadawane pytania dotyczące zbierania elektronicznych materiałów dowodowych i blokad w miejscu</span><span class="sxs-lookup"><span data-stu-id="83665-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



