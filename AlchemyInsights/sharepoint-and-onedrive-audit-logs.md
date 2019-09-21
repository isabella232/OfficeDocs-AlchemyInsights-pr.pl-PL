---
title: Klasyczne raporty dziennika inspekcji programu SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068033"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="95308-102">Dzienniki inspekcji programu SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="95308-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="95308-103">**SharePoint i OneDrive Modern Unified audytu dzienniki z zgodności**</span><span class="sxs-lookup"><span data-stu-id="95308-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="95308-104">Włączanie/wyłączanie ujednoliconego rejestrowania inspekcji</span><span class="sxs-lookup"><span data-stu-id="95308-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="95308-105">Nie jest wymagana żadna dodatkowa konfiguracja w programie SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="95308-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="95308-106">Użyj wyszukiwania rejestrowania inspekcji, aby sprawdzić aktywność plików, folderów, użytkowników, uprawnień:</span><span class="sxs-lookup"><span data-stu-id="95308-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="95308-107">Działania plików i stron</span><span class="sxs-lookup"><span data-stu-id="95308-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="95308-108">Działania folderu</span><span class="sxs-lookup"><span data-stu-id="95308-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="95308-109">Udostępnianie i działania związane z żądaniem dostępu</span><span class="sxs-lookup"><span data-stu-id="95308-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="95308-110">Działania synchronizacji</span><span class="sxs-lookup"><span data-stu-id="95308-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="95308-111">Czynności administrowania witryną</span><span class="sxs-lookup"><span data-stu-id="95308-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="95308-112">Aby uzyskać więcej informacji dotyczących sposobu pobierania tych zdarzeń, zobacz [przeszukiwanie dziennika inspekcji](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="95308-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="95308-113">**Dzienniki inspekcji klasycznego programu SharePoint**</span><span class="sxs-lookup"><span data-stu-id="95308-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="95308-114">Zmigrowaliśmy inspekcji starszej wersji SPO do Unified dziennik inspekcji (UAL).</span><span class="sxs-lookup"><span data-stu-id="95308-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="95308-115">Oznacza to zasadniczo, że wszystkie raporty inspekcji starszej wersji SPO będą teraz zasilane za pośrednictwem rejestrowania dostępu użytkowników, a starsze sygnały inspekcji zostały przeniesione do rejestrowania dostępu użytkowników.</span><span class="sxs-lookup"><span data-stu-id="95308-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="95308-116">Najważniejsze zmiany:</span><span class="sxs-lookup"><span data-stu-id="95308-116">Key changes:</span></span>

- <span data-ttu-id="95308-117">Przycinanie jako możliwości nie jest dostępne.</span><span class="sxs-lookup"><span data-stu-id="95308-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="95308-118">Sekcja, w której można wybrać określone zdarzenia do inspekcji, nie jest dostępna.</span><span class="sxs-lookup"><span data-stu-id="95308-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="95308-119">Aby uzyskać pełną listę inspekcji zdarzeń dostępnych domyślnie, należy zapoznać się z [tym dokumentem](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="95308-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="95308-120">Opcja "lokalizacja" w **raportach DOSTOSOWANYCH** nie jest dostępna.</span><span class="sxs-lookup"><span data-stu-id="95308-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="95308-121">Zdarzenia "Otwieranie lub pobieranie dokumentów" nie są dostępne.</span><span class="sxs-lookup"><span data-stu-id="95308-121">“Opening or downloading documents” events is NOT available.</span></span> 

