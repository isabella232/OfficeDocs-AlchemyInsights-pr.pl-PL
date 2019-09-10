---
title: Przenoszenie wiadomości e-mail do archiwalnej skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822172"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="6ed87-102">Przenoszenie wiadomości e-mail do archiwalnej skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="6ed87-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="6ed87-103">Potwierdź, że została włączona **archiwalna skrzynka pocztowa** .</span><span class="sxs-lookup"><span data-stu-id="6ed87-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="6ed87-104">Jeśli nie, wykonaj kroki opisane w [tym artykule](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , aby włączyć archiwalną skrzynkę pocztową.</span><span class="sxs-lookup"><span data-stu-id="6ed87-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="6ed87-105">Aby automatycznie archiwizować wiadomości w archiwalnej skrzynce pocztowej, znacznik przechowywania z akcją **Przenieś na archiwizację** musi być ustawiony na **automatycznie zastosowany do całej skrzynki pocztowej (domyślnie)**.</span><span class="sxs-lookup"><span data-stu-id="6ed87-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="6ed87-106">Wykonaj poniższe kroki, aby utworzyć znacznik: [Archive default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="6ed87-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="6ed87-107">Następnie Dodaj tag **archiwum** do zasad przechowywania.</span><span class="sxs-lookup"><span data-stu-id="6ed87-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="6ed87-108">W centrum administracyjnego programu Exchange wybierz **zasady przechowywania** > Dodaj **Przenieś do archiwum tag** do zasady > **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="6ed87-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="6ed87-109">Teraz [Przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6ed87-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="6ed87-110">Te same zasady zostaną zastosowane zarówno do **podstawowej** , jak i **archiwalnej** skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="6ed87-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="6ed87-111">Może być konieczne wymuszenie Asystenta folderów zarządzanych (MFA), aby uruchomić i zastosować nowe ustawienia do skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6ed87-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="6ed87-112">Uruchom następujące polecenie podczas [połączenia z EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="6ed87-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="6ed87-113">Start-ManagedFolderAssistant-tożsamość<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="6ed87-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="6ed87-114">Aby uzyskać więcej informacji o konfigurowaniu zasad archiwizacji, zobacz [Konfigurowanie zasad archiwizacji i usuwania dla skrzynek pocztowych](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="6ed87-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  