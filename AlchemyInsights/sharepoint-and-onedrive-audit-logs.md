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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992628"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="68c67-102">Dzienniki inspekcji programu SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="68c67-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="68c67-103">Dzienniki inspekcji klasycznego programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="68c67-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="68c67-104">Inspekcja starszej wersji SPO została przeniesiona do Unified dziennik inspekcji (UAL).</span><span class="sxs-lookup"><span data-stu-id="68c67-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="68c67-105">Wszystkie raporty inspekcji starszej wersji SPO będą teraz zasilane za pośrednictwem rejestrowania dostępu użytkowników, a starsze sygnały inspekcji zostały przeniesione do rejestrowania dostępu użytkowników.</span><span class="sxs-lookup"><span data-stu-id="68c67-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="68c67-106">Najważniejsze zmiany:</span><span class="sxs-lookup"><span data-stu-id="68c67-106">Key changes:</span></span>

* <span data-ttu-id="68c67-107">Przycinanie nie jest dostępne jako funkcja.</span><span class="sxs-lookup"><span data-stu-id="68c67-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="68c67-108">Wybór określonych zdarzeń do inspekcji nie jest dostępny.</span><span class="sxs-lookup"><span data-stu-id="68c67-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="68c67-109">Zapoznaj się z [tym dokumentem](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) , aby uzyskać pełną listę inspekcji zdarzeń dostępnych domyślnie.</span><span class="sxs-lookup"><span data-stu-id="68c67-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="68c67-110">Opcja **Lokalizacja** w **raportach dostosowanych** jest niedostępna.</span><span class="sxs-lookup"><span data-stu-id="68c67-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="68c67-111">Opcja **otwierania lub pobierania dokumentów** zdarzenia nie jest dostępna.</span><span class="sxs-lookup"><span data-stu-id="68c67-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="68c67-112">Konfigurowanie ustawień inspekcji dla zbioru witryn</span><span class="sxs-lookup"><span data-stu-id="68c67-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="68c67-113">SharePoint i OneDrive Modern Unified audytu dzienniki z zgodności</span><span class="sxs-lookup"><span data-stu-id="68c67-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="68c67-114">Włączanie/wyłączanie ujednoliconego rejestrowania inspekcji</span><span class="sxs-lookup"><span data-stu-id="68c67-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="68c67-115">Nie jest wymagana żadna dodatkowa konfiguracja w programie SharePoint lub OneDrive.</span><span class="sxs-lookup"><span data-stu-id="68c67-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="68c67-116">Użyj wyszukiwania rejestrowania inspekcji, aby sprawdzić aktywność plików, folderów, użytkowników, uprawnień:</span><span class="sxs-lookup"><span data-stu-id="68c67-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="68c67-117">Działania plików i stron</span><span class="sxs-lookup"><span data-stu-id="68c67-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="68c67-118">Działania folderu</span><span class="sxs-lookup"><span data-stu-id="68c67-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="68c67-119">Udostępnianie i działania związane z żądaniem dostępu</span><span class="sxs-lookup"><span data-stu-id="68c67-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="68c67-120">Działania synchronizacji</span><span class="sxs-lookup"><span data-stu-id="68c67-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="68c67-121">Czynności administrowania witryną</span><span class="sxs-lookup"><span data-stu-id="68c67-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="68c67-122">Aby uzyskać więcej informacji dotyczących sposobu pobierania tych zdarzeń, zobacz [przeszukiwanie dziennika inspekcji](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="68c67-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
