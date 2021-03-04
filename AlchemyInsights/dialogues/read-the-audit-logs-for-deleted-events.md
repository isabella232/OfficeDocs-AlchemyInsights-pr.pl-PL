---
title: Odczytywanie dzienników inspekcji usuniętych zdarzeń
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429827"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="cc52b-102">Odczytywanie dzienników inspekcji usuniętych zdarzeń</span><span class="sxs-lookup"><span data-stu-id="cc52b-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="cc52b-103">Poniżej opisano, jak to zrobić:</span><span class="sxs-lookup"><span data-stu-id="cc52b-103">Here's how to do this:</span></span>

1. <span data-ttu-id="cc52b-104">Przejdź do Centrum [zabezpieczeń usługi Office 365 & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="cc52b-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="cc52b-105">Wybierz **pozycję**  >  [**Przeszukiwanie dziennika inspekcji.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="cc52b-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="cc52b-106">Jeśli zobaczysz powiadomienie, że musisz włączyć tę funkcję, możesz ją włączyć już teraz.</span><span class="sxs-lookup"><span data-stu-id="cc52b-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="cc52b-107">Jeśli funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły wyciągać danych z poprzednich dat.</span><span class="sxs-lookup"><span data-stu-id="cc52b-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="cc52b-108">Wybierz **pozycję Działania,** a następnie znajdź działania **skrzynki pocztowej programu Exchange.**</span><span class="sxs-lookup"><span data-stu-id="cc52b-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="cc52b-109">Wybierz opcje **Folderu Elementy usunięte i** Przenieś wiadomości **do** folderu Elementy usunięte.</span><span class="sxs-lookup"><span data-stu-id="cc52b-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="cc52b-110">Gdy to zrobisz, kliknij poza okienkiem, aby zminimalizować okienko **Działania.**</span><span class="sxs-lookup"><span data-stu-id="cc52b-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="cc52b-111">Określ zakres dat, a  następnie w polu Użytkownicy wybierz nazwę użytkownika, którego chcesz zbadać.</span><span class="sxs-lookup"><span data-stu-id="cc52b-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="cc52b-112">Możesz wybrać więcej niż jednego użytkownika na raz.</span><span class="sxs-lookup"><span data-stu-id="cc52b-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="cc52b-113">Wybierz **pozycję Wyszukaj.**</span><span class="sxs-lookup"><span data-stu-id="cc52b-113">Select **Search**.</span></span> <span data-ttu-id="cc52b-114">Działania zostaną wyświetlone w obszarze **Wyniki.**</span><span class="sxs-lookup"><span data-stu-id="cc52b-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="cc52b-115">Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz **pozycję Więcej informacji.**</span><span class="sxs-lookup"><span data-stu-id="cc52b-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="cc52b-116">W polu Elementy, których dotyczy problem, są wyświetlane dodatkowe informacje o usuniętym elementie, takie jak wiersz tematu i lokalizacja **usuniętego** elementu.</span><span class="sxs-lookup"><span data-stu-id="cc52b-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="cc52b-117">Za pomocą funkcji dziennika inspekcji nie można przywrócić usuniętych elementów.</span><span class="sxs-lookup"><span data-stu-id="cc52b-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="cc52b-118">Aby przywrócić usunięte elementy, zobacz [Odzyskiwanie usuniętych elementów lub wiadomości e-mail w aplikacji Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="cc52b-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="cc52b-119">Aby dowiedzieć się więcej, zobacz Przeszukiwanie dziennika inspekcji usługi [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)w celu rozwiązania typowych scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="cc52b-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
