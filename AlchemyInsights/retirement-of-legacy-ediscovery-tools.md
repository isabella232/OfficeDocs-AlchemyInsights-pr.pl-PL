---
title: Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798559"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="c7320-102">Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="c7320-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="c7320-103">W wyniku nowych i ulepszonych funkcji zbierania elektronicznych materiałów dowodowych w Centrum zgodności platformy Microsoft 365 następujące starsze narzędzia i polecenia zbierania elektronicznych materiałów dowodowych zostaną wycofane w nadchodzących miesiącach:</span><span class="sxs-lookup"><span data-stu-id="c7320-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="c7320-104">[Zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) w miejscu i [zbierania](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) elektronicznych materiałów dowodowych w centrum administracyjnym programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7320-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="c7320-105">Polecenia cmdlet programu PowerShell usługi Exchange Online, które obsługują In-Place zbierania elektronicznych materiałów dowodowych i In-Place zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="c7320-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="c7320-106">(Te polecenia cmdlet są zbiorczo identyfikowane jako polecenia cmdlet \*-MailboxSearch). Obejmuje to następujące polecenia cmdlet:</span><span class="sxs-lookup"><span data-stu-id="c7320-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="c7320-107">Nowe wyszukiwanie skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="c7320-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="c7320-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7320-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="c7320-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7320-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="c7320-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7320-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="c7320-111">Polecenie [cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) w programie PowerShell dla usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c7320-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="c7320-112">Następujące operacje w interfejsie API usług sieci Web programu Exchange:</span><span class="sxs-lookup"><span data-stu-id="c7320-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="c7320-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c7320-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="c7320-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c7320-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="c7320-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c7320-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="c7320-116">Advanced eDiscovery 1.0</span><span class="sxs-lookup"><span data-stu-id="c7320-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="c7320-117">**Oś czasu dla wycofania:**</span><span class="sxs-lookup"><span data-stu-id="c7320-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="c7320-118">**1 lipca 2020 r.** Nie możesz już tworzyć nowych wyszukiwań ani blokady, ale możesz uruchamiać, edytować i usuwać istniejące wyszukiwania na własne ryzyko.</span><span class="sxs-lookup"><span data-stu-id="c7320-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="c7320-119">Pomoc techniczna firmy Microsoft nie obsługuje już In-Place zbierania elektronicznych materiałów dowodowych & eAC.</span><span class="sxs-lookup"><span data-stu-id="c7320-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="c7320-120">**1 października 2020** rIn-Place funkcja zbierania elektronicznych materiałów dowodowych & w Aplikacji EAC zostanie umieszczona w trybie tylko do odczytu, więc można tylko usuwać istniejące wyszukiwania i blokady.</span><span class="sxs-lookup"><span data-stu-id="c7320-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="c7320-121">**Aby uzyskać więcej informacji, zobacz:**</span><span class="sxs-lookup"><span data-stu-id="c7320-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="c7320-122">Migrowanie starszych wyszukiwań i funkcji zbierania elektronicznych materiałów dowodowych do Centrum zgodności platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c7320-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="c7320-123">Wycofanie starszych narzędzi zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="c7320-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="c7320-124">Często zadawane pytania dotyczące zbierania In-Place eDiscovery i zbierania elektronicznych In-Place zbierania elektronicznych materiałów dowodowych</span><span class="sxs-lookup"><span data-stu-id="c7320-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



