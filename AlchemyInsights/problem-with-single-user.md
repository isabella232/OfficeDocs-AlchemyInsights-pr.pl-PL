---
title: Problem z jednym użytkownikiem
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430202"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="04c91-102">Problem z jednym użytkownikiem</span><span class="sxs-lookup"><span data-stu-id="04c91-102">Problem with single user</span></span>

- <span data-ttu-id="04c91-103">Być może użytkownikowi nie zapewniano obsługi administracyjnej, ponieważ usługa nie miała jeszcze możliwości oceny użytkownika.</span><span class="sxs-lookup"><span data-stu-id="04c91-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="04c91-104">Zapoznaj się ze wskazówkami, jak długo trwa inicjowanie obsługi administracyjnej, a także z paska postępu na stronie konfiguracji inicjowania obsługi.</span><span class="sxs-lookup"><span data-stu-id="04c91-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="04c91-105">Jeśli stan określony w sekcji dodatkowych szczegółów jest stały przed datą utworzenia/aktualizacji/usunięcia użytkownika, oznacza to, że ten użytkownik nie został jeszcze ocenić.</span><span class="sxs-lookup"><span data-stu-id="04c91-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="04c91-106">W tym scenariuszu najlepiej jest zaczekać na ukończenie obsługi administracyjnej.</span><span class="sxs-lookup"><span data-stu-id="04c91-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="04c91-107">Pamiętaj, że usługa ma świadomość zmian wprowadzonych tylko do użytkownika w systemie źródłowym (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="04c91-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="04c91-108">Aby wykryć zmianę i przepływać ją do usługi Active Directory, w systemie źródłowym usługi Azure AD musi być prawidłowa zmiana.</span><span class="sxs-lookup"><span data-stu-id="04c91-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="04c91-109">Usługa inicjowania obsługi administracyjnej oszacowała użytkownika i ustaliła, że nie powinna być zapewniana obsługa aprowizowana:</span><span class="sxs-lookup"><span data-stu-id="04c91-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="04c91-110">Jeśli ustawiono filtr zakresu oparty na atrybutach, upewnij się, że użytkownik spełnia określone kryteria.</span><span class="sxs-lookup"><span data-stu-id="04c91-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="04c91-111">Jeśli użytkownicy już istnieją w systemie docelowym i stanie użytkownika w dopasowaniu źródłowym i docelowym, nie podejmiemy dalszych działań.</span><span class="sxs-lookup"><span data-stu-id="04c91-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="04c91-112">Usługa inicjowania obsługi administracyjnej próbowała aprowizować użytkownika i nie powiodła się.</span><span class="sxs-lookup"><span data-stu-id="04c91-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="04c91-113">Aby zapoznać się z tymi scenariuszami, zapoznaj się z kartą rozwiązywania problemów i zaleceń dzienników inicjowania obsługi:</span><span class="sxs-lookup"><span data-stu-id="04c91-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="04c91-114">W lokalnej usłudze Active Directory lub usłudze Azure AD może brakować wymaganego atrybutu użytkownika.</span><span class="sxs-lookup"><span data-stu-id="04c91-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="04c91-115">Na przykład reguły generowania userPrincipalName lub sAMAccountName nie generują odpowiedniej wartości.</span><span class="sxs-lookup"><span data-stu-id="04c91-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="04c91-116">Zgodny atrybut (zwykle identyfikator pracownika) nie jest rozpoznawny dla unikatowego użytkownika w lokalnej usłudze Active Directory lub usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="04c91-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="04c91-117">Na przykład dwóch użytkowników ma ten sam identyfikator pracownika w usłudze AD, a usługa zwraca kod błędu wskazujący zduplikowane wpisy docelowe dla tego samego wpisu źródłowego.</span><span class="sxs-lookup"><span data-stu-id="04c91-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="04c91-118">Aby przejrzeć dzienniki dla jednego użytkownika i grup, zobacz Przeglądanie dzienników inicjowania obsługi [dla problemu z określonym użytkownikiem.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="04c91-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
