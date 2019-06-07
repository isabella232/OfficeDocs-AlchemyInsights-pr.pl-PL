---
title: Określenie adresu IP i klienta w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752069"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="90bc9-102">Określenie adresu IP i klienta w dziennikach inspekcji</span><span class="sxs-lookup"><span data-stu-id="90bc9-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="90bc9-103">Adres IP, który odpowiada do działania przez użytkownika lub administratora jest wyświetlane w dziennikach inspekcji.</span><span class="sxs-lookup"><span data-stu-id="90bc9-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="90bc9-104">Rejestrowane są również informacje klienta.</span><span class="sxs-lookup"><span data-stu-id="90bc9-104">The client information is also logged.</span></span> <span data-ttu-id="90bc9-105">Poniżej przedstawiono kroki, aby takie informacje identyfikacyjne</span><span class="sxs-lookup"><span data-stu-id="90bc9-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="90bc9-106">Zaloguj się do [Centrum zgodności Office 365 zabezpieczeń &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="90bc9-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="90bc9-107">Kliknij przycisk **Wyszukaj i dochodzenia** i wybierz **Przeszukiwania dzienników inspekcji**.</span><span class="sxs-lookup"><span data-stu-id="90bc9-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="90bc9-108">Jeśli interesują Cię określone działanie, wybierz go z listy **działań** .</span><span class="sxs-lookup"><span data-stu-id="90bc9-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="90bc9-109">W przeciwnym razie zostaną zwrócone wszystkie działania dla wybranego użytkownika (ustawienie domyślne).</span><span class="sxs-lookup"><span data-stu-id="90bc9-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="90bc9-110">**Uwaga**: niektóre rodzaje działalności mogą nie być dostępne w menu **działań** ; Jednakże inspekcja tych elementów zostaną zwrócone, jeśli **Pokaż wyniki dla wszystkich działalności** jest wybrany (ustawienie domyślne).</span><span class="sxs-lookup"><span data-stu-id="90bc9-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="90bc9-111">Określ nazwę użytkownika w polu **Użytkownicy** , wybierz zakres dat odpowiednie działania i kliknij przycisk **Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="90bc9-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="90bc9-112">W wynikach można zobaczyć adres IP dla tego działania w okienku wyników.</span><span class="sxs-lookup"><span data-stu-id="90bc9-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="90bc9-113">Wybierz rekord audytu, aby zobaczyć szczegółowe informacje w menu wysuwane **Szczegóły** (na przykład klienta, użytkownika, która wykonywana akcja, itp.).</span><span class="sxs-lookup"><span data-stu-id="90bc9-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="90bc9-114">Aby uzyskać więcej informacji zobacz [Znajdowanie adresu IP komputera umożliwia dostęp do skierowanego na to konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="90bc9-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
