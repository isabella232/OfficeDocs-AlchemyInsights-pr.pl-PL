---
title: 2609-zatrzymywanie lub zbieranie elektronicznych materiałów dowodowych-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994084"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="7ad68-102">Nie można usunąć elementów w programie SharePoint w trybie online lub OneDrive dla firmy</span><span class="sxs-lookup"><span data-stu-id="7ad68-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="7ad68-103">Użytkownik lub jego użytkownicy mogą nie być w stanie usunąć elementy w usłudze SharePoint Online lub OneDrive dla firmy, ponieważ zasady przechowywania, etykieta przechowywania lub przechowywania zbierania elektronicznych materiałów dowodowych jest stosowany do programu SharePoint witryny OneDrive lub do określonego elementu.</span><span class="sxs-lookup"><span data-stu-id="7ad68-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="7ad68-104">Obejmuje to nie można usunąć dokumentu, wersji dokumentu, folderu, biblioteki dokumentów, listy, aplikacji, witryny lub zbioru witryn.</span><span class="sxs-lookup"><span data-stu-id="7ad68-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="7ad68-105">Oto kilka przykładów komunikatów o błędach, które mogą zostać odebrane podczas próby usunięcia elementu, który jest zachowywany:</span><span class="sxs-lookup"><span data-stu-id="7ad68-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="7ad68-106">"Ta witryna nie może zostać usunięta, ponieważ jest uwzględniona w zasadach przechowywania lub zatrzymywania zbierania elektronicznych materiałów dowodowych"</span><span class="sxs-lookup"><span data-stu-id="7ad68-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="7ad68-107">"Ta witryna ma zasady zgodności ustawione na blokowanie usuwania"</span><span class="sxs-lookup"><span data-stu-id="7ad68-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="7ad68-108">"Zasady zgodności obecnie blokuje usunięcie tej witryny"</span><span class="sxs-lookup"><span data-stu-id="7ad68-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="7ad68-109">"Ten zbiór witryn nie może zostać usunięty, ponieważ zawiera witryny, które są uwzględnione w eDiscovery przechowywania lub zasady przechowywania"</span><span class="sxs-lookup"><span data-stu-id="7ad68-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="7ad68-110">"Musisz usunąć wszystkie elementy w tym folderze przed usunięciem folderu"</span><span class="sxs-lookup"><span data-stu-id="7ad68-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="7ad68-111">"Nie można usunąć wersji tego elementu, ponieważ jest on zawieszone lub zasady przechowywania"</span><span class="sxs-lookup"><span data-stu-id="7ad68-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="7ad68-112">"Nie można usunąć elementu podczas wstrzymania"</span><span class="sxs-lookup"><span data-stu-id="7ad68-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="7ad68-113">"Etykieta, która jest stosowana do tego elementu uniemożliwia jego edytowania lub usunięcia"</span><span class="sxs-lookup"><span data-stu-id="7ad68-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="7ad68-114">"Nie można usunąć listy podczas wstrzymania lub zasady przechowywania"</span><span class="sxs-lookup"><span data-stu-id="7ad68-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="7ad68-115">"Lista nie może zostać usunięta, jeśli jest zablokowana lub jeśli zastosowano do niej zasadę przechowywania"</span><span class="sxs-lookup"><span data-stu-id="7ad68-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="7ad68-116">Aby usunąć elementy w jednym z tych scenariuszy, zasady przechowywania, etykieta przechowywania lub przechowywania zbierania elektronicznych materiałów dowodowych musi zostać usunięta (lub witryny musi być wykluczone z zasad przechowywania).</span><span class="sxs-lookup"><span data-stu-id="7ad68-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="7ad68-117">Musisz wyłączyć lub wykluczyć odpowiednie wstrzymanie, które jest przyczyną tego problemu.</span><span class="sxs-lookup"><span data-stu-id="7ad68-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="7ad68-118">Po usunięciu zasad przechowywania lub wstrzymania może potrwać do 24 godzin, aby zmiany zostały uwzględnione.</span><span class="sxs-lookup"><span data-stu-id="7ad68-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="7ad68-119">Aby uzyskać informacje o różnych funkcjach przechowywania i przechowywania, które można zastosować do witryn programu SharePoint i kont usługi OneDrive, zobacz jeden z następujących tematów.</span><span class="sxs-lookup"><span data-stu-id="7ad68-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="7ad68-120">Omówienie zasad przechowywania</span><span class="sxs-lookup"><span data-stu-id="7ad68-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="7ad68-121">Omówienie etykiet przechowywania</span><span class="sxs-lookup"><span data-stu-id="7ad68-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="7ad68-122">Zarządzanie przechowuje w zaawansowanym eDiscovery</span><span class="sxs-lookup"><span data-stu-id="7ad68-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="7ad68-123">eDiscovery posiada</span><span class="sxs-lookup"><span data-stu-id="7ad68-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="7ad68-124">Zasady dotyczące zamykania i usuwania witryn starszych</span><span class="sxs-lookup"><span data-stu-id="7ad68-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
