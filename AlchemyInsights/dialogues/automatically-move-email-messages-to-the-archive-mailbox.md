---
title: Automatyczne przenoszenie wiadomości e-mail do archiwaowej skrzynki pocztowej
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527104"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="9c9d3-102">Automatyczne przenoszenie wiadomości e-mail do archiwaowej skrzynki pocztowej</span><span class="sxs-lookup"><span data-stu-id="9c9d3-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="9c9d3-103">Oto jak skonfigurować zasady automatycznego przenoszenia starych wiadomości e-mail użytkownika do archiwaowej skrzynki pocztowej:</span><span class="sxs-lookup"><span data-stu-id="9c9d3-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="9c9d3-104">Przejdź do [**& zarządzania**](https://go.microsoft.com/fwlink/p/?linkid=2077143)danymi zgodności, aby sprawdzić, czy dla użytkownika włączono archiwacyjną  >    >   skrzynkę pocztową.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="9c9d3-105">Jeśli tak nie jest, kliknij przycisk **Włącz,** a następnie **przycisk Tak w** polu ostrzeżenia.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="9c9d3-106">Przejdź do [**Centrum administracyjnego programu Exchange, > zarządzania zgodnością > tagami przechowywania.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="9c9d3-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="9c9d3-107">Wybierz ikonę +, a następnie wybierz **pozycję Automatycznie zastosuj do całej skrzynki pocztowej.**</span><span class="sxs-lookup"><span data-stu-id="9c9d3-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="9c9d3-108">Przypisz nazwę do tagu przechowywania i wybierz pozycję **Przenieś do archiwum.**</span><span class="sxs-lookup"><span data-stu-id="9c9d3-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="9c9d3-109">W okresie przechowywania wprowadź czas, na przykład 90 dni.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="9c9d3-110">Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-110">Click **Save**.</span></span>
5. <span data-ttu-id="9c9d3-111">Teraz utwórz zasady przechowywania: wybierz **zasady przechowywania,** wybierz ikonę, aby dodać nowe zasady.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="9c9d3-112">Przypisz nazwę do zasad przechowywania, a następnie kliknij i przewiń, aby znaleźć i dodać właśnie utworzony tag przechowywania.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="9c9d3-113">Kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="9c9d3-113">Click **Save**.</span></span>
7. <span data-ttu-id="9c9d3-114">Na koniec zastosuj zasady przechowywania do skrzynki pocztowej użytkownika: nadal w centrum administracyjnym programu Exchange przejdź do **skrzynek**  >  **pocztowych adresatów.**</span><span class="sxs-lookup"><span data-stu-id="9c9d3-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="9c9d3-115">Wybierz wszystkich użytkowników, do których chcesz zastosować zasady, a następnie wybierz pozycję **Edytuj** (ikona ołówka).</span><span class="sxs-lookup"><span data-stu-id="9c9d3-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="9c9d3-116">W oknie dialogowym kliknij pozycję **Funkcje skrzynki pocztowej.**</span><span class="sxs-lookup"><span data-stu-id="9c9d3-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="9c9d3-117">W **obszarze Zasady przechowywania** zastosuj zasady, które właśnie zostały > **Zapisz.**</span><span class="sxs-lookup"><span data-stu-id="9c9d3-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="9c9d3-118">Aby uzyskać instrukcje dotyczące stosowania zasad do wszystkich użytkowników, zobacz [Stosowanie zasad przechowywania do skrzynek pocztowych.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="9c9d3-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
