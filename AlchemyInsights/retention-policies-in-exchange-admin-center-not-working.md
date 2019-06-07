---
title: Zasady przechowywania w Centrum administracyjnego programu Exchange nie działa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761592"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="642f0-102">Zasady przechowywania w Centrum administracyjnego programu Exchange</span><span class="sxs-lookup"><span data-stu-id="642f0-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="642f0-103">**Problem:** Nowo utworzony lub zasady przechowywania zaktualizowane w Centrum administracyjnego programu Exchange nie są stosowane do skrzynek pocztowych lub elementy nie są przenoszone do archiwum skrzynki pocztowej lub usunięte.</span><span class="sxs-lookup"><span data-stu-id="642f0-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="642f0-104">**Główne przyczyny:**</span><span class="sxs-lookup"><span data-stu-id="642f0-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="642f0-105">Może to być spowodowane **Zarządzany Asystent folderów** nie przetworzył skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="642f0-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="642f0-106">Asystent folderów zarządzanych próbuje przetworzyć każdą skrzynkę pocztową w organizacji chmurze co siedem dni.</span><span class="sxs-lookup"><span data-stu-id="642f0-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="642f0-107">Jeśli zmianie tagu przechowywania lub zastosowania innych zasad przechowywania do skrzynki pocztowej, możesz poczekać aż zarządzanych folderów pomagają przetwarza skrzynki pocztowej, lub można uruchomić polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych do przetwarzania określonego Skrzynka pocztowa.</span><span class="sxs-lookup"><span data-stu-id="642f0-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="642f0-108">Uruchomienie tego polecenia cmdlet jest użyteczne dla testowania i rozwiązywania problemów z zasad przechowywania lub ustawienia znacznika przechowywania.</span><span class="sxs-lookup"><span data-stu-id="642f0-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="642f0-109">Aby uzyskać więcej informacji odwiedź witrynę [uruchomić Asystenta folderów zarządzanych](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="642f0-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="642f0-110">**Rozwiązania:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych w konkretnej skrzynce pocztowej:</span><span class="sxs-lookup"><span data-stu-id="642f0-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="642f0-111">To również może wystąpić, jeśli **RetentionHold** została **włączona** do skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="642f0-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="642f0-112">Jeśli skrzynka pocztowa jest umieszczone na RetentionHold, zasad przechowywania do skrzynki pocztowej nie będą przetwarzane w tym czasie.</span><span class="sxs-lookup"><span data-stu-id="642f0-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="642f0-113">Aby uzyskać więcej informacji, zobacz ustawienie RetentionHold: [Przytrzymaj przechowywania skrzynki pocztowej](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="642f0-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="642f0-114">**Rozwiązanie:**</span><span class="sxs-lookup"><span data-stu-id="642f0-114">**Solution:**</span></span>
    
  - <span data-ttu-id="642f0-115">Sprawdź ustawienie RetentionHold określonej skrzynki pocztowej w [programie powershell EKSO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="642f0-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="642f0-116">Uruchom następujące polecenie, aby **wyłączyć** RetentionHold na określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="642f0-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="642f0-117">Teraz uruchom ponownie folder zarządzany Asystent:</span><span class="sxs-lookup"><span data-stu-id="642f0-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="642f0-118">**Uwaga:** Jeśli skrzynka pocztowa jest mniejszy niż 10 MB, zarządzany Asystent folderów nie będzie automatycznie przetwarzać skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="642f0-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

