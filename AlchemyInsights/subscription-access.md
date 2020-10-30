---
title: Dostęp do abonamentu
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807717"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nie można zalogować się na platformie Azure ze względu na problemy z przeglądarką (przeglądarka zawiesza się, nie ładuje, itd.)

Może to mieć wpływ na awarię. Sprawdź, czy są stale dostępne awarie: [stan kondycji Azure](https://status.azure.com/status/history/).

Wyloguj się ze wszystkich aktywnych sesji platformy Azure. Uruchom w przeglądarce sieci Web tryb in-prywatny lub incognito.

Możesz również spróbować odświeżyć przeglądarkę, użyć innej przeglądarki, usunąć pliki cookie z pamięci podręcznej, jeśli nie działają.

Dowiedz się więcej: [Rozwiązywanie problemów z logowaniem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nie można uzyskać dostępu do subskrypcji**

W [portalu Azure](https://portal.azure.com/)upewnij się, że w obszarze konto u ¿prawego prawej strony wybrano właściwy katalog Azure.

Upewnij się, że w [centrum konta platformy Azure](https://account.windowsazure.com/Subscriptions)jest używane konto administratora konta.

Dowiedz się więcej: [Rozwiązywanie problemów z nie odnalezionymi subskrypcjami](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nie można uzyskać dostępu do historii rozliczeń**

Administrator konta musi upewnić się, że użytkownik uzyskujący dostęp do informacji o rozliczeniach jest dodawany w usłudze Azure Active Directory jako użytkownik Gość: [Dodawanie lub usuwanie nowego użytkownika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Użytkownik musi być następnie członkiem roli administratora globalnego: [Przypisywanie roli użytkownikom](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Opublikuj, użytkownik może otrzymać dostęp do rozliczeń za pomocą zasad RBAC: [udzielanie dostępu do rozliczeń](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Polecane dokumenty**

-   [Nie mogę się zalogować, aby zarządzać subskrypcją platformy Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)