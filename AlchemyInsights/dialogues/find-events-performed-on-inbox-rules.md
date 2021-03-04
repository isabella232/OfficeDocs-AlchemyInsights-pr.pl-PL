---
title: Znajdowanie zdarzeń wykonanych w zasadach skrzynki odbiorczej
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430012"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="23b65-102">Znajdowanie zdarzeń wykonanych w zasadach skrzynki odbiorczej</span><span class="sxs-lookup"><span data-stu-id="23b65-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="23b65-103">Podczas tworzenia, zmieniania lub usuwania reguł skrzynki odbiorczej zdarzenia są rejestrowane w dzienniku inspekcji.</span><span class="sxs-lookup"><span data-stu-id="23b65-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="23b65-104">Oto jak je przejrzeć:</span><span class="sxs-lookup"><span data-stu-id="23b65-104">Here's how to review them:</span></span>

1. <span data-ttu-id="23b65-105">Przejdź do Centrum [zabezpieczeń usługi Office 365 & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="23b65-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="23b65-106">Wybierz pozycję Wyszukiwanie > przeszukiwanie dziennika inspekcji.</span><span class="sxs-lookup"><span data-stu-id="23b65-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="23b65-107">Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz ją włączyć już teraz.</span><span class="sxs-lookup"><span data-stu-id="23b65-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="23b65-108">Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły wyciągać danych z poprzednich dat.</span><span class="sxs-lookup"><span data-stu-id="23b65-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="23b65-109">Wybierz pole Działania i znajdź działania skrzynki pocztowej programu Exchange, a następnie wybierz pozycję New-InboxRule Utwórz regułę skrzynki odbiorczej w aplikacji Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="23b65-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="23b65-110">Gdy to zrobisz, kliknij poza okienkiem, aby zminimalizować okienko Działania.</span><span class="sxs-lookup"><span data-stu-id="23b65-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="23b65-111">Określ zakres dat, a następnie w polu Użytkownicy wybierz nazwę użytkownika, którego chcesz zbadać.</span><span class="sxs-lookup"><span data-stu-id="23b65-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="23b65-112">Możesz wybrać więcej niż jednego użytkownika na raz.</span><span class="sxs-lookup"><span data-stu-id="23b65-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="23b65-113">Wybierz pozycję Wyszukaj.</span><span class="sxs-lookup"><span data-stu-id="23b65-113">Select Search.</span></span> <span data-ttu-id="23b65-114">Działania zostaną wyświetlone w obszarze Wyniki.</span><span class="sxs-lookup"><span data-stu-id="23b65-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="23b65-115">Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz pozycję Więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="23b65-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="23b65-116">W sekcji Parametry możesz zobaczyć nazwę reguły, zestaw warunków i akcje, które będą podejmowane przez regułę.</span><span class="sxs-lookup"><span data-stu-id="23b65-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="23b65-117">Aby dowiedzieć się więcej, zobacz Przeszukiwanie dziennika inspekcji usługi Office 365 w celu rozwiązania typowych scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="23b65-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>