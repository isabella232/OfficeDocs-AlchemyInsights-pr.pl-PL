---
title: Przenoszenie wiadomości e-mail do archiwum Skrzynka pocztowa
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799790"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="1e954-102">Przenoszenie wiadomości e-mail do archiwum Skrzynka pocztowa</span><span class="sxs-lookup"><span data-stu-id="1e954-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="1e954-103">Jeśli chcesz, aby w przypadku uruchamiania zautomatyzowanego sprawdzania ustawień wymienionych poniżej wybrać przycisk Wstecz <--u góry tej strony, a następnie wprowadź adres e-mail użytkownika, który ma problemy z przenoszeniem wiadomości e-mail do ich archiwum.</span><span class="sxs-lookup"><span data-stu-id="1e954-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="1e954-104">Potwierdź, że włączono **skrzynkę pocztową archiwum** .</span><span class="sxs-lookup"><span data-stu-id="1e954-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="1e954-105">Jeśli nie, wykonaj czynności opisane w [tym artykule](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , aby włączyć archiwizowaną skrzynkę pocztową.</span><span class="sxs-lookup"><span data-stu-id="1e954-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="1e954-106">Aby automatycznie archiwizować wiadomości w archiwum Skrzynka pocztowa, należy ustawić znacznik przechowywania z akcją **Przenieś do archiwum** , aby był **stosowany automatycznie do całego znacznika skrzynki pocztowej (domyślnego)**.</span><span class="sxs-lookup"><span data-stu-id="1e954-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="1e954-107">Wykonaj poniższe czynności, aby utworzyć Tag: [archiwum domyślne](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="1e954-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="1e954-108">Następnie Dodaj tag **archiwum** do zasad przechowywania.</span><span class="sxs-lookup"><span data-stu-id="1e954-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="1e954-109">W centrum administracyjnym programu Exchange wybierz pozycję **zasady przechowywania** > Dodaj **tag Przenieś do archiwum** do zasad > **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="1e954-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="1e954-110">Teraz [Przypisz zasady przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej określonego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="1e954-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="1e954-111">Te same zasady zostaną zastosowane zarówno do **głównej** , jak i do **archiwum** Skrzynka pocztowa.</span><span class="sxs-lookup"><span data-stu-id="1e954-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="1e954-112">Może być konieczne wymuszenie uruchomienia Asystenta zarządzanego folderu (MFA) i zastosowania nowych ustawień do skrzynki pocztowej użytkownika.</span><span class="sxs-lookup"><span data-stu-id="1e954-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="1e954-113">Uruchom następujące polecenie podczas [nawiązania połączenia z programem EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , aby uruchomić Asystenta folderów zarządzanych dla określonej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="1e954-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="1e954-114">Start-ManagedFolderAssistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="1e954-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="1e954-115">Aby uzyskać więcej informacji na temat konfigurowania zasad archiwizacji, zobacz [Konfigurowanie zasad archiwizacji i usuwania dla skrzynek pocztowych](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="1e954-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  