---
title: Monitorowanie dostępu warunkowego w usłudze Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427925"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="0a907-102">Monitorowanie dostępu warunkowego w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="0a907-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="0a907-103">Użytkownicy z dostępem warunkowym otrzymają powiadomienie e-mail, jeśli nie spełniają wymagań dotyczących dostępu do organizacji.</span><span class="sxs-lookup"><span data-stu-id="0a907-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0a907-104">Aby rozwiązać problem, zalecamy co najmniej jedno z następujących rozwiązań:</span><span class="sxs-lookup"><span data-stu-id="0a907-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="0a907-105">Jeśli urządzenie powinno zostać zarejestrowane, zasuń użytkownika do aplikacji Portal firmy i sprawdź, czy jest ono widoczne w portalu firmy.</span><span class="sxs-lookup"><span data-stu-id="0a907-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0a907-106">Jeśli tak się nie stanie, użytkownik musi zarejestrować urządzenie.</span><span class="sxs-lookup"><span data-stu-id="0a907-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="0a907-107">W portalu Azure przejdź do tematu **zgodność**  >  **urządzenia Intune.**</span><span class="sxs-lookup"><span data-stu-id="0a907-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="0a907-108">Aby wyświetlić raport zgodności urządzenia w celu sprawdzenia, czy urządzenie użytkownika jest zgodne, w obszarze **Monitorowanie** kliknij pozycję **Zgodność urządzenia.**</span><span class="sxs-lookup"><span data-stu-id="0a907-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="0a907-109">W portalu Azure przejdź do tematu **zgodność**  >  **urządzenia Intune.**</span><span class="sxs-lookup"><span data-stu-id="0a907-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="0a907-110">W **obszarze Zarządzanie kliknij** pozycję **Zasady.**</span><span class="sxs-lookup"><span data-stu-id="0a907-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="0a907-111">Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika.</span><span class="sxs-lookup"><span data-stu-id="0a907-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0a907-112">Jeśli nie przypisano żadnego profilu, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.</span><span class="sxs-lookup"><span data-stu-id="0a907-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="0a907-113">Edytuj przypisanie dostępu warunkowego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="0a907-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="0a907-114">W portalu Azure przejdź do zasad dostępu warunkowego usługi **Intune,** wybierz zasady z listy, a następnie kliknij pozycję  >    >  Użytkownicy **i grupy.**</span><span class="sxs-lookup"><span data-stu-id="0a907-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="0a907-115">Aby zasady dotyczące określonej osoby dotyczyły określonej osoby, dodaj ją do **listy Dołącz.**</span><span class="sxs-lookup"><span data-stu-id="0a907-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="0a907-116">Aby mieć pewność, że dana osoba zostanie pominięta w zasadach, dodaj ją do **listy Wyklucz.**</span><span class="sxs-lookup"><span data-stu-id="0a907-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="0a907-117">**Przydatne linki:**</span><span class="sxs-lookup"><span data-stu-id="0a907-117">**Helpful links:**</span></span>

- [<span data-ttu-id="0a907-118">Omówienie zgodności urządzeń</span><span class="sxs-lookup"><span data-stu-id="0a907-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="0a907-119">Rozwiązywanie problemów z urzędu certyfikacji</span><span class="sxs-lookup"><span data-stu-id="0a907-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="0a907-120">Zasady rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="0a907-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="0a907-121">Monitorowanie zgodności urządzenia w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="0a907-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="0a907-122">Te kroki są pomocne tylko podczas rozwiązywania problemów z dostępem warunkowym funkcji usługi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a907-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="0a907-123">Za pomocą zasad programu Exchange można także poddać kwarantannie urządzenie, które blokuje dostęp do poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="0a907-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="0a907-124">Więcej informacji na temat zarządzania urządzeniami z programem Exchange można znaleźć [**tutaj.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="0a907-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
