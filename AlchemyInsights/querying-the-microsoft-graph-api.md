---
title: Badanie interfejsu API programu Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974681"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="53a29-102">Badanie interfejsu API programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="53a29-103">Ten temat może również dotyczyć deweloperów korzystających z interfejsu API Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="53a29-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="53a29-104">Jednak **stanowczo** zaleca się korzystanie z programu Microsoft Graph we wszystkich scenariuszach dotyczących katalogów, tożsamości i zarządzania dostępem.</span><span class="sxs-lookup"><span data-stu-id="53a29-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="53a29-105">**Problemy z uwierzytelnianiem lub autoryzacją**</span><span class="sxs-lookup"><span data-stu-id="53a29-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="53a29-106">Jeśli aplikacja **nie może uzyskać tokenów** w celu nawiązania połączenia z programem Microsoft Graph, wybierz pozycję problem, aby uzyskać bardziej szczegółową pomoc i obsługę techniczną dotyczącą tego tematu, wybierając kategorię Microsoft Graph **token (uwierzytelnianie)** .</span><span class="sxs-lookup"><span data-stu-id="53a29-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="53a29-107">Jeśli aplikacja otrzymuje **Błędy autoryzacji usługi 401 lub 403** podczas nawiązywania połączenia z programem Microsoft Graph, wybierz kategorię **błąd podczas uzyskiwania dostępu** do aplikacji Microsoft Graph API, aby uzyskać bardziej właściwą pomoc i obsługę techniczną w tym temacie.</span><span class="sxs-lookup"><span data-stu-id="53a29-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="53a29-108">**Chcę używać programu Microsoft Graph, ale nie wiesz, gdzie zacząć**</span><span class="sxs-lookup"><span data-stu-id="53a29-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="53a29-109">Aby uzyskać więcej informacji na temat programu Microsoft Graph, zobacz:</span><span class="sxs-lookup"><span data-stu-id="53a29-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="53a29-110">Omówienie programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="53a29-111">Omówienie zarządzania tożsamościami i dostępem w programie Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="53a29-112">Wprowadzenie do tworzenia aplikacji Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="53a29-113">**Eksplorator Microsoft Graph** -testowanie interfejsów API programu Microsoft Graph w dzierżawie lub w dzierżawie demonstracyjnej</span><span class="sxs-lookup"><span data-stu-id="53a29-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="53a29-114">**Chcę używać programu Microsoft Graph, ale obsługuje on interfejsy API katalogów v 1.0?**</span><span class="sxs-lookup"><span data-stu-id="53a29-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="53a29-115">Program Microsoft Graph to zalecany interfejs API dla katalogu, tożsamości i zarządzania dostępem.</span><span class="sxs-lookup"><span data-stu-id="53a29-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="53a29-116">Jednak w przypadku programu Azure AD Graph i Microsoft Graph nadal są dostępne niewiele przerw.</span><span class="sxs-lookup"><span data-stu-id="53a29-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="53a29-117">Zapoznaj się z następującymi artykułami, które wyróżnią najbardziej aktualne różnice, aby pomóc w wyborze:</span><span class="sxs-lookup"><span data-stu-id="53a29-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="53a29-118">Różnice typów zasobów na platformie Azure AD Graph i w programie Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="53a29-119">Różnice między właściwościami programu Azure AD Graph a programem Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="53a29-120">Różnice między metodami Azure AD i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="53a29-121">**Podczas wysyłania zapytania do obiektu *użytkownika* brakuje wielu jego właściwości**</span><span class="sxs-lookup"><span data-stu-id="53a29-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="53a29-122">`GET https://graph.microsoft.com/v1.0/users` zwraca tylko 11 właściwości, ponieważ program Microsoft Graph automatycznie wybiera domyślny zestaw właściwości *użytkownika* , które mają zostać zwrócone.</span><span class="sxs-lookup"><span data-stu-id="53a29-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="53a29-123">Jeśli potrzebujesz innych właściwości *użytkownika* , użyj $SELECT, aby wybrać właściwości, których potrzebuje aplikacja.</span><span class="sxs-lookup"><span data-stu-id="53a29-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="53a29-124">Najpierw wypróbuj **program Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="53a29-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="53a29-125">**Niektóre wartości właściwości użytkownika mają *wartość null* , mimo że wiemy, że są ustawione**</span><span class="sxs-lookup"><span data-stu-id="53a29-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="53a29-126">Najbardziej prawdopodobnym wyjaśnieniem jest to, że dla aplikacji udzielono uprawnienia *User. ReadBasic. All* .</span><span class="sxs-lookup"><span data-stu-id="53a29-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="53a29-127">Umożliwia to aplikacji odczytywanie ograniczonego zestawu właściwości użytkownika i zwracanie wszystkich innych właściwości jako wartości null, nawet jeśli zostały one wcześniej ustawione.</span><span class="sxs-lookup"><span data-stu-id="53a29-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="53a29-128">Spróbuj udzielić użytkownikowi aplikacji *. Przeczytaj. wszystkie* uprawnienia.</span><span class="sxs-lookup"><span data-stu-id="53a29-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="53a29-129">Aby uzyskać więcej informacji, zobacz [uprawnienia użytkownika programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="53a29-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="53a29-130">**Występują problemy z używaniem parametrów zapytania OData w celu filtrowania danych w moich żądaniach**</span><span class="sxs-lookup"><span data-stu-id="53a29-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="53a29-131">Gdy program Microsoft Graph obsługuje szeroki zakres parametrów zapytania OData, wiele z tych parametrów nie jest w pełni obsługiwane przez usługi katalogowe (zasoby dziedziczące po elemencie *directoryobject*) w programie Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="53a29-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="53a29-132">Te same ograniczenia, które były dostępne w programie Azure AD Graph, są zachowywane w większości części programu Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="53a29-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="53a29-133">**Nieobsługiwane**: $count, $search i $Filter wartości *null* lub *not null*</span><span class="sxs-lookup"><span data-stu-id="53a29-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="53a29-134">**Nieobsługiwane**: $Filter niektórych właściwości (zobacz tematy dotyczące zasobów, na których właściwości można filtrować)</span><span class="sxs-lookup"><span data-stu-id="53a29-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="53a29-135">**Nieobsługiwane**: stronicowanie, filtrowanie i sortowanie w tym samym czasie</span><span class="sxs-lookup"><span data-stu-id="53a29-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="53a29-136">**Nieobsługiwane**: filtrowanie w relacji.</span><span class="sxs-lookup"><span data-stu-id="53a29-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="53a29-137">Na przykład — Znajdź wszystkich członków grupy inżynierskiej w Wielkiej Brytanii.</span><span class="sxs-lookup"><span data-stu-id="53a29-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="53a29-138">**Pomoc techniczna częściowa**: $OrderBy dla *użytkownika* (DisplayName, tylko userPrincipalName) i *Group*</span><span class="sxs-lookup"><span data-stu-id="53a29-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="53a29-139">**Pomoc techniczna częściowa**: $Filter (obsługiwana tylko *w przypadku funkcji* *EQ*, *StartsWith* *lub*( *i*), $expand (rozwinięcie relacji pojedynczego obiektu zwraca wszystkie relacje, ale rozwijanie kolekcji obiektów) jest ograniczone.</span><span class="sxs-lookup"><span data-stu-id="53a29-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="53a29-140">Aby uzyskać więcej informacji, zobacz [Dostosowywanie odpowiedzi za pomocą parametrów kwerendy](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="53a29-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="53a29-141">**Wywołanie funkcji API nie działa — gdzie można wykonać więcej testów?**</span><span class="sxs-lookup"><span data-stu-id="53a29-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="53a29-142">**Eksplorator Microsoft Graph** — Przetestuj interfejsy API programu Microsoft Graph w dzierżawie lub w dzierżawie demonstracyjnej, a także zapoznaj się z **przykładowymi kwerendami** w Eksploratorze Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="53a29-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="53a29-143">**Gdy badam dane, tak wygląda na to, że wybiorę niekompletny zestaw danych**</span><span class="sxs-lookup"><span data-stu-id="53a29-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="53a29-144">Jeśli wysyłasz zapytanie do kolekcji (na przykład *Użytkownicy*), program Microsoft Graph używa limitów stron po stronie serwera, więc wyniki są zawsze zwracane z domyślnym rozmiarem strony.</span><span class="sxs-lookup"><span data-stu-id="53a29-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="53a29-145">Aplikacja powinna zawsze oczekiwać na przechodzenie między pozostałymi kolekcjami zwróconymi z usługi.</span><span class="sxs-lookup"><span data-stu-id="53a29-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="53a29-146">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="53a29-146">For more information, see:</span></span>

- [<span data-ttu-id="53a29-147">Najważniejsze wskazówki dotyczące programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="53a29-148">Stronicowanie danych programu Microsoft Graph w aplikacji</span><span class="sxs-lookup"><span data-stu-id="53a29-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="53a29-149">**Moja aplikacja jest zbyt wolna i jest również dowolnie ograniczana. Jakie usprawnienia można wprowadzić?**</span><span class="sxs-lookup"><span data-stu-id="53a29-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="53a29-150">W zależności od tego, co się stanie, w dyspozycji jest wiele różnych opcji, które umożliwiają wydajniejszą realizację aplikacji, a w niektórych przypadkach jest to mniej podatne na ograniczenie działania usługi (gdy zbyt wiele połączeń).</span><span class="sxs-lookup"><span data-stu-id="53a29-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="53a29-151">Aby dowiedzieć się więcej, zobacz:</span><span class="sxs-lookup"><span data-stu-id="53a29-151">To learn more, see:</span></span>

- [<span data-ttu-id="53a29-152">Najważniejsze wskazówki dotyczące programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="53a29-153">Żądania wsadowe</span><span class="sxs-lookup"><span data-stu-id="53a29-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="53a29-154">Śledzenie zmian za pomocą kwerendy Delta</span><span class="sxs-lookup"><span data-stu-id="53a29-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="53a29-155">Otrzymywanie powiadomień o zmianach za pośrednictwem webhook</span><span class="sxs-lookup"><span data-stu-id="53a29-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="53a29-156">Wskazówki dotyczące ograniczania</span><span class="sxs-lookup"><span data-stu-id="53a29-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="53a29-157">**Gdzie można znaleźć więcej informacji o błędach i znanych problemach?**</span><span class="sxs-lookup"><span data-stu-id="53a29-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="53a29-158">Informacje dotyczące odpowiedzi na błędy programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="53a29-159">Znane problemy dotyczące programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="53a29-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="53a29-160">**Gdzie można sprawdzić dostępność statusu usługi i łączności?**</span><span class="sxs-lookup"><span data-stu-id="53a29-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="53a29-161">Dostępność usług i łączność podstawowych usług, do których można uzyskać dostęp za pośrednictwem programu Microsoft Graph, może wpływać na ogólną dostępność i wydajność programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="53a29-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="53a29-162">W przypadku kondycji usługi Azure Active Directory Sprawdź stan **zabezpieczeń + usługi tożsamości** wymienione na [stronie Stan platformy Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="53a29-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="53a29-163">W przypadku usług pakietu Office, które współużytkują się z programem Microsoft Graph, sprawdź stan usług wymienionych na [pulpicie nawigacyjnym kondycja usługi Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="53a29-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
