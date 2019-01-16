---
title: Zasady przechowywania w Centrum administracyjnego programu Exchange nie działa
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303938"
---
 <span data-ttu-id="04922-102">**Problem:** Nowo utworzony lub zasady przechowywania zaktualizowane w Centrum administracyjnego programu Exchange nie są stosowane do skrzynek pocztowych lub elementy nie są przenoszone do archiwum skrzynki pocztowej lub usunięte.</span><span class="sxs-lookup"><span data-stu-id="04922-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="04922-103">**Główne przyczyny:**</span><span class="sxs-lookup"><span data-stu-id="04922-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="04922-p101">Może to być spowodowane **Zarządzany Asystent folderów** nie przetworzył skrzynki pocztowej użytkownika. Asystent folderów zarządzanych próbuje przetworzyć każdą skrzynkę pocztową w organizacji chmurze co siedem dni. Jeśli zmianie tagu przechowywania lub zastosowania innych zasad przechowywania do skrzynki pocztowej, możesz poczekać aż zarządzanych folderów pomagają przetwarza skrzynki pocztowej, lub można uruchomić polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych do przetwarzania określonego Skrzynka pocztowa. Uruchomienie tego polecenia cmdlet jest użyteczne dla testowania i rozwiązywania problemów z zasad przechowywania lub ustawienia znacznika przechowywania. Aby uzyskać więcej informacji odwiedź witrynę [uruchomić Asystenta folderów zarządzanych](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="04922-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="04922-109">**Rozwiązania:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych w konkretnej skrzynce pocztowej:</span><span class="sxs-lookup"><span data-stu-id="04922-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="04922-p102">To również może wystąpić, jeśli **RetentionHold** została **włączona** do skrzynki pocztowej. Jeśli skrzynka pocztowa jest umieszczone na RetentionHold, zasad przechowywania do skrzynki pocztowej nie będą przetwarzane w tym czasie. Aby uzyskać więcej informacji, zobacz ustawienie RetentionHold: [Przytrzymaj przechowywania skrzynki pocztowej](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="04922-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="04922-113">**Rozwiązanie:**</span><span class="sxs-lookup"><span data-stu-id="04922-113">**Solution:**</span></span>
    
  - <span data-ttu-id="04922-114">Sprawdź ustawienie RetentionHold określonej skrzynki pocztowej w [programie powershell EKSO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="04922-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="04922-115">Uruchom następujące polecenie, aby **wyłączyć** RetentionHold na określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="04922-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="04922-116">Teraz uruchom ponownie folder zarządzany Asystent:</span><span class="sxs-lookup"><span data-stu-id="04922-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="04922-117">**Uwaga:** Jeśli skrzynka pocztowa jest mniejszy niż 10 MB, zarządzany Asystent folderów nie będzie automatycznie przetwarzać skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="04922-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

