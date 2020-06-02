---
title: Raporty dziennika inspekcji klasycznej programu SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509610"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="019cc-102">Dzienniki inspekcji programu SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="019cc-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="019cc-103">Klasyczne dzienniki inspekcji programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="019cc-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="019cc-104">Inspekcja starszej wersji spo została zmigrowana do ujednoliconego dziennika inspekcji (UAL).</span><span class="sxs-lookup"><span data-stu-id="019cc-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="019cc-105">Wszystkie starsze raporty inspekcji spo będą teraz zasilane przez UAL, a starsze sygnały inspekcji zostały przeniesione do UAL.</span><span class="sxs-lookup"><span data-stu-id="019cc-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="019cc-106">Kluczowe zmiany:</span><span class="sxs-lookup"><span data-stu-id="019cc-106">Key changes:</span></span>

* <span data-ttu-id="019cc-107">Przycinanie NIE jest dostępne jako możliwość.</span><span class="sxs-lookup"><span data-stu-id="019cc-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="019cc-108">Wybieranie określonych zdarzeń do inspekcji NIE jest dostępne.</span><span class="sxs-lookup"><span data-stu-id="019cc-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="019cc-109">Pełną listę zdarzeń inspekcji dostępnych domyślnie można znaleźć w [tym dokumencie.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="019cc-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="019cc-110">Opcja **Lokalizacja** w obszarze **Raporty niestandardowe** NIE jest dostępna.</span><span class="sxs-lookup"><span data-stu-id="019cc-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="019cc-111">Opcja **Otwieranie lub pobieranie dokumentów** zdarzenia nie jest dostępna.</span><span class="sxs-lookup"><span data-stu-id="019cc-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="019cc-112">Konfigurowanie ustawień inspekcji dla zbioru witryn</span><span class="sxs-lookup"><span data-stu-id="019cc-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="019cc-113">Dzienniki inspekcji programu SharePoint i OneDrive Modern Unified Audit pochodzą z zgodności</span><span class="sxs-lookup"><span data-stu-id="019cc-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="019cc-114">Włączanie/wyłączanie rejestrowania inspekcji ujednoliconej inspekcji</span><span class="sxs-lookup"><span data-stu-id="019cc-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="019cc-115">W programie SharePoint lub OneDrive nie jest wymagana żadna dodatkowa konfiguracja.</span><span class="sxs-lookup"><span data-stu-id="019cc-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="019cc-116">Użyj wyszukiwania rejestrowania inspekcji, aby sprawdzić aktywność plików, folderów, użytkowników, uprawnień:</span><span class="sxs-lookup"><span data-stu-id="019cc-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="019cc-117">Działania związane z plikami i stronicowakami</span><span class="sxs-lookup"><span data-stu-id="019cc-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="019cc-118">Działania folderów</span><span class="sxs-lookup"><span data-stu-id="019cc-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="019cc-119">Udostępnianie i uzyskiwanie dostępu do działań żądań</span><span class="sxs-lookup"><span data-stu-id="019cc-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="019cc-120">Działania synchronizacji</span><span class="sxs-lookup"><span data-stu-id="019cc-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="019cc-121">Działania związane z administracją witryną</span><span class="sxs-lookup"><span data-stu-id="019cc-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="019cc-122">Aby uzyskać więcej informacji na temat pobierania tych zdarzeń, zobacz [Wyszukiwanie w dzienniku inspekcji](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="019cc-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
