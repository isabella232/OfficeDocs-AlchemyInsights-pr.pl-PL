---
title: Problem z atrybutem i filtrem zakresu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481897"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="25e9f-102">Problem z atrybutami i filtrowaniem zakresu</span><span class="sxs-lookup"><span data-stu-id="25e9f-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="25e9f-103">**Problem z wartościami upn powodujące konflikt**</span><span class="sxs-lookup"><span data-stu-id="25e9f-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="25e9f-104">W dzień roboczy inicjowania obsługi administracyjnej użytkownika usługi AD w trybie inicjowania obsługi administracyjnej użytkownika usługi AD jest wyświetlany komunikat o błędzie **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="25e9f-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="25e9f-105">Operacja nie powiodła się, ponieważ główna wartość w zakresie dodatku/modyfikacji nie jest unikatowa dla całego lasu.</span><span class="sxs-lookup"><span data-stu-id="25e9f-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="25e9f-106">Szczegóły błędu: **CONSTRAINT_ATT_TYPE — userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="25e9f-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="25e9f-107">Wartość **userPrincipalName,** która próbuje ustawić łącznik dzień roboczy podczas tworzenia konta użytkownika usługi AD, już istnieje w docelowej domenie usługi AD.</span><span class="sxs-lookup"><span data-stu-id="25e9f-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="25e9f-108">Oznacza to, że użytkownik (1) już istnieje i nie udało się sprawdzić pasującego identyfikatora przez użytkownika lub (2) reguła generowania upn wygenerowała wartość kolidującą.</span><span class="sxs-lookup"><span data-stu-id="25e9f-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="25e9f-109">Poniżej podano sugerowane kroki rozwiązania problemu:</span><span class="sxs-lookup"><span data-stu-id="25e9f-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="25e9f-110">Jeśli użytkownik już istnieje, a nie udało się połączyć konta w dzień roboczy z kontem usługi Active Directory, sprawdź, czy zgodny atrybut identyfikatora (zwykle **identyfikator** pracownika) zarówno w dzień roboczy, jak i w usłudze AD ma dokładne dopasowanie.</span><span class="sxs-lookup"><span data-stu-id="25e9f-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="25e9f-111">Jeśli nie ma dopasowania, problem z danymi należy rozwiązać.</span><span class="sxs-lookup"><span data-stu-id="25e9f-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="25e9f-112">Jeśli na przykład identyfikator pracownika w dniu pracy to 001052, a w u użytkownikach AD jest to 1052, aparat obsługi administracyjnej nie połączy tych dwóch kont i spróbuje utworzyć użytkownika, który już istnieje.</span><span class="sxs-lookup"><span data-stu-id="25e9f-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="25e9f-113">W tym przypadku rozwiązaniem jest zmiana wartości **Identyfikator** pracownika w u użytkownikach w u użytkownikach AD tak, aby zawierała zera wiodące, aby była równa 001052.</span><span class="sxs-lookup"><span data-stu-id="25e9f-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="25e9f-114">Jeśli wyrażenie generujące upn nie generuje unikatowej wartości, rozważ każdorazowe wygenerowanie unikatowej wartości przy użyciu funkcji de duplikowania **SelectUniqueValue.**</span><span class="sxs-lookup"><span data-stu-id="25e9f-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="25e9f-115">**Inicjowanie obsługi użytkowników w dni robocze do usługi AD nie powoduje ustawienia wartości atrybutu menedżera dla konta użytkownika usługi AD**</span><span class="sxs-lookup"><span data-stu-id="25e9f-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="25e9f-116">Zadanie inicjowania obsługi użytkowników usługi AD w dzień roboczy nie ustawia wartości atrybutu **menedżera** dla kont użytkowników usługi AD.</span><span class="sxs-lookup"><span data-stu-id="25e9f-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="25e9f-117">Takie zachowanie jest widoczne w dwóch scenariuszach:</span><span class="sxs-lookup"><span data-stu-id="25e9f-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="25e9f-118">Kierownika w dzień roboczy nie można rozpoznać do odpowiadającego mu konta użytkownika usługi AD, ponieważ menedżer nie znajduje się w zakresie.</span><span class="sxs-lookup"><span data-stu-id="25e9f-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="25e9f-119">W **scenariuszu z wieloma domenami** usługi AD kierownik w dzień roboczy nie występuje w tej samej domenie co użytkownik.</span><span class="sxs-lookup"><span data-stu-id="25e9f-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="25e9f-120">Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="25e9f-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="25e9f-121">Jeśli zdefiniowano zakres filtrów, najpierw sprawdź, czy menedżer znajduje się w zakresie i spełnia warunki określone w klauzuli zakresu.</span><span class="sxs-lookup"><span data-stu-id="25e9f-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="25e9f-122">Jeśli menedżer nie spełnia filtru zakresu, zmień filtr tak, aby menedżer również był w zakresie operacji inicjowania obsługi administracyjnej.</span><span class="sxs-lookup"><span data-stu-id="25e9f-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="25e9f-123">Jeśli masz wiele domen usługi AD, łącznik ma znane ograniczenie, które ma problemy z rozwiązywanie odwołań między menedżerami domen.</span><span class="sxs-lookup"><span data-stu-id="25e9f-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="25e9f-124">Aby uzyskać więcej szczegółowych informacji na temat konfigurowania dnia roboczego dla automatycznego inicjowania obsługi, zobacz Samouczek: Konfigurowanie dnia roboczego dla [automatycznego inicjowania obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="25e9f-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













