---
title: Przenoszenie wiadomości e-mail do skrzynki pocztowej Archiwum
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522781"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="b580e-102">Przenoszenie wiadomości e-mail do archiwalnej skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="b580e-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="b580e-103">Jeśli chcesz, abyśmy przeprowadzili automatyczne kontrole ustawień wymienionych poniżej, wybierz przycisk Wstecz < - u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z przeniesieniem poczty e-mail do swojej archiwalnej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="b580e-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="b580e-104">Upewnij się, że **skrzynka pocztowa archiwum** została włączona.</span><span class="sxs-lookup"><span data-stu-id="b580e-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="b580e-105">Jeśli nie, użyj kroków w [tym artykule,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) aby włączyć archiwalnej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="b580e-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="b580e-106">Aby automatycznie archiwizować wiadomości do archiwalnej skrzynki pocztowej, tag przechowywania z akcją **Przenieś do archiwum** musi być automatycznie **stosowany do całego tagu skrzynki pocztowej (domyślnie).**</span><span class="sxs-lookup"><span data-stu-id="b580e-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="b580e-107">Użyj kroków tutaj, aby utworzyć tag: [Archiwum domyślny tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="b580e-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="b580e-108">Następnie dodaj tag **Archiwum** do zasad przechowywania.</span><span class="sxs-lookup"><span data-stu-id="b580e-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="b580e-109">W Centrum administracyjnym programu Exchange wybierz pozycję **Zasady przechowywania** > dodaj tag Przenieś **do archiwum** do zasad > **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="b580e-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="b580e-110">Teraz [przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="b580e-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="b580e-111">Ta sama zasada zostanie zastosowana zarówno do **skrzynki pocztowej Podstawowa,** jak i **Archiwum.**</span><span class="sxs-lookup"><span data-stu-id="b580e-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="b580e-112">Może być konieczne wymuszenie uruchomienia asystenta folderów zarządzanych (MFA) i zastosowania nowych ustawień do skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="b580e-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="b580e-113">Uruchom następujące polecenie po [podłączeniu do programu EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="b580e-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="b580e-114">Start-ManagedFolderAssistant -Tożsamość<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="b580e-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="b580e-115">Aby uzyskać więcej informacji na temat konfigurowania zasad archiwizacji, zobacz [Konfigurowanie zasad archiwizacji i usuwania skrzynek pocztowych](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="b580e-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  