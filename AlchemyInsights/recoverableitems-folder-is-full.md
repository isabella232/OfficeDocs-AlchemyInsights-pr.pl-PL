---
title: 1336 RecoverableItems folder jest pełny
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: a048949d5284d018303d03aad26cdf26eee2fb5c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776406"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="9c6f6-102">Przechowalni jest pełny</span><span class="sxs-lookup"><span data-stu-id="9c6f6-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="9c6f6-103">Dla skrzynek pocztowych Exchange Online w usłudze Office 365 domyślny limit miejsca dla folderu odzyskane elementy wynosi 30 GB.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="9c6f6-104">Limit miejsca dla folderu odzyskane elementy automatycznie wzrasta do 100 GB, jeśli Skrzynka pocztowa jest umieszczany na sądowym, przytrzymaj zbierania elektronicznych materiałów dowodowych lub jest przypisana do zasad przechowywania usługi Office 365.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="9c6f6-105">Gdy przechowalni osiągnie limit magazynowania, funkcje skrzynki pocztowej ma wpływ w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="9c6f6-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="9c6f6-106">Użytkownika nie można usunąć elementów ze skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="9c6f6-107">Zarządzany Asystent folderów nie można usunąć elementów na podstawie tagu przechowywania lub ustawienia folderów zarządzanych.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="9c6f6-108">Dla skrzynek pocztowych, które włączonym odzyskiwaniem pojedynczego elementu lub są wstrzymane proces kopiowania przy zapisie strony ochrony nie może utrzymać wersje elementów edytowane przez użytkownika.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="9c6f6-109">Skrzynki pocztowe, które ma włączone rejestrowanie inspekcji skrzynki pocztowej wpisy dziennika inspekcji skrzynki pocztowej nie można zapisywać w podfolderze audyty w przechowalni.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="9c6f6-110">Skrzynki pocztowe, które nie są zablokowane, Administratorzy można użyć `Search-Mailbox -SearchDumpsterOnly -DeleteContent` polecenia programu PowerShell Online programu Exchange do usuwania elementów w przechowalni.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-110">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="9c6f6-111">Aby uzyskać więcej informacji, zobacz następujące tematy:</span><span class="sxs-lookup"><span data-stu-id="9c6f6-111">For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="9c6f6-112">Wyszukiwanie i usuwanie wiadomości</span><span class="sxs-lookup"><span data-stu-id="9c6f6-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="9c6f6-113">Skrzynka pocztowa wyszukiwania</span><span class="sxs-lookup"><span data-stu-id="9c6f6-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="9c6f6-114">Administratorzy dla skrzynek pocztowych, które zostały wstrzymane, trzeba usunąć ładowni, zanim będą mogli elementy usunięte z folderu elementów do odzyskania.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="9c6f6-115">Aby uzyskać więcej informacji zobacz [Usuwanie elementów w przechowalni, przytrzymaj folder chmurowych skrzynek pocztowych na](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9c6f6-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="9c6f6-116">Aby zapobiec przechowalni staje się pełne, Administratorzy mogą zwiększyć limit magazynowania odzyskiwalnych elementów folderu dla skrzynek pocztowych na przytrzymaj i ustawianie zasad przechowywania skrzynki pocztowej, która przenosi elementy z folderu odzyskane elementy do archiwum użytkownika Skrzynka pocztowa.</span><span class="sxs-lookup"><span data-stu-id="9c6f6-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="9c6f6-117">Zobacz [zwiększyć odzyskane elementy przydziału dla skrzynek pocztowych na przytrzymaj](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9c6f6-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

