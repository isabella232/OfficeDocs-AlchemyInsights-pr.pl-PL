---
title: Privileged Identity Management roli
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973239"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Po aktywowaniu roli nie są udzielane uprawnienia**

Po aktywowaniu roli w usłudze Azure AD Privileged Identity Management (PIM) aktywacja może nie zostać natychmiast propagowana do wszystkich portali, które wymagają roli z uprawnieniami. Czasami, nawet jeśli zmiana jest propagowana, buforowanie w sieci Web w portalu może spowodować, że zmiana nie zostanie od razu wzięciem pod uwagę.

Jeśli aktywacja jest opóźniona, wykonaj następujące czynności:

1. Wyloguj się z portalu Azure Portal, a następnie zaloguj się ponownie. Po aktywowaniu roli usługi Azure AD lub roli zasobów platformy Azure zobaczysz etapy aktywacji. Po ukończeniu wszystkich etapów zobaczysz link "Wyloguj się". Możesz użyć tego linku, aby się wylogować. W ten sposób większość przypadków zostanie rozwiązana w przypadku opóźnienia aktywacji.
2. W funkcji PIM sprawdź, czy na liście jest wymieniona rola.
3. Jeśli aktywujesz rolę administratora Exchange, wyloguj się i zaloguj ponownie. Jeśli problem będzie nadal występował, otwórz bilet pomocy technicznej i podnieś go jako problem. Jeśli używasz roli administratora Exchange w celu uzyskiwania dostępu do Centrum zabezpieczeń i zgodności, zobacz następny krok.
4. W przypadku aktywowania roli w celu uzyskania dostępu do Centrum zabezpieczeń i zgodności lub aktywowania roli administratora usługi SharePoint może wystąpić pewne opóźnienie aktywacji od kilku minut do kilku godzin. Jest to znany problem i aktywnie współpracujemy z tymi zespołami, aby jak najszybciej rozwiązać ten problem.

Więcej informacji można znaleźć w następujących artykułach:

- [Aktywowanie ról usługi Azure AD w usłudze PiM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktywowanie ról zasobów platformy Azure w usłudze PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Uprawnienia nie są usuwane po dezaktywowaniu roli lub wygaśnięciu aktywacji roli**

Po dezaktywowaniu roli w usłudze Azure AD Privileged Identity Management lub po wygaśnięciu okresu aktywacji roli może wystąpić opóźnienie w dalszym uzyskiwaniu dostępu.

Jeśli Dezaktywacja jest opóźniona, wykonaj następujące czynności:

1. W przypadku dezaktywowania roli administratora usługi Exchange lub okresu aktywacji roli zauważysz istotne opóźnienie przed usunięciem uprawnień, otwórz bilet pomocy technicznej i powiedz inżynierowi pomocy technicznej, aby pomógł Ci w zgłoszenie do zespołu zarządzania dostępem uprzywilejowanym w organizacji Office o tym problemie.
2. Jeśli okres aktywacji wygasł, ale nadal masz otwartą sesję przeglądarki, zamknij przeglądarkę. Możesz nadal używać tej roli do momentu zamknięcia tej sesji. Jest to znany problem i pracujemy nad poprawą, która może aktywnie odwołać każdą sesję po wygaśnięciu aktywacji.

Jeśli Twoje opóźnienie różni się od tych dwóch scenariuszy, otwórz bilet pomocy technicznej.
