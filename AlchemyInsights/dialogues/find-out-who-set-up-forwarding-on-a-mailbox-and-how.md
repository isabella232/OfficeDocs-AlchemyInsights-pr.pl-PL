---
title: Dowiedz się, kto i jak skonfigurować przesyłanie dalej w skrzynce pocztowej
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429990"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="31517-102">Dowiedz się, kto i jak skonfigurować przesyłanie dalej w skrzynce pocztowej</span><span class="sxs-lookup"><span data-stu-id="31517-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="31517-103">Jeśli w skrzynce pocztowej ustawiono zewnętrzne przesyłanie dalej, to działanie jest raportowane w Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="31517-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="31517-104">Poniżej opisano, jak można znaleźć działanie w dzienniku inspekcji:</span><span class="sxs-lookup"><span data-stu-id="31517-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="31517-105">Przejdź do Centrum [zabezpieczeń usługi Office 365 & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="31517-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="31517-106">Wybierz **pozycję** >  **Przeszukiwanie dziennika inspekcji.**</span><span class="sxs-lookup"><span data-stu-id="31517-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="31517-107">Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz ją włączyć już teraz.</span><span class="sxs-lookup"><span data-stu-id="31517-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="31517-108">Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły wyciągać danych z poprzednich dat.</span><span class="sxs-lookup"><span data-stu-id="31517-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="31517-109">Upewnij się, **że pole Działania** ma ustawioną wartość Pokaż wyniki dla wszystkich **działań** (ustawienie domyślne).</span><span class="sxs-lookup"><span data-stu-id="31517-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="31517-110">Określ zakres dat.</span><span class="sxs-lookup"><span data-stu-id="31517-110">Specify the date range.</span></span> <span data-ttu-id="31517-111">Nie musisz określać nazwy użytkownika.</span><span class="sxs-lookup"><span data-stu-id="31517-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="31517-112">Wybierz **pozycję Wyszukaj.**</span><span class="sxs-lookup"><span data-stu-id="31517-112">Select **Search**.</span></span> <span data-ttu-id="31517-113">Działania zostaną wyświetlone w obszarze **Wyniki.**</span><span class="sxs-lookup"><span data-stu-id="31517-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="31517-114">Wybierz **pozycję Filtruj** wyniki, a następnie **wprowadź pole Ustaw skrzynkę** pocztową w **polu** Filtr aktywności.</span><span class="sxs-lookup"><span data-stu-id="31517-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="31517-115">W ten sposób są **zwracane wszystkie działania typu Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="31517-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="31517-116">Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz **pozycję Więcej informacji.**</span><span class="sxs-lookup"><span data-stu-id="31517-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="31517-117">W **obszarze** Parametry możesz zobaczyć adres e-mail przesyłania dalej ustawiony w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="31517-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="31517-118">Identyfikator **użytkownika reprezentuje** użytkownika, który schowa zewnętrzne przesyłanie dalej w skrzynce pocztowej.</span><span class="sxs-lookup"><span data-stu-id="31517-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="31517-119">Aby dowiedzieć się więcej, zobacz Przeszukiwanie dziennika inspekcji usługi [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)w celu rozwiązania typowych scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="31517-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>