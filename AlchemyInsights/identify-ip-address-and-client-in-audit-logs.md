---
title: Identyfikowanie adresu IP i klienta w dziennikach inspekcji
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668320"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="88107-102">Identyfikowanie adresu IP i klienta w dziennikach inspekcji</span><span class="sxs-lookup"><span data-stu-id="88107-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="88107-103">W dziennikach inspekcji jest wyświetlany adres IP, który odpowiada działaniu użytkownika lub administratora usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="88107-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="88107-104">Informacje dotyczące klienta są również rejestrowane.</span><span class="sxs-lookup"><span data-stu-id="88107-104">The client information is also logged.</span></span> <span data-ttu-id="88107-105">Poniżej przedstawiono procedurę identyfikowania takich informacji</span><span class="sxs-lookup"><span data-stu-id="88107-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="88107-106">Zaloguj się do [Centrum zabezpieczeń & programu Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="88107-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="88107-107">Przejdź do strony **Search**  >  **wyszukiwania dziennika inspekcji** wyszukiwania.</span><span class="sxs-lookup"><span data-stu-id="88107-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="88107-108">Jeśli chcesz skorzystać z określonej czynności, wybierz ją z listy **działań** .</span><span class="sxs-lookup"><span data-stu-id="88107-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="88107-109">Jeśli nie, wszystkie działania zostaną zwrócone dla wybranego użytkownika (ustawienie domyślne).</span><span class="sxs-lookup"><span data-stu-id="88107-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="88107-110">**Uwaga**: niektóre działania mogą nie być dostępne w menu **działania** ; Jednak te elementy inspekcji zostaną zwrócone, jeśli wybrano opcję **Pokaż wyniki dla wszystkich działań** (ustawienie domyślne).</span><span class="sxs-lookup"><span data-stu-id="88107-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="88107-111">Określ nazwę użytkownika w polu **Użytkownicy** , wybierz odpowiedni zakres dat dla działania, a następnie kliknij przycisk **Wyszukaj**.</span><span class="sxs-lookup"><span data-stu-id="88107-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="88107-112">W wynikach wyszukiwania w okienku wyniki jest widoczny adres IP dla tego działania.</span><span class="sxs-lookup"><span data-stu-id="88107-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="88107-113">Wybierz rekord inspekcji, aby wyświetlić szczegółowe informacje w menu wysuwanym **szczegóły** (na przykład klient, użytkownik, który wykonał akcję itd.).</span><span class="sxs-lookup"><span data-stu-id="88107-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="88107-114">Aby uzyskać więcej informacji, zobacz [Znajdowanie adresu IP komputera, za pomocą którego można uzyskać dostęp do złamanego konta](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="88107-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
