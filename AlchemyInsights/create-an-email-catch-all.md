---
title: Tworzenie wiadomości e-mail catch wszystkich
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286202"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="34793-102">Tworzenie wiadomości e-mail catch wszystkich</span><span class="sxs-lookup"><span data-stu-id="34793-102">Create an email catch all</span></span>

<span data-ttu-id="34793-103">Korzystanie z połowu wszystko jest zdecydowanie odradzane.</span><span class="sxs-lookup"><span data-stu-id="34793-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="34793-104">Lepiej jest zapewnić odbicie z powrotem do nadawcy, informując nadawców, że ich wiadomość nie może zostać dostarczona jako adresowana, aby mogli podjąć działania.</span><span class="sxs-lookup"><span data-stu-id="34793-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="34793-105">Można również ograniczyć monitorowana skrzynka pocztowa, aby tylko wyłapywać wcześniej prawidłowe adresy e-mail.</span><span class="sxs-lookup"><span data-stu-id="34793-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="34793-106">Każdy połów wszystkie skrzynki pocztowej otrzyma sporo spamu i może ostatecznie wypełnić, jeśli nie ściśle monitorowane.</span><span class="sxs-lookup"><span data-stu-id="34793-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="34793-107">(Istnieją limity odbioru.)</span><span class="sxs-lookup"><span data-stu-id="34793-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="34793-108">Jeśli zdecydujesz się kontynuować, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="34793-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="34793-109">Utwórz dynamiczną grupę dystrybucyjną & zawierać "Wszystkie typy adresatów".</span><span class="sxs-lookup"><span data-stu-id="34793-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="34793-110">Utwórz dedykowaną skrzynkę pocztową, aby wyłapywać wiadomości e-mail, na przykład catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="34793-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="34793-111">W przypadku określonej domeny ustaw DomainType na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="34793-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="34793-112">Jeśli później usuniesz wszystkie catch, należy ustawić domenę z powrotem do autorytatywne.</span><span class="sxs-lookup"><span data-stu-id="34793-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="34793-113">Utwórz regułę transportu przepływów mailowych w następujący sposób:</span><span class="sxs-lookup"><span data-stu-id="34793-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="34793-114">Jeśli nadawca jest "Poza organizacją"</span><span class="sxs-lookup"><span data-stu-id="34793-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="34793-115">Przekieruj wiadomość do Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="34793-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="34793-116">Z wyjątkiem sytuacji, gdy odbiorca jest członkiem allusers@domain.com (Grupa dystrybucyjna zawiera wszystkich członków)</span><span class="sxs-lookup"><span data-stu-id="34793-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="34793-117">Upewnij się, że nowe skrzynki pocztowe są dodawane do dynamicznej grupy dystrybucyjnej</span><span class="sxs-lookup"><span data-stu-id="34793-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
