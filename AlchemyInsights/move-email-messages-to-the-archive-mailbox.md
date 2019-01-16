---
title: Przenoszenie wiadomości e-mail do skrzynki pocztowej archiwum
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28305009"
---
<span data-ttu-id="1e2ec-p101">Występują problemy podczas archiwizacji elementów do archiwum skrzynki pocztowej. Upewnij się, że zostały wykonane następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="1e2ec-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="1e2ec-p102">Upewnij się, że **archiwum skrzynki pocztowej** zostało włączone. Jeśli tak nie jest, wykonaj kroki w [tym artykule](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) , aby umożliwić archiwum skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="1e2ec-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="1e2ec-106">W Centrum administracyjnego programu Exchange wybierz **Tagi przechowywania** w obszarze **Compliance Management**, Utwórz **tag przechowywania** z akcją **Przenieś do archiwum** zawierające żądane **Limitu czasowego**.</span><span class="sxs-lookup"><span data-stu-id="1e2ec-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="1e2ec-107">W Centrum administracyjnego programu Exchange wybierz **Zasady przechowywania**, utworzyć **Zasady przechowywania** i dodać tag przechowywania **Przenieś do archiwum** do tej zasady.</span><span class="sxs-lookup"><span data-stu-id="1e2ec-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="1e2ec-p103">[Przypisywanie zasad przechowywania](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej danego użytkownika. Takie same zasady zostaną zastosowane do **podstawowego** i **archiwum** skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="1e2ec-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="1e2ec-p104">Skrzynka pocztowa użytkownika powinny być zasad archiwizacji Aby przenieść elementy do archiwum skrzynki pocztowej. Może być konieczne wymuszenie zarządzanych folderów Asystenta (MFA) do uruchomienia i Zastosuj nowe ustawienia do skrzynki pocztowej danego użytkownika. Uruchom następujące polecenie podczas [podłączony do środowiska PowerShell EKSO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) uruchomić Asystenta folderów zarządzanych w konkretnej skrzynce pocztowej:</span><span class="sxs-lookup"><span data-stu-id="1e2ec-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="1e2ec-113">Chcesz uzyskać więcej informacji na temat definiowania zasad archiwizacji, zobacz temat [Set up to archiwum i usuwanie zasady dla skrzynek pocztowych](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="1e2ec-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

