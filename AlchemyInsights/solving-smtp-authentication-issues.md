---
title: Włączanie uwierzytelniania SMTP i rozwiązywania problemów
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077661"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="058bc-102">Włączanie uwierzytelniania SMTP i rozwiązywania problemów</span><span class="sxs-lookup"><span data-stu-id="058bc-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="058bc-103">Jeśli chcesz włączyć uwierzytelnianie SMTP dla skrzynki pocztowej lub jest wyświetlany komunikat o błędzie "Klient nie uwierzytelniony", "Uwierzytelnienie nie powiodło się" lub "SmtpClientAuthentication" z kodem 5.7.57 albo 5.7.3 lub 5.7.139 podczas próby przekazywania wiadomości e-mail przez uwierzytelnienie urządzenia lub aplikacji przy użyciu programu Microsoft 365, wykonaj następujące trzy czynności, aby rozwiązać ten problem:</span><span class="sxs-lookup"><span data-stu-id="058bc-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="058bc-104">Wyłącz domyślne [ustawienia zabezpieczeń platformy Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) przełączanie opcji Włącz **domyślne ustawienia zabezpieczeń** na **Wartość Nie.**</span><span class="sxs-lookup"><span data-stu-id="058bc-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="058bc-105">a.</span><span class="sxs-lookup"><span data-stu-id="058bc-105">a.</span></span> <span data-ttu-id="058bc-106">Zaloguj się do portalu Azure jako administrator zabezpieczeń, administrator dostępu warunkowego lub administrator globalny.</span><span class="sxs-lookup"><span data-stu-id="058bc-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="058bc-107">b.</span><span class="sxs-lookup"><span data-stu-id="058bc-107">b.</span></span> <span data-ttu-id="058bc-108">Przejdź do Azure Active Directory > **właściwości.**</span><span class="sxs-lookup"><span data-stu-id="058bc-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="058bc-109">c.</span><span class="sxs-lookup"><span data-stu-id="058bc-109">c.</span></span> <span data-ttu-id="058bc-110">Wybierz **pozycję Zarządzaj ustawieniami domyślnymi zabezpieczeń.**</span><span class="sxs-lookup"><span data-stu-id="058bc-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="058bc-111">d.</span><span class="sxs-lookup"><span data-stu-id="058bc-111">d.</span></span> <span data-ttu-id="058bc-112">Ustaw **wartość Włącz domyślne ustawienia zabezpieczeń** na **Nie**.</span><span class="sxs-lookup"><span data-stu-id="058bc-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="058bc-113">e.</span><span class="sxs-lookup"><span data-stu-id="058bc-113">e.</span></span> <span data-ttu-id="058bc-114">Wybierz **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="058bc-114">Select **Save**.</span></span>

2. <span data-ttu-id="058bc-115">[Włącz przesyłanie smtp klienta](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) dla licencjonowanej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="058bc-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="058bc-116">a.</span><span class="sxs-lookup"><span data-stu-id="058bc-116">a.</span></span> <span data-ttu-id="058bc-117">Z centrum administracyjne platformy Microsoft 365 przejdź do **strony Aktywni użytkownicy** i wybierz użytkownika.</span><span class="sxs-lookup"><span data-stu-id="058bc-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="058bc-118">b.</span><span class="sxs-lookup"><span data-stu-id="058bc-118">b.</span></span> <span data-ttu-id="058bc-119">Przejdź do karty Poczta, a następnie w obszarze **Aplikacje poczty e-mail** wybierz **pozycję Zarządzaj aplikacjami poczty e-mail**.</span><span class="sxs-lookup"><span data-stu-id="058bc-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="058bc-120">d.</span><span class="sxs-lookup"><span data-stu-id="058bc-120">d.</span></span> <span data-ttu-id="058bc-121">Upewnij **się, że jest zaznaczona** opcja Uwierzytelniony SMTP (włączona).</span><span class="sxs-lookup"><span data-stu-id="058bc-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="058bc-122">e.</span><span class="sxs-lookup"><span data-stu-id="058bc-122">e.</span></span> <span data-ttu-id="058bc-123">Wybierz **pozycję Zapisz zmiany.**</span><span class="sxs-lookup"><span data-stu-id="058bc-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="058bc-124">[Wyłącz uwierzytelnianie wieloskładnikowe (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) dla licencjonowanej skrzynki pocztowej.</span><span class="sxs-lookup"><span data-stu-id="058bc-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="058bc-125">a.</span><span class="sxs-lookup"><span data-stu-id="058bc-125">a.</span></span> <span data-ttu-id="058bc-126">Przejdź do centrum administracyjne platformy Microsoft 365, a następnie w lewym menu nawigacji wybierz **pozycję**  >  **Aktywni użytkownicy** Użytkownicy.</span><span class="sxs-lookup"><span data-stu-id="058bc-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="058bc-127">b.</span><span class="sxs-lookup"><span data-stu-id="058bc-127">b.</span></span> <span data-ttu-id="058bc-128">Wybierz **pozycję Uwierzytelnianie wieloskładnikowe**.</span><span class="sxs-lookup"><span data-stu-id="058bc-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="058bc-129">c.</span><span class="sxs-lookup"><span data-stu-id="058bc-129">c.</span></span> <span data-ttu-id="058bc-130">Wybierz użytkownika i wyłącz **funkcję Multi-Factor Auth.**</span><span class="sxs-lookup"><span data-stu-id="058bc-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
