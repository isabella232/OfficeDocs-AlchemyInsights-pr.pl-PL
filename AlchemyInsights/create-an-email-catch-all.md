---
title: Tworzenie wiadomości e-mail z całą połową
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712996"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="fd57e-102">Tworzenie wiadomości e-mail z całą połową</span><span class="sxs-lookup"><span data-stu-id="fd57e-102">Create an email catch all</span></span>

<span data-ttu-id="fd57e-103">Korzystanie z funkcji catch all nie jest zalecane.</span><span class="sxs-lookup"><span data-stu-id="fd57e-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="fd57e-104">Lepszym rozwiązaniem jest dostarczenie odskakującego przeskoku nadawcy informującego, że nadawcy nie będą wiedzieli, że mogą podjąć działania.</span><span class="sxs-lookup"><span data-stu-id="fd57e-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="fd57e-105">Możesz również ograniczyć monitorowaną skrzynkę pocztową tylko do połowów, które były wcześniej prawidłowymi adresami e-mail.</span><span class="sxs-lookup"><span data-stu-id="fd57e-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="fd57e-106">Każda Skrzynka pocztowa będzie otrzymywać dobrą okazję do spamu i może ostatecznie wypełnić, jeśli nie jest ściśle monitorowana.</span><span class="sxs-lookup"><span data-stu-id="fd57e-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="fd57e-107">(Istnieją limity dotyczące odbierania).</span><span class="sxs-lookup"><span data-stu-id="fd57e-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="fd57e-108">Jeśli zdecydujesz się kontynuować, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="fd57e-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="fd57e-109">Utwórz dynamiczną grupę dystrybucyjną, & dołączyć "wszystkie typy adresatów".</span><span class="sxs-lookup"><span data-stu-id="fd57e-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="fd57e-110">Utwórz dedykowaną skrzynkę pocztową do obsługi wiadomości e-mail, na przykład catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="fd57e-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="fd57e-111">W przypadku określonej domeny ustaw dla tej usługi wartość "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="fd57e-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="fd57e-112">Jeśli później usuniesz przechwycenie, upewnij się, że domena jest ponownie ustawiona na wartość autorytatywna.</span><span class="sxs-lookup"><span data-stu-id="fd57e-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="fd57e-113">Utwórz regułę transportu o w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="fd57e-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="fd57e-114">Jeśli nadawca to "spoza organizacji"</span><span class="sxs-lookup"><span data-stu-id="fd57e-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="fd57e-115">Przekierowywanie wiadomości do Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="fd57e-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="fd57e-116">Chyba że adresat jest członkiem allusers@domain.com (grupa dystrybucyjna zawiera wszystkich członków)</span><span class="sxs-lookup"><span data-stu-id="fd57e-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="fd57e-117">Sprawdzanie, czy nowe skrzynki pocztowe są dodawane do grupy dystrybucyjnej dynamicznej</span><span class="sxs-lookup"><span data-stu-id="fd57e-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
