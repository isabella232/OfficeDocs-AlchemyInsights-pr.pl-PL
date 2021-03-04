---
title: Znajdowanie adresu IP w dzienniku inspekcji
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429786"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="bb022-102">Znajdowanie adresu IP w dzienniku inspekcji</span><span class="sxs-lookup"><span data-stu-id="bb022-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="bb022-103">Adres IP odpowiadający działaniu wykonanemu przez użytkownika lub administratora jest wyświetlany w dziennikach inspekcji.</span><span class="sxs-lookup"><span data-stu-id="bb022-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="bb022-104">Rejestrowane są również informacje o kliencie.</span><span class="sxs-lookup"><span data-stu-id="bb022-104">The client information is also logged.</span></span> <span data-ttu-id="bb022-105">Oto jak zidentyfikować adres IP:</span><span class="sxs-lookup"><span data-stu-id="bb022-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="bb022-106">Przejdź do Centrum [zabezpieczeń usługi Office 365 & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="bb022-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="bb022-107">Wybierz **pozycję**  >  **[Przeszukiwanie dziennika inspekcji.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="bb022-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="bb022-108">Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz ją włączyć już teraz.</span><span class="sxs-lookup"><span data-stu-id="bb022-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="bb022-109">Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły wyciągać danych z poprzednich dat.</span><span class="sxs-lookup"><span data-stu-id="bb022-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="bb022-110">Jeśli interesuje Cię określone działanie, wybierz je z **listy Działania.** w przeciwnym razie domyślnie wszystkie działania zostaną zwrócone dla wybranego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="bb022-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="bb022-111">Pamiętaj, że niektóre działania mogą nie być dostępne do wyboru z menu **Działania;** jednak te elementy inspekcji zostaną zwrócone, jeśli wybrano opcję Pokaż wyniki dla **wszystkich** działań (ustawienie domyślne).</span><span class="sxs-lookup"><span data-stu-id="bb022-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="bb022-112">Określ zakres dat, a  następnie w polu Użytkownicy wybierz nazwę użytkownika, którego chcesz zbadać.</span><span class="sxs-lookup"><span data-stu-id="bb022-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="bb022-113">Wybierz **pozycję Wyszukaj.**</span><span class="sxs-lookup"><span data-stu-id="bb022-113">Select **Search**.</span></span> <span data-ttu-id="bb022-114">Działania zostaną wyświetlone w obszarze **Wyniki.**</span><span class="sxs-lookup"><span data-stu-id="bb022-114">The activities appear under **Results**.</span></span> <span data-ttu-id="bb022-115">Możesz wyświetlić adresy IP poszczególnych działań.</span><span class="sxs-lookup"><span data-stu-id="bb022-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="bb022-116">Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz **pozycję Więcej informacji.**</span><span class="sxs-lookup"><span data-stu-id="bb022-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="bb022-117">Aby dowiedzieć się więcej, zobacz Przeszukiwanie dziennika inspekcji usługi [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)w celu rozwiązania typowych scenariuszy.</span><span class="sxs-lookup"><span data-stu-id="bb022-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>