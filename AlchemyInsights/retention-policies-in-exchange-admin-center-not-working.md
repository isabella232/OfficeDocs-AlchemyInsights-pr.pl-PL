---
title: Zasady przechowywania w Centrum administracyjnym programu Exchange nie działają
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502617"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="f5524-102">Zasady przechowywania w Centrum administracyjnym programu Exchange</span><span class="sxs-lookup"><span data-stu-id="f5524-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="f5524-103">**Problem:** Nowo utworzone lub zaktualizowane zasady przechowywania w Centrum administracyjnym programu Exchange nie mają zastosowania do skrzynek pocztowych lub elementy nie są przenoszone do archiwalnej skrzynki pocztowej ani usuwane.</span><span class="sxs-lookup"><span data-stu-id="f5524-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="f5524-104">**Przyczyn:**</span><span class="sxs-lookup"><span data-stu-id="f5524-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="f5524-105">Może to być spowodowane tym, że **Asystent folderów zarządzanych** nie przetworzył skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f5524-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="f5524-106">Asystent folderów zarządzanych próbuje przetworzyć każdą skrzynkę pocztową w organizacji chmurowej raz na siedem dni.</span><span class="sxs-lookup"><span data-stu-id="f5524-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="f5524-107">Jeśli zmienisz tag przechowywania lub zastosujesz inną zasadę przechowywania do skrzynki pocztowej, możesz poczekać, aż Asysta folderu zarządzanego przetworzy skrzynkę pocztową lub uruchomisz polecenie cmdlet Start-ManagedFolderAssistant, aby uruchomić Asystenta folderów zarządzanych w celu przetworzenia określonej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="f5524-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="f5524-108">Uruchamianie tego polecenia cmdlet jest przydatne do testowania lub rozwiązywania problemów z ustawieniami zasad przechowywania lub tagu przechowywania.</span><span class="sxs-lookup"><span data-stu-id="f5524-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="f5524-109">Aby uzyskać więcej informacji, odwiedź stronę [Uruchom Asystenta folderów zarządzanych](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="f5524-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="f5524-110">**Rozwiązanie:** Uruchom następujące polecenie, aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="f5524-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="f5524-111">Może to również wystąpić, jeśli **retentionHold** została **włączona** w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="f5524-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="f5524-112">Jeśli skrzynka pocztowa została umieszczona w retencji, zasady przechowywania w skrzynce pocztowej nie będą przetwarzane w tym czasie.</span><span class="sxs-lookup"><span data-stu-id="f5524-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="f5524-113">Aby uzyskać więcej informacji na temat ustawienia HoldHold, zobacz: [Wstrzymanie przechowywania skrzynki pocztowej](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="f5524-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="f5524-114">**Rozwiązanie:**</span><span class="sxs-lookup"><span data-stu-id="f5524-114">**Solution:**</span></span>
    
  - <span data-ttu-id="f5524-115">Sprawdź stan ustawienia Retencja w określonej skrzynce pocztowej w programie [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="f5524-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="f5524-116">Uruchom następujące polecenie, aby **wyłączyć** retencję w określonej skrzynce pocztowej:</span><span class="sxs-lookup"><span data-stu-id="f5524-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="f5524-117">Teraz ponownie uruchom Asystenta folderu zarządzanego:</span><span class="sxs-lookup"><span data-stu-id="f5524-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="f5524-118">**Uwaga:** Jeśli skrzynka pocztowa jest mniejsza niż 10 MB, Asystent folderów zarządzanych nie będzie automatycznie przetwarzał skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="f5524-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="f5524-119">Aby uzyskać więcej informacji na temat zasad przechowywania w Centrum administracyjnym programu Exchange, zobacz:</span><span class="sxs-lookup"><span data-stu-id="f5524-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="f5524-120">Tagi przechowywania i zasady przechowywania</span><span class="sxs-lookup"><span data-stu-id="f5524-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="f5524-121">Stosowanie zasad przechowywania do skrzynek pocztowych</span><span class="sxs-lookup"><span data-stu-id="f5524-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="f5524-122">Dodawanie lub usuwanie znaczników przechowywania</span><span class="sxs-lookup"><span data-stu-id="f5524-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="f5524-123">Jak zidentyfikować typ blokady umieszczonej na skrzynce pocztowej</span><span class="sxs-lookup"><span data-stu-id="f5524-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
