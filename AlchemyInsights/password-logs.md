---
title: Dzienniki haseł
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527177"
---
# <a name="password-logs"></a><span data-ttu-id="93c08-102">Dzienniki haseł</span><span class="sxs-lookup"><span data-stu-id="93c08-102">Password logs</span></span>

<span data-ttu-id="93c08-103">**Występują problemy z uzyskiwaniem dostępu do dzienników inspekcji resetowania hasła**</span><span class="sxs-lookup"><span data-stu-id="93c08-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="93c08-104">Aby rozwiązać problemy dotyczące dostępu do dzienników inspekcji resetowania hasła, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="93c08-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="93c08-105">Upewnij się, że masz uprawnienia do wyświetlania dzienników inspekcji.</span><span class="sxs-lookup"><span data-stu-id="93c08-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="93c08-106">Autoryzowane są tylko następujące role:</span><span class="sxs-lookup"><span data-stu-id="93c08-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="93c08-107">Administrator globalny</span><span class="sxs-lookup"><span data-stu-id="93c08-107">Global administrator</span></span>
 - <span data-ttu-id="93c08-108">Administrator zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="93c08-108">Security administrator</span></span>
 - <span data-ttu-id="93c08-109">Czytelnik zabezpieczeń</span><span class="sxs-lookup"><span data-stu-id="93c08-109">Security reader</span></span>

<span data-ttu-id="93c08-110">**Chcę wyświetlić wszystkie zdarzenia inspekcji resetowania hasła od chwili wstępnego wdrożenia**</span><span class="sxs-lookup"><span data-stu-id="93c08-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="93c08-111">W raportach z ostatnich 30 dni jest przechowywanych maksymalnie 120 000 zdarzeń resetowania/rejestracji hasła.</span><span class="sxs-lookup"><span data-stu-id="93c08-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="93c08-112">Ten maksymalny limit dotyczy interfejsu użytkownika podczas pobierania pliku CSV.</span><span class="sxs-lookup"><span data-stu-id="93c08-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="93c08-113">Za pośrednictwem programu PowerShell dostępnych jest 1 milion zdarzeń.</span><span class="sxs-lookup"><span data-stu-id="93c08-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="93c08-114">Aby uzyskać więcej informacji, zobacz poniższe linki:</span><span class="sxs-lookup"><span data-stu-id="93c08-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="93c08-115">Zdarzenia samodzielnego resetowania hasła z interfejsu API raportów i zdarzeń usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="93c08-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="93c08-116">Jak szybko pobrać zdarzenia rejestracji resetowania hasła za pomocą programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="93c08-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="93c08-117">**Chcę dowiedzieć się więcej o możliwościach raportowania resetowania haseł**</span><span class="sxs-lookup"><span data-stu-id="93c08-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="93c08-118">Sprawdź, kto rejestruje lub resetuje hasła w dziennikach inspekcji resetowania haseł usługi Azure AD w portalu Azure w **obszarze Użytkownicy i grupy.**</span><span class="sxs-lookup"><span data-stu-id="93c08-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="93c08-119">Aby uzyskać więcej informacji, zobacz następujące linki:</span><span class="sxs-lookup"><span data-stu-id="93c08-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="93c08-120">Omówienie raportów dotyczących resetowania hasła</span><span class="sxs-lookup"><span data-stu-id="93c08-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="93c08-121">Jak wyświetlić raporty resetowania hasła w portalu Azure Portal</span><span class="sxs-lookup"><span data-stu-id="93c08-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="93c08-122">Zdarzenia samodzielnego resetowania hasła z interfejsu API raportów i zdarzeń usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="93c08-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="93c08-123">Jak szybko pobrać zdarzenia rejestracji resetowania hasła za pomocą programu PowerShell</span><span class="sxs-lookup"><span data-stu-id="93c08-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


