---
title: Problemy z dostępem warunkowym
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014888"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="3a0a0-102">Problemy z dostępem warunkowym</span><span class="sxs-lookup"><span data-stu-id="3a0a0-102">Conditional access issues</span></span>

<span data-ttu-id="3a0a0-103">**Rozwiązywanie problemów z diagnostyką logowania**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="3a0a0-104">Możesz szybko dowiedzieć się, co się stało lub zdiagnozować o problemach związanych z logowaniem się użytkowników przy użyciu [diagnostyki logowania](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="3a0a0-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="3a0a0-105">Uruchom diagnostykę logowania.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="3a0a0-106">Znajdź zdarzenie, które ma zostać zanalizowane, wprowadzając szczegółowe informacje o użytkowniku, aplikacji, czasie logowania, identyfikatorze żądania lub identyfikatorze korelacji.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="3a0a0-107">Przejrzyj wyniki diagnostyczne przedstawiające szczegóły dotyczące tego, co się stało, oraz jakie działania możesz podjąć, aby wprowadzić zmiany (jeśli są potrzebne zmiany).</span><span class="sxs-lookup"><span data-stu-id="3a0a0-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="3a0a0-108">**Procedura rozwiązywania problemów z logowaniem**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="3a0a0-109">Przejdź do strony logowania usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="3a0a0-110">Filtruj logowanie według użytkownika, zakresu czasu, aplikacji, statusu, aplikacji klienckiej itd.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="3a0a0-111">Wybierz zdarzenie logowania i Wyświetl kartę dostęp warunkowy, aby sprawdzić, które zasady zostały oszacowane.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="3a0a0-112">Kliknij wiersz zasady, aby wyświetlić szczegółowe informacje o zasadach i zrozumieć, dlaczego jest ona stosowana.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="3a0a0-113">**Narzędzia do rozwiązywania problemów z zasadami dostępu warunkowego**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="3a0a0-114">Tryb tylko w raporcie umożliwia ocenę zasad bez wpływu na użytkowników.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="3a0a0-115">Narzędzie warunkowe umożliwia symulowanie zdarzeń logowania i sprawdzanie, jakie zasady obowiązują.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="3a0a0-116">W skoroszycie informacji szczegółowych i raportowania jest wyświetlany wpływ poszczególnych zasad na czas w czasie rzeczywistym.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="3a0a0-117">**Zasady ochrony planu bazowego**</span><span class="sxs-lookup"><span data-stu-id="3a0a0-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="3a0a0-118">Zasady ochrony planu bazowego są przestarzałe.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="3a0a0-119">Nie są już wymuszane i wkrótce zostaną usunięte z portalu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="3a0a0-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="3a0a0-120">Zalecamy włączenie [ustawień domyślnych zabezpieczeń](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="3a0a0-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="3a0a0-121">Aby uzyskać więcej informacji o dostępie warunkowym, zobacz:</span><span class="sxs-lookup"><span data-stu-id="3a0a0-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="3a0a0-122">[Najważniejsze wskazówki dotyczące dostępu warunkowego w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Warunki w dostępie](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 warunkowym [Formanty w dostępie](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 warunkowym [Lokalizacje w dostępie warunkowym](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="3a0a0-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
