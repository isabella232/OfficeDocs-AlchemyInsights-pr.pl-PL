---
title: Wycofanie starszych wersji narzędzi zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727793"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="40035-102">Wycofanie starszych wersji narzędzi zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="40035-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="40035-103">W rezultacie nowych i ulepszonych funkcji zbierania elektronicznych materiałów dowodowych w centrum zgodności z programem Microsoft 365 następujące starsze narzędzia zbierania elektronicznych materiałów dowodowych i commandlets zostaną wycofane w nadchodzących miesiącach:</span><span class="sxs-lookup"><span data-stu-id="40035-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="40035-104">[Miejscowe zbieranie elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [archiwa miejscowe](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="40035-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="40035-105">Polecenia cmdlet programu Exchange Online PowerShell, które obsługują miejscowe archiwa zbierania elektronicznych materiałów dowodowych i miejscowe.</span><span class="sxs-lookup"><span data-stu-id="40035-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="40035-106">Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet \*-MailboxSearch. Obejmuje następujące polecenia cmdlet:</span><span class="sxs-lookup"><span data-stu-id="40035-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="40035-107">Nowe — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="40035-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="40035-108">Start — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="40035-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="40035-109">Zatrzymaj — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="40035-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="40035-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="40035-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="40035-111">Polecenie cmdlet [Search — Skrzynka pocztowa](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="40035-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="40035-112">Poniższe operacje w interfejsie API usług sieci Web programu Exchange:</span><span class="sxs-lookup"><span data-stu-id="40035-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="40035-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="40035-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="40035-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="40035-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="40035-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="40035-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="40035-116">Zaawansowane zbieranie elektronicznych materiałów dowodowych v 1.0</span><span class="sxs-lookup"><span data-stu-id="40035-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="40035-117">**Oś czasu dla emerytury**:</span><span class="sxs-lookup"><span data-stu-id="40035-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="40035-118">**1 lipca 2020** r. Nie możesz już tworzyć nowych wyszukiwań i blokad, ale możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko.</span><span class="sxs-lookup"><span data-stu-id="40035-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="40035-119">Pomoc techniczna firmy Microsoft nie obsługuje już zamiejscowych & zbierania elektronicznych materiałów dowodowych w pakiecie administracyjnym.</span><span class="sxs-lookup"><span data-stu-id="40035-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="40035-120">**1 października 2020** r. Miejscowe zbieranie elektronicznych materiałów dowodowych & funkcje zostaną umieszczone w trybie tylko do odczytu, więc możesz usunąć tylko istniejące wyszukiwania i blokady.</span><span class="sxs-lookup"><span data-stu-id="40035-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="40035-121">**Aby uzyskać więcej informacji, zobacz**:</span><span class="sxs-lookup"><span data-stu-id="40035-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="40035-122">Migrowanie starszych wyszukiwań i archiwów zbierania elektronicznych materiałów dowodowych do centrum zgodności z programem Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="40035-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="40035-123">Wycofanie starszych wersji narzędzi zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="40035-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="40035-124">Często zadawane pytania dotyczące archiwów zbierania elektronicznych materiałów dowodowych i miejscowych</span><span class="sxs-lookup"><span data-stu-id="40035-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



