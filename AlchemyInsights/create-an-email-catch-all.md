---
title: Utwórz wiadomość e-mail, aby wszystkie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816210"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="dc508-102">Utwórz wiadomość e-mail, aby wszystkie</span><span class="sxs-lookup"><span data-stu-id="dc508-102">Create an email catch all</span></span>

<span data-ttu-id="dc508-103">Korzystanie z tego wszystkiego jest stanowczo zalecane.</span><span class="sxs-lookup"><span data-stu-id="dc508-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="dc508-104">Lepiej wrócić do nadawcy, aby nadawca wiedział, że jego wiadomość nie może zostać dostarczona jako zaadresowana, aby mogli podjąć działania.</span><span class="sxs-lookup"><span data-stu-id="dc508-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="dc508-105">Monitorowaną skrzynkę pocztową można również ograniczyć do tylko tych, które wcześniej były prawidłowe.</span><span class="sxs-lookup"><span data-stu-id="dc508-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="dc508-106">Każdy chwyć całą skrzynkę pocztową otrzyma dużo spamu i może zostać w końcu zapełnienie, jeśli nie będzie ściśle monitorowane.</span><span class="sxs-lookup"><span data-stu-id="dc508-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="dc508-107">(Istnieją limity).</span><span class="sxs-lookup"><span data-stu-id="dc508-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="dc508-108">Jeśli zdecydujesz się kontynuować, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="dc508-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="dc508-109">Utwórz dynamiczną grupę dystrybucyjną, & dołącz "Wszystkie typy adresatów".</span><span class="sxs-lookup"><span data-stu-id="dc508-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="dc508-110">Utwórz dedykowaną skrzynkę pocztową, aby chwyć wiadomości e-mail, na catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="dc508-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="dc508-111">Dla określonej domeny ustaw dla ustawienia DomainType wartość "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="dc508-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="dc508-112">Jeśli później usuniesz wszystkie ustawienia, upewnij się, że domena ma ustawioną wartość Autorytatywny.</span><span class="sxs-lookup"><span data-stu-id="dc508-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="dc508-113">Utwórz regułę transportu przepływu poczty e-mail w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="dc508-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="dc508-114">Jeśli nadawca to "Spoza organizacji"</span><span class="sxs-lookup"><span data-stu-id="dc508-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="dc508-115">Przekieruj wiadomość do Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="dc508-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="dc508-116">Za wyjątkiem, jeśli adresat jest członkiem grupy allusers@domain.com (grupa dystrybucyjna zawiera wszystkich członków)</span><span class="sxs-lookup"><span data-stu-id="dc508-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="dc508-117">Sprawdzanie, czy nowe skrzynki pocztowe zostały dodane do dynamicznej grupy dystrybucyjnej</span><span class="sxs-lookup"><span data-stu-id="dc508-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
