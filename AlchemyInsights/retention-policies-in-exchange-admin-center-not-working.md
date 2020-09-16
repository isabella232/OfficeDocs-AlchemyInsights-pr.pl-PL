---
title: Zasady przechowywania w centrum administracyjnym programu Exchange nie działają
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740520"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="88f72-102">Zasady przechowywania w centrum administracyjnym programu Exchange</span><span class="sxs-lookup"><span data-stu-id="88f72-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="88f72-103">Jeśli chcesz, aby w przypadku uruchamiania zautomatyzowanej kontroli nad ustawieniami wymienionymi poniżej, wybierz przycisk Wstecz <--u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z zasadami przechowywania.</span><span class="sxs-lookup"><span data-stu-id="88f72-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="88f72-104">**Problem:** Nowo utworzone lub zaktualizowane zasady przechowywania w centrum administracyjnym programu Exchange nie są stosowane do skrzynek pocztowych ani elementów, które nie są przenoszone do archiwum ani do usuniętej archiwalnej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="88f72-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="88f72-105">**Główne przyczyny:**</span><span class="sxs-lookup"><span data-stu-id="88f72-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="88f72-106">Może to wynikać z faktu, że **Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="88f72-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="88f72-107">Asystent folderów zarządzanych próbuje przetwarzać każdą skrzynkę pocztową w organizacji opartą na chmurze raz na siedem dni.</span><span class="sxs-lookup"><span data-stu-id="88f72-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="88f72-108">Jeśli zmienisz znacznik przechowywania lub zastosowano inne zasady przechowywania do skrzynki pocztowej, możesz poczekać, aż folder zarządzany będzie mógł przetworzyć skrzynkę pocztową, lub uruchomić polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych w celu przetworzenia określonej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="88f72-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="88f72-109">Uruchomienie tego polecenia cmdlet jest przydatne w przypadku testowania lub rozwiązywania problemów dotyczących zasad przechowywania lub ustawień znaczników przechowywania.</span><span class="sxs-lookup"><span data-stu-id="88f72-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="88f72-110">Aby uzyskać więcej informacji, odwiedź stronę [uruchamianie Asystenta folderów zarządzanych](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="88f72-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="88f72-111">**Rozwiązanie:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="88f72-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="88f72-112">Może to być również możliwe, jeśli w skrzynce pocztowej **włączono** **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="88f72-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="88f72-113">Jeśli skrzynka pocztowa została umieszczona na RetentionHoldie, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie.</span><span class="sxs-lookup"><span data-stu-id="88f72-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="88f72-114">Aby uzyskać więcej Informaton na temat ustawienia RetentionHold, zobacz: [Blokada przechowywania skrzynek pocztowych](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="88f72-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="88f72-115">**Rozwiązać**</span><span class="sxs-lookup"><span data-stu-id="88f72-115">**Solution:**</span></span>
    
  - <span data-ttu-id="88f72-116">Sprawdź stan ustawienia RetentionHold w określonej skrzynce pocztowej w programie [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="88f72-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="88f72-117">Uruchom następujące polecenie, aby **wyłączyć** RetentionHold w określonej skrzynce pocztowej:</span><span class="sxs-lookup"><span data-stu-id="88f72-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="88f72-118">Teraz uruchom ponownie Asystenta zarządzanego folderu:</span><span class="sxs-lookup"><span data-stu-id="88f72-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="88f72-119">**Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzać skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="88f72-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="88f72-120">Aby uzyskać więcej informacji na temat zasad przechowywania w centrum administracyjnym programu Exchange, zobacz:</span><span class="sxs-lookup"><span data-stu-id="88f72-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="88f72-121">Tagi przechowywania i zasady przechowywania</span><span class="sxs-lookup"><span data-stu-id="88f72-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="88f72-122">Stosowanie zasad przechowywania do skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="88f72-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="88f72-123">Dodawanie lub usuwanie znaczników przechowywania</span><span class="sxs-lookup"><span data-stu-id="88f72-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="88f72-124">Jak zidentyfikować typ blokady umieszczanej w skrzynce pocztowej</span><span class="sxs-lookup"><span data-stu-id="88f72-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
