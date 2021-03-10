---
title: Problem z resetowaniem hasła
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696273"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="911f9-102">Problemy z resetowaniem hasła</span><span class="sxs-lookup"><span data-stu-id="911f9-102">Problems resetting password</span></span>

<span data-ttu-id="911f9-103">Poniżej przedstawiono niektóre problemy, które mogą wystąpić podczas resetowania hasła i możliwe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="911f9-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="911f9-104">**Mam problem z resetowaniem hasła, które nie jest uwzględnione w innych kategoriach**</span><span class="sxs-lookup"><span data-stu-id="911f9-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="911f9-105">Upewnij się, że masz upoważnienie do resetowania haseł.</span><span class="sxs-lookup"><span data-stu-id="911f9-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="911f9-106">Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.</span><span class="sxs-lookup"><span data-stu-id="911f9-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="911f9-107">Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.</span><span class="sxs-lookup"><span data-stu-id="911f9-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="911f9-108">Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:</span><span class="sxs-lookup"><span data-stu-id="911f9-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="911f9-109">W organizacji musi być przypisana co najmniej jedna licencja</span><span class="sxs-lookup"><span data-stu-id="911f9-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="911f9-110">Tylko użytkownicy w chmurze — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="911f9-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="911f9-111">Użytkownicy chmury i/lub lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="911f9-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="911f9-112">Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz artykuł Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w [usłudze Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="911f9-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="911f9-113">**Mam problemy z testowaniem ustawionych przeze mnie zasad resetowania hasła**</span><span class="sxs-lookup"><span data-stu-id="911f9-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="911f9-114">Replikowanie ostatnio zastosowanych zasad we wszystkich centrach danych i punktach końcowych może potrwać kilka minut.</span><span class="sxs-lookup"><span data-stu-id="911f9-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="911f9-115">Odległość fizyczna od centrum danych ma również wpływ na sposób szybkiego stosowania zmian.</span><span class="sxs-lookup"><span data-stu-id="911f9-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="911f9-116">Przetestuj z użytkownikiem końcowego, a nie z administratorem, i przetestuj z niewielkim zestawem użytkowników.</span><span class="sxs-lookup"><span data-stu-id="911f9-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="911f9-117">Zasady skonfigurowane w portalu Azure Portal mają zastosowanie TYLKO do użytkowników końcowych, a nie administratorów.</span><span class="sxs-lookup"><span data-stu-id="911f9-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="911f9-118">Firma Microsoft wymusza silne, domyślne zasady resetowania hasła w dwóch bramach dla dowolnej roli administratora platformy Azure (przykład: Administrator globalny, Administrator pomocy technicznej, Administrator haseł itp.).</span><span class="sxs-lookup"><span data-stu-id="911f9-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="911f9-119">Dowiedz się więcej o [zasadach dla administratorów.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="911f9-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="911f9-120">**Chcę wdrożyć resetowanie hasła, ale nie chcę, aby moi użytkownicy rejestrować dodatkowe informacje zabezpieczające**</span><span class="sxs-lookup"><span data-stu-id="911f9-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="911f9-121">Wstępnie wypełnij dane użytkowników, aby nie muszą tego zrobić!</span><span class="sxs-lookup"><span data-stu-id="911f9-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="911f9-122">— Jako administrator możesz ustawić właściwości telefonu i poczty e-mail dla użytkowników przed rozpoczęciem resetowania hasła w organizacji.</span><span class="sxs-lookup"><span data-stu-id="911f9-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="911f9-123">Możesz to zrobić przy użyciu interfejsu API, programu PowerShell lub programu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="911f9-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="911f9-124">Więcej informacji tutaj:</span><span class="sxs-lookup"><span data-stu-id="911f9-124">More information here:</span></span>
- [<span data-ttu-id="911f9-125">Wdrażanie resetowania hasła bez konieczności rejestrowania użytkowników</span><span class="sxs-lookup"><span data-stu-id="911f9-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="911f9-126">Jakie dane są używane przez resetowanie hasła</span><span class="sxs-lookup"><span data-stu-id="911f9-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="911f9-127">**Przycisk resetowania hasła jest wyszzarowany**</span><span class="sxs-lookup"><span data-stu-id="911f9-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="911f9-128">Nie masz uprawnień do resetowania haseł tego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="911f9-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="911f9-129">Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.</span><span class="sxs-lookup"><span data-stu-id="911f9-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="911f9-130">Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.</span><span class="sxs-lookup"><span data-stu-id="911f9-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="911f9-131">**Nie widzę bladego resetowania hasła**</span><span class="sxs-lookup"><span data-stu-id="911f9-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="911f9-132">Nie masz uprawnień do resetowania haseł.</span><span class="sxs-lookup"><span data-stu-id="911f9-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="911f9-133">Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.</span><span class="sxs-lookup"><span data-stu-id="911f9-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="911f9-134">Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.</span><span class="sxs-lookup"><span data-stu-id="911f9-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="911f9-135">**W resetowaniu hasła nie widzę lokalnego bloku integracji**</span><span class="sxs-lookup"><span data-stu-id="911f9-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="911f9-136">Lokalna tarcza integracji pojawia się tylko w środowiskach hybrydowych — co oznacza, że do manipulowania hasłami użytkowników lokalnych używasz funkcji zapisu hasła.</span><span class="sxs-lookup"><span data-stu-id="911f9-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="911f9-137">Ten blok blokowy nie jest wyświetlony, jeśli:</span><span class="sxs-lookup"><span data-stu-id="911f9-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="911f9-138">Nie korzystasz z funkcji zapisu hasła</span><span class="sxs-lookup"><span data-stu-id="911f9-138">You are not using password writeback</span></span>
    - <span data-ttu-id="911f9-139">Występuje problem z instalacją/łącznością zapisu hasła</span><span class="sxs-lookup"><span data-stu-id="911f9-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="911f9-140">Występuje problem z instalacją/łącznością programu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="911f9-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="911f9-141">Aby uzyskać więcej kroków rozwiązywania problemów z zapisem hasła, zobacz sekcję Rozwiązywanie problemów z [pisaniem hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="911f9-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="911f9-142">**Nie wiem, jak zresetować hasło użytkownika**</span><span class="sxs-lookup"><span data-stu-id="911f9-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="911f9-143">Zaloguj się do portalu Azure Portal jako odpowiedni administrator.</span><span class="sxs-lookup"><span data-stu-id="911f9-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="911f9-144">Przejdź do bloku Użytkownicy i grupy, wybierz **pozycję Wszyscy użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="911f9-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="911f9-145">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="911f9-145">Select a user from the list.</span></span>
1. <span data-ttu-id="911f9-146">Dla wybranego użytkownika wybierz **pozycję Przegląd,** a następnie na pasku poleceń kliknij pozycję **Resetuj hasło.**</span><span class="sxs-lookup"><span data-stu-id="911f9-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="911f9-147">Postępuj zgodnie z instrukcjami wyświetlanymi na ekranie.</span><span class="sxs-lookup"><span data-stu-id="911f9-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="911f9-148">Resetowanie odbywa się tylko za pośrednictwem portalu Azure Portal i obsługuje pisanie hasła.</span><span class="sxs-lookup"><span data-stu-id="911f9-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="911f9-149">**Resetowanie hasła użytkownika lokalnego z portalu administracyjnego usługi Office 365 lub aplikacji mobilnej usługi Office 365, ale użytkownik nadal nie może się zalogować**</span><span class="sxs-lookup"><span data-stu-id="911f9-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="911f9-150">W tym portalu nie jest obsługiwane pisanie zwrotne hasła.</span><span class="sxs-lookup"><span data-stu-id="911f9-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="911f9-151">Zresetuj ponownie hasło użytkownika w portalu Azure Portal — portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="911f9-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

