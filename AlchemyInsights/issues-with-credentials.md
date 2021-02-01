---
title: Problemy z poświadczeniami
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063683"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="d6958-102">Problemy z poświadczeniami</span><span class="sxs-lookup"><span data-stu-id="d6958-102">Issues with credentials</span></span>

<span data-ttu-id="d6958-103">Platforma tożsamości firmy Microsoft i przepływ poświadczeń klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisują sposób uwierzytelniania bezpośrednio przy użyciu przepływu przyznawania poświadczeń klienta OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="d6958-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="d6958-104">**Jak zarządzać poświadczeniami hasła lub certyfikatu aplikacji?**</span><span class="sxs-lookup"><span data-stu-id="d6958-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="d6958-105">W interfejsie logowania do usługi Azure możesz użyć poświadczeń [aplikacji az ad,](https://docs.microsoft.com/cli/azure/ad/app/credential) aby usunąć, utworzyć listę lub zresetować poświadczenia certyfikatu lub hasła aplikacji.</span><span class="sxs-lookup"><span data-stu-id="d6958-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="d6958-106">**Jak użytkownicy resetują swoje hasła?**</span><span class="sxs-lookup"><span data-stu-id="d6958-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="d6958-107">Użytkownicy muszą zarejestrować [się w celu samodzielnego](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) resetowania hasła, zanim będą oni mieli możliwość resetowania swoich haseł.</span><span class="sxs-lookup"><span data-stu-id="d6958-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="d6958-108">Po zarejestrowaniu użytkownik może wykonać instrukcje z tego artykułu, aby zresetować swoje hasło: [zresetuj](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)swoje hasło służbowe.</span><span class="sxs-lookup"><span data-stu-id="d6958-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="d6958-109">**Jak moi użytkownicy zmieniają swoje hasła?**</span><span class="sxs-lookup"><span data-stu-id="d6958-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="d6958-110">Użytkownicy mogą wykonać czynności opisane w tym artykule, aby zmienić swoje hasła: [jak zmienić hasło.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="d6958-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="d6958-111">Mogą oni również [zarządzać hasłami aplikacji w celu weryfikacji dwuetapowej.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="d6958-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="d6958-112">**Mój użytkownik jest wyświetlany komunikat o błędzie podczas zmieniania lub resetowania hasła**</span><span class="sxs-lookup"><span data-stu-id="d6958-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="d6958-113">Ten link zawiera informacje o typowych problemach, które mogą wystąpić podczas próby zresetowania hasła przez [użytkownika: typowe problemy i ich rozwiązania](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="d6958-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="d6958-114">**Mam problem z resetowaniem hasła użytkownika**</span><span class="sxs-lookup"><span data-stu-id="d6958-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="d6958-115">Upewnij się, że masz upoważnienie do resetowania haseł.</span><span class="sxs-lookup"><span data-stu-id="d6958-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="d6958-116">*Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.*</span><span class="sxs-lookup"><span data-stu-id="d6958-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="d6958-117">Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.</span><span class="sxs-lookup"><span data-stu-id="d6958-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="d6958-118">Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:</span><span class="sxs-lookup"><span data-stu-id="d6958-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="d6958-119">W organizacji musi być przypisana co najmniej jedna licencja:</span><span class="sxs-lookup"><span data-stu-id="d6958-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="d6958-120">**Tylko użytkownicy w chmurze** — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="d6958-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="d6958-121">**Użytkownicy chmury i/lub** lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="d6958-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="d6958-122">Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w [usłudze Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="d6958-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="d6958-123">Aby zresetować hasło użytkownika, znajdź użytkownika w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d6958-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="d6958-124">Następnie na ekranie podglądu tego użytkownika kliknij przycisk "resetuj hasło".</span><span class="sxs-lookup"><span data-stu-id="d6958-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="d6958-125">**Przycisk resetowania hasła jest wyszzarowany**</span><span class="sxs-lookup"><span data-stu-id="d6958-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="d6958-126">Nie masz uprawnień do **resetowania** haseł tego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="d6958-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="d6958-127">*Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.*</span><span class="sxs-lookup"><span data-stu-id="d6958-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="d6958-128">Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.</span><span class="sxs-lookup"><span data-stu-id="d6958-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="d6958-129">**Nie widzę bladego resetowania hasła**</span><span class="sxs-lookup"><span data-stu-id="d6958-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="d6958-130">Nie masz uprawnień do resetowania haseł.</span><span class="sxs-lookup"><span data-stu-id="d6958-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="d6958-131">*Tylko administratorzy globalni, administratorzy haseł i użytkowników mogą resetować hasła użytkowników.*</span><span class="sxs-lookup"><span data-stu-id="d6958-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="d6958-132">Administratorzy globalni mogą także resetować hasła innych administratorów z uprawnieniami.</span><span class="sxs-lookup"><span data-stu-id="d6958-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="d6958-133">**W resetowaniu hasła nie widzę lokalnego bloku integracji**</span><span class="sxs-lookup"><span data-stu-id="d6958-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="d6958-134">Lokalna tarcza integracji pojawia się tylko w środowiskach hybrydowych — co oznacza, że do manipulowania hasłami użytkowników lokalnych używasz funkcji zapisu hasła.</span><span class="sxs-lookup"><span data-stu-id="d6958-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="d6958-135">Ten blok blokowy nie jest wyświetlony, jeśli:</span><span class="sxs-lookup"><span data-stu-id="d6958-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="d6958-136">Nie korzystasz z funkcji zapisu hasła</span><span class="sxs-lookup"><span data-stu-id="d6958-136">You are not using password writeback</span></span>
  - <span data-ttu-id="d6958-137">Występuje problem z instalacją/łącznością zapisu hasła</span><span class="sxs-lookup"><span data-stu-id="d6958-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="d6958-138">Występuje problem z instalacją/łącznością programu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d6958-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="d6958-139">Aby uzyskać więcej kroków rozwiązywania problemów z zapisem hasła, zobacz [Rozwiązywanie problemów z pisaniem hasła](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="d6958-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="d6958-140">**Nie wiem, jak zresetować hasło użytkownika**</span><span class="sxs-lookup"><span data-stu-id="d6958-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="d6958-141">Zaloguj się do portalu Azure Portal jako odpowiedni administrator.</span><span class="sxs-lookup"><span data-stu-id="d6958-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="d6958-142">Przejdź do bloku **Użytkownicy i grupy,** wybierz **pozycję Wszyscy użytkownicy.**</span><span class="sxs-lookup"><span data-stu-id="d6958-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="d6958-143">Wybierz użytkownika z listy.</span><span class="sxs-lookup"><span data-stu-id="d6958-143">Select a user from the list.</span></span>
4. <span data-ttu-id="d6958-144">Dla wybranego użytkownika wybierz pozycję **Przegląd,** a następnie na pasku poleceń wybierz pozycję **Resetuj hasło.**</span><span class="sxs-lookup"><span data-stu-id="d6958-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="d6958-145">Wybierz przycisk **Resetuj** hasło i postępuj zgodnie z instrukcjami wyświetlanymi na ekranie.</span><span class="sxs-lookup"><span data-stu-id="d6958-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="d6958-146">Resetowanie odbywa się tylko za pośrednictwem **portalu Azure Portal** i obsługuje pisanie hasła.</span><span class="sxs-lookup"><span data-stu-id="d6958-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="d6958-147">**Resetowanie hasła użytkownika lokalnego z portalu administracyjnego usługi Office 365 lub aplikacji mobilnej usługi Office 365, ale użytkownik nadal nie może się zalogować**</span><span class="sxs-lookup"><span data-stu-id="d6958-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="d6958-148">W tym portalu nie jest obsługiwane pisanie zwrotne hasła.</span><span class="sxs-lookup"><span data-stu-id="d6958-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="d6958-149">Zresetuj ponownie hasło użytkownika w portalu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d6958-149">Reset the user's password again in the Azure portal.</span></span>
