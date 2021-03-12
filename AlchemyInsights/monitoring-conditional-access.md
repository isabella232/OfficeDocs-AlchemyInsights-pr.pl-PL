---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708684"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="f25db-102">Monitorowanie dostępu warunkowego dla programu Exchange</span><span class="sxs-lookup"><span data-stu-id="f25db-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="f25db-103">Użytkownicy z dostępem warunkowym otrzymają powiadomienie e-mail, jeśli nie spełniają wymagań dotyczących dostępu do organizacji.</span><span class="sxs-lookup"><span data-stu-id="f25db-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f25db-104">Aby rozwiązać problem, zalecamy co najmniej jedno z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="f25db-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="f25db-105">Jeśli urządzenie powinno zostać zarejestrowane, zasuń użytkownika do aplikacji Portal firmy i sprawdź, czy jest ono widoczne w portalu firmy.</span><span class="sxs-lookup"><span data-stu-id="f25db-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f25db-106">Jeśli tak się nie stanie, użytkownik powinien zarejestrować urządzenie.</span><span class="sxs-lookup"><span data-stu-id="f25db-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="f25db-107">W portalu Azure przejdź do usługi Intune > zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f25db-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="f25db-108">W obszarze Monitorowanie kliknij pozycję Zgodność urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f25db-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="f25db-109">Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest zgodne.</span><span class="sxs-lookup"><span data-stu-id="f25db-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="f25db-110">W portalu Azure przejdź do usługi Intune > zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f25db-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="f25db-111">W obszarze Zarządzanie kliknij pozycję Zasady.</span><span class="sxs-lookup"><span data-stu-id="f25db-111">Under Manage, click Policies.</span></span> <span data-ttu-id="f25db-112">Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f25db-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f25db-113">Jeśli nie przypisano żadnego profilu, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f25db-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="f25db-114">Edytuj przypisanie dostępu warunkowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="f25db-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="f25db-115">W portalu Azure przejdź do zasad **dostępu**  >    >  **warunkowego usługi Intune.**</span><span class="sxs-lookup"><span data-stu-id="f25db-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="f25db-116">Wybierz zasady z listy.</span><span class="sxs-lookup"><span data-stu-id="f25db-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="f25db-117">Kliknij pozycję Użytkownicy i grupy.</span><span class="sxs-lookup"><span data-stu-id="f25db-117">Click Users and groups.</span></span>
4. <span data-ttu-id="f25db-118">Aby zasady dotyczące określonej osoby dotyczyły określonej osoby, dodaj ją do listy Uwzględnij.</span><span class="sxs-lookup"><span data-stu-id="f25db-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="f25db-119">Aby mieć pewność, że dana osoba zostanie pominięta w zasadach, dodaj ją do listy Wyklucz.</span><span class="sxs-lookup"><span data-stu-id="f25db-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="f25db-120">Przydatne linki:</span><span class="sxs-lookup"><span data-stu-id="f25db-120">Helpful links:</span></span>

[<span data-ttu-id="f25db-121">Omówienie zgodności urządzeń</span><span class="sxs-lookup"><span data-stu-id="f25db-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f25db-122">Rozwiązywanie problemów z urzędu certyfikacji</span><span class="sxs-lookup"><span data-stu-id="f25db-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f25db-123">Zasady rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="f25db-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="f25db-124">Monitorowanie zgodności urządzenia w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="f25db-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="f25db-125">Uwaga: te kroki są pomocne tylko podczas rozwiązywania problemów z dostępem warunkowym funkcji usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f25db-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="f25db-126">Za pomocą zasad programu Exchange można także poddać kwarantannie urządzenie, które blokuje dostęp do poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="f25db-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="f25db-127">Więcej informacji na temat zarządzania urządzeniami z programem Exchange można znaleźć [tutaj]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="f25db-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
