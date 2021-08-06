---
title: Dostęp do subskrypcji
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999250"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nie można zalogować się na platformie Azure z powodu problemów z przeglądarką (Przeglądarka zawiesza się, obraca się, nie ładuje się itp.).

Może na Ciebie wystąpić błąd. Sprawdź, czy jest bieżąca usługa, w przypadku których nie ma obecnie danych: [Stan usługi Azure Health.](https://status.azure.com/status/history/)

Wyloguj się ze wszystkich aktywnych sesji platformy Azure. Uruchom tryb prywatny lub incognito w przeglądarce sieci Web.

Możesz również spróbować odświeżyć przeglądarkę, użyć innej przeglądarki i usunąć pliki cookie pamięci podręcznej, jeśli powyższe nie działają.

Dowiedz się więcej: [Rozwiązywanie problemów z logowaniem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nie można uzyskać dostępu do subskrypcji**

W portalu [Azure portal](https://portal.azure.com/)upewnij się, że z konta w prawym górnym rogu jest wybrany właściwy katalog Azure.

W Centrum [konta Azure upewnij](https://account.windowsazure.com/Subscriptions)się, czy używane konto jest administratorem konta.

Dowiedz się więcej: [Rozwiązywanie problemów z nie znalezioną subskrypcją](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nie można uzyskać dostępu do historii rozliczeń**

Administrator konta musi upewnić się, że użytkownik, który ma dostęp do informacji rozliczeniowych, został dodany do usługi Azure Active Directory jako użytkownik gość: Dodaj lub [usuń nowego użytkownika.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Następnie użytkownik musi mieć przypisaną rolę administratora globalnego: [Przypisywanie roli użytkownikom.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Opublikuj to, użytkownikowi można przyznać dostęp do rozliczeń przy użyciu zasad RBAC: [Udzielanie dostępu do rozliczeń.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zalecane dokumenty**

-   [Nie mogę się zalogować, aby zarządzać subskrypcją platformy Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)