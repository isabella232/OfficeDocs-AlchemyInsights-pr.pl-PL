---
title: Włączanie zapisywania zwrotnego haseł w programie Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814022"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="fe04f-102">Włączanie zapisywania zwrotnego haseł w programie Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="fe04f-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="fe04f-103">Aby włączyć zapisywanie zwrotne dla samoobsługowego resetowania hasła, najpierw włącz opcję zapisywania zwrotnego haseł w programie Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fe04f-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="fe04f-104">Wykonaj następujące kroki na serwerze Azure AD Connect:</span><span class="sxs-lookup"><span data-stu-id="fe04f-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="fe04f-105">Zaloguj się na serwerze Azure AD Connect i uruchom kreatora konfiguracji **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="fe04f-106">Na **Stronie głównej** kliknij przycisk **Konfiguruj**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="fe04f-107">Na stronie **Zadania dodatkowe** wybierz pozycję **Dostosuj opcje synchronizacji**, a następnie kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="fe04f-108">Na stronie **Połącz z usługą Azure AD**, wprowadź poświadczenie administratora globalnego dla Twojej dzierżawy platformy Azure, a następnie kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="fe04f-109">Na stronach **Połącz katalogi** oraz **Domena/jednostka organizacyjna** kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="fe04f-110">Na stronie **Funkcje opcjonalne** zaznacz pole wyboru obok opcji **Zapisywanie zwrotne haseł** i kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="fe04f-111">Na stronie **Gotowy do konfiguracji** kliknij przycisk **Konfiguruj** i poczekaj aż proces się skończy.</span><span class="sxs-lookup"><span data-stu-id="fe04f-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="fe04f-112">Kiedy konfiguracja dobiegnie końca, naciśnij przycisk **Wyjdź**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="fe04f-113">Gdy zapisywanie zwrotne zostało już włączone w programie Azure AD Connect, skonfiguruj funkcję samoobsługowego resetowania hasła (SSPR) w usłudze Azure AD do zapisywania zwrotnego.</span><span class="sxs-lookup"><span data-stu-id="fe04f-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="fe04f-114">Aby włączyć zapisywanie zwrotne haseł dla funkcji SSPR, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="fe04f-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="fe04f-115">Zaloguj się w portalu Azure używając konta administratora globalnego.</span><span class="sxs-lookup"><span data-stu-id="fe04f-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="fe04f-116">Wyszukaj i wybierz usługę **Azure Active Directory**, kliknij przycisk **Resetowanie hasła**, a następnie kliknij przycisk **Integracja lokalna**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="fe04f-117">Ustaw dla opcji **Zapisywać zwrotnie hasła w katalogu lokalnym?** wartość **Tak**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="fe04f-118">Ustaw dla opcji **Zezwalać użytkownikom na odblokowanie konta bez resetowania hasła?** wartość **Tak**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="fe04f-119">Po zakończeniu kliknij przycisk **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="fe04f-119">When ready, click **Save**.</span></span>

<span data-ttu-id="fe04f-120">Aby uzyskać więcej informacji, zobacz: [Włączanie zapisywania zwrotnego dla samoobsługowego resetowania hasła w usłudze Azure Active Directory w środowisku lokalnym](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="fe04f-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="fe04f-121">Gdy administrator resetuje hasło użytkownika w portalu Azure, jeśli jest to użytkownik federacyjny lub skrót hasła został zsynchronizowany, hasło zostanie zapisane zwrotnie lokalnie.</span><span class="sxs-lookup"><span data-stu-id="fe04f-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="fe04f-122">Ta funkcja wymaga licencji Azure Premium (P1 lub P2) i obecnie nie jest obsługiwana w portalu Office Admin.</span><span class="sxs-lookup"><span data-stu-id="fe04f-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
