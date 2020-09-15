---
title: Klasyczne raporty dziennika inspekcji programu SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662218"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="a8609-102">Dzienniki inspekcji programu SharePoint i usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="a8609-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="a8609-103">Klasyczne dzienniki inspekcji programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="a8609-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="a8609-104">USŁUGI spo starszej inspekcji uległa migracji do dziennika ujednoliconej inspekcji (UAL).</span><span class="sxs-lookup"><span data-stu-id="a8609-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="a8609-105">Wszystkie usługi spo starsze raporty inspekcji będą teraz obsługiwane przez UAL, a starsze sygnały inspekcji zostaną zmigrowane do UAL.</span><span class="sxs-lookup"><span data-stu-id="a8609-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="a8609-106">Kluczowe zmiany:</span><span class="sxs-lookup"><span data-stu-id="a8609-106">Key changes:</span></span>

* <span data-ttu-id="a8609-107">Przycinanie nie jest dostępne w ramach funkcji.</span><span class="sxs-lookup"><span data-stu-id="a8609-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="a8609-108">Wybieranie określonych zdarzeń do inspekcji jest niedostępne.</span><span class="sxs-lookup"><span data-stu-id="a8609-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="a8609-109">Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) , aby uzyskać pełną listę dostępnych zdarzeń, które można poddać inspekcji domyślnie.</span><span class="sxs-lookup"><span data-stu-id="a8609-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="a8609-110">Opcja **Lokalizacja** w obszarze **niestandardowe raporty** jest niedostępna.</span><span class="sxs-lookup"><span data-stu-id="a8609-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="a8609-111">Opcja **otwierania lub pobierania dokumentów** jest niedostępna.</span><span class="sxs-lookup"><span data-stu-id="a8609-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="a8609-112">Konfigurowanie ustawień inspekcji dla zbioru witryn</span><span class="sxs-lookup"><span data-stu-id="a8609-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="a8609-113">Nowoczesne dzienniki ujednoliconej inspekcji programu SharePoint i usługi OneDrive z poziomu zgodności</span><span class="sxs-lookup"><span data-stu-id="a8609-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="a8609-114">Włączanie/wyłączanie ujednoliconych rejestracji inspekcji</span><span class="sxs-lookup"><span data-stu-id="a8609-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="a8609-115">W programie SharePoint lub usłudze OneDrive nie jest wymagana żadna dodatkowa konfiguracja.</span><span class="sxs-lookup"><span data-stu-id="a8609-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="a8609-116">Użyj funkcji wyszukiwania rejestrowania inspekcji, aby sprawdzić aktywność plików, folderów, użytkowników, uprawnień:</span><span class="sxs-lookup"><span data-stu-id="a8609-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="a8609-117">Działania dotyczące plików i stron</span><span class="sxs-lookup"><span data-stu-id="a8609-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="a8609-118">Działania dotyczące folderów</span><span class="sxs-lookup"><span data-stu-id="a8609-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="a8609-119">Działania dotyczące udostępniania i żądania dostępu</span><span class="sxs-lookup"><span data-stu-id="a8609-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="a8609-120">Działania synchronizacji</span><span class="sxs-lookup"><span data-stu-id="a8609-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="a8609-121">Działania administracyjne witryny</span><span class="sxs-lookup"><span data-stu-id="a8609-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="a8609-122">Aby uzyskać więcej informacji o tym, jak pobrać te zdarzenia, zobacz [przeszukiwanie dziennika inspekcji](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="a8609-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
