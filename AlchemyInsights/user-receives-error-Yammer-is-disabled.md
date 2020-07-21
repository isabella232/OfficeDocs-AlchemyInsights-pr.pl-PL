---
title: Użytkownik odbiera błąd AADSTS7000112 Usługa Yammer jest wyłączona
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198376"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="2efc9-102">Użytkownik odbiera błąd AADSTS7000112 Usługa Yammer jest wyłączona</span><span class="sxs-lookup"><span data-stu-id="2efc9-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="2efc9-103">Jeśli zostanie wyświetlony błąd "AADSTS7000112: Application '00000005-0000-0ff1-ce00-00000000000000000" (Yammer) jest wyłączony", występuje problem z jednostką usługi w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2efc9-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="2efc9-104">Administrator mógł wyłączyć jednostkę usługi, aby zablokować dostęp do usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="2efc9-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="2efc9-105">Wyłączenie jednostki usługi nie jest zalecane i może spowodować dodatkowe problemy.</span><span class="sxs-lookup"><span data-stu-id="2efc9-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="2efc9-106">Aby uzyskać więcej informacji na temat obsługiwanego podejścia do blokowania dostępu użytkownika do usługi Yammer, zobacz [Wyłączanie dostępu usługi Yammer dla użytkowników usługi Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="2efc9-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="2efc9-107">Aby rozwiązać ten problem w witrynie Azure Portal i przywrócić dostęp użytkowników do usługi Yammer:</span><span class="sxs-lookup"><span data-stu-id="2efc9-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="2efc9-108">Otwórz stronę Usługi Azure Active Directory i wybierz pozycję **Aplikacje przedsiębiorstwa** w obszarze **Zarządzaj** w lewym okienku nawigacji.</span><span class="sxs-lookup"><span data-stu-id="2efc9-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="2efc9-109">Wpisz **usługę Yammer usługi Office 365** w polu wyszukiwania i wybierz nazwę aplikacji, aby otworzyć ustawienia.</span><span class="sxs-lookup"><span data-stu-id="2efc9-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="2efc9-110">Wybierz **pozycję Właściwości** w obszarze **Zarządzaj** w lewym okienku nawigacji.</span><span class="sxs-lookup"><span data-stu-id="2efc9-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="2efc9-111">Czy ustaw wartość **Włączone dla użytkowników do logowania?** na **Tak**, a następnie wybierz pozycję **Zapisz**.</span><span class="sxs-lookup"><span data-stu-id="2efc9-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="2efc9-112">Zaloguj się ponownie do usługi Yammer.</span><span class="sxs-lookup"><span data-stu-id="2efc9-112">Sign in to Yammer again.</span></span> <span data-ttu-id="2efc9-113">Może być konieczne wyczyszczenie plików cookie.</span><span class="sxs-lookup"><span data-stu-id="2efc9-113">You might need to clear cookies.</span></span>

<span data-ttu-id="2efc9-114">Alternatywnie uruchom polecenia programu PowerShell, aby ustawić wartość.</span><span class="sxs-lookup"><span data-stu-id="2efc9-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="2efc9-115">Aby uzyskać więcej informacji, zobacz [błąd "Przepraszamy, ale problemy z zalogowaniem się" po kliknięciu kafelka Usługi Yammer w usłudze Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="2efc9-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 