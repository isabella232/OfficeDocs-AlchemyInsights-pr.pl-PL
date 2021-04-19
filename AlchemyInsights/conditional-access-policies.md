---
title: Zasady dostępu warunkowego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817290"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="36cba-102">Zasady dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="36cba-102">Conditional Access policies</span></span>

<span data-ttu-id="36cba-103">Dostęp warunkowy to funkcja usługi Azure AD, która umożliwia egzekwowanie kontroli dostępu do aplikacji w danym środowisku na podstawie określonych warunków i z zarządzaniem z lokalizacji centralnej.</span><span class="sxs-lookup"><span data-stu-id="36cba-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="36cba-104">Dowiedz się więcej o [dostępie warunkowym usługi Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="36cba-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="36cba-105">**Uwaga**: jeśli Twoja dzierżawa została utworzona po 21 października 2019 r. i nieoczekiwanie pojawił się monit dotyczący uwierzytelniania wieloskładnikowego, prawdopodobnie masz włączone [domyślne ustawienia zabezpieczeń](https://aka.ms/securitydefaults) w tej dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="36cba-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="36cba-106">**Aby zarządzać domyślnymi ustawieniami zabezpieczeń**</span><span class="sxs-lookup"><span data-stu-id="36cba-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="36cba-107">Zaloguj się do [centrum administracyjnego](https://go.microsoft.com/fwlink/p/?linkid=834822) za pomocą poświadczeń administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="36cba-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="36cba-108">Przejdź do [właściwości usługi Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="36cba-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="36cba-109">Na dole strony kliknij **Zarządzaj ustawieniami domyślnymi zabezpieczeń**.</span><span class="sxs-lookup"><span data-stu-id="36cba-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="36cba-110">Kliknij **Tak**, aby włączyć domyślne ustawienia zabezpieczeń, lub **Nie**, aby je wyłączyć.</span><span class="sxs-lookup"><span data-stu-id="36cba-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
