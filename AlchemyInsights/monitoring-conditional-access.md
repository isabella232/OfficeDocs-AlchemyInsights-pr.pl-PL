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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366438"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e69ed-102">Monitorowanie dostępu warunkowego dla programu Exchange</span><span class="sxs-lookup"><span data-stu-id="e69ed-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e69ed-103">Użytkownicy ukierunkowany na dostęp warunkowy otrzymają powiadomienie pocztą e-mail, jeśli nie spełnią wymagań organizacji dotyczących dostępu.</span><span class="sxs-lookup"><span data-stu-id="e69ed-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e69ed-104">W celu rozwiązania problemu zalecamy co najmniej jedno z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="e69ed-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="e69ed-105">Jeśli urządzenie jest uważane za zarejestrowane, zaleca się, aby użytkownik przeszedł do aplikacji Portal firmy i upewnić się, że jest wyświetlany w portalu firmy.</span><span class="sxs-lookup"><span data-stu-id="e69ed-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e69ed-106">Jeśli nie, użytkownik powinien zarejestrować urządzenie.</span><span class="sxs-lookup"><span data-stu-id="e69ed-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="e69ed-107">W portalu Azure przejdź do usługi Intune > Device.</span><span class="sxs-lookup"><span data-stu-id="e69ed-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="e69ed-108">W obszarze Monitor kliknij pozycję Zgodność urządzenia.</span><span class="sxs-lookup"><span data-stu-id="e69ed-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="e69ed-109">Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczone jako zgodne.</span><span class="sxs-lookup"><span data-stu-id="e69ed-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="e69ed-110">W portalu Azure przejdź do usługi Intune > Device.</span><span class="sxs-lookup"><span data-stu-id="e69ed-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="e69ed-111">W obszarze Zarządzanie kliknij pozycję zasady.</span><span class="sxs-lookup"><span data-stu-id="e69ed-111">Under Manage, click Policies.</span></span> <span data-ttu-id="e69ed-112">Na liście zasad zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="e69ed-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e69ed-113">Jeśli żaden profil nie jest przypisany, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="e69ed-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="e69ed-114">Edytowanie przydziału dostępu warunkowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="e69ed-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="e69ed-115">W portalu Azure Portal przejdź do **Intune**  >  **zasad dostępu warunkowego**usługi Intune  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="e69ed-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="e69ed-116">Wybierz zasadę z listy.</span><span class="sxs-lookup"><span data-stu-id="e69ed-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="e69ed-117">Kliknij pozycję Użytkownicy i grupy.</span><span class="sxs-lookup"><span data-stu-id="e69ed-117">Click Users and groups.</span></span>
4. <span data-ttu-id="e69ed-118">Aby określić zasady jako docelowe dla określonej osoby, Dodaj je do listy dołączania.</span><span class="sxs-lookup"><span data-stu-id="e69ed-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="e69ed-119">Aby upewnić się, że dana osoba zostanie pominięta w zasadach, Dodaj je do listy wykluczania.</span><span class="sxs-lookup"><span data-stu-id="e69ed-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="e69ed-120">Pomocne linki:</span><span class="sxs-lookup"><span data-stu-id="e69ed-120">Helpful links:</span></span>

[<span data-ttu-id="e69ed-121">Omówienie zgodności urządzeń</span><span class="sxs-lookup"><span data-stu-id="e69ed-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="e69ed-122">Rozwiązywanie problemów dotyczących urzędu certyfikacji</span><span class="sxs-lookup"><span data-stu-id="e69ed-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e69ed-123">Zasady rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="e69ed-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="e69ed-124">Monitorowanie zgodności urządzenia usługi Intune</span><span class="sxs-lookup"><span data-stu-id="e69ed-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="e69ed-125">Uwaga: te czynności są pomocne tylko w rozwiązywaniu problemów z funkcją dostęp warunkowy usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e69ed-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e69ed-126">Możliwe jest również poddawanie kwarantannie urządzenia blokującego dostęp do poczty e-mail za pomocą zasad programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="e69ed-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e69ed-127">Więcej informacji na temat zarządzania urządzeniami programu Exchange można znaleźć [tutaj](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="e69ed-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
