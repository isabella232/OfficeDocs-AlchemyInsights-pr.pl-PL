---
title: Uprzywilejowana rola zarządzania tożsamością
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088877"
---
# <a name="privileged-identity-managementpim-role"></a>Rola uprzywilejowanego zarządzania tożsamościami (PIM)

**Uprawnienia nie są udzielane po aktywowaniu roli**

Po aktywowaniu roli w usłudze Azure AD o uprzywilejowanym zarządzaniu tożsamości (PIM) Aktywacja może nie zostać natychmiast rozpropagowana do wszystkich portali wymagających roli uprzywilejowanej. Czasami nawet w przypadku propagacji zmiany buforowanie w sieci Web w portalu może spowodować, że zmiana nie zostanie wprowadzona od razu.

Jeśli aktywacja jest opóźniona, wykonaj następujące czynności:

1. Wyloguj się z portalu Azure, a następnie zaloguj się ponownie. Po aktywowaniu roli usługi Azure AD lub roli zasobów platformy Azure zostaną wyświetlone etapy aktywacji. Po zakończeniu wszystkich etapów zostanie wyświetlone łącze Wyloguj. Możesz użyć tego linku, aby się wylogować. Spowoduje to rozwiązanie większości przypadków opóźnienia aktywacji.
2. W programie PIM Sprawdź, czy jesteś członkiem roli.
3. Jeśli uaktywniasz rolę administratora programu Exchange, upewnij się, że wylogowano się i zaloguj się ponownie. Jeśli problem będzie nadal występował, Otwórz bilet pomocy technicznej i zwiększ go jako problem. Jeśli korzystasz z roli administratora programu Exchange, aby uzyskać dostęp do centrum zabezpieczeń i zgodności, zobacz następny krok.
4. Jeśli uaktywniasz rolę w celu uzyskania dostępu do centrum zabezpieczeń i zgodności albo jeśli uaktywniasz rolę administratora programu SharePoint, będziesz mieć pewne opóźnienie aktywacji od kilku minut do kilku godzin. Jest to znany problem i aktywnie pracujemy nad tym zespołem w celu możliwie jak najszybszego rozwiązania problemu.

Aby uzyskać więcej informacji, zobacz:

- [Aktywowanie ról usługi Azure AD w programie PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktywowanie ról zasobów platformy Azure w programie PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Uprawnienia nie są usuwane po zdezaktywowaniu roli lub wygaśnięciu aktywacji roli**

Po zdezaktywowaniu roli w ramach uprzywilejowanego zarządzania tożsamościami usługi Azure AD lub po wygaśnięciu okresu aktywacji roli może istnieć opóźnienie, w którym nadal masz dostęp.

Jeśli dezaktywacja jest opóźniona, wykonaj następujące czynności:

1. Jeśli użytkownik dezaktywuje rolę administratora programu Exchange lub upłynie okres aktywacji roli, a Użytkownik zauważy znaczne opóźnienie przed usunięciem uprawnień, należy otworzyć bilet pomocy technicznej i poinstruować inżyniera pomocy technicznej, aby pomóc Ci w zalogowaniu się do biletu za pomocą zespołu PAM (uprzywilejowanego zarządzania dostępem) w pakiecie Office o tym problemie.
2. Jeśli okres aktywacji upłynął, ale nadal masz otwartą sesję przeglądarki, zamknij przeglądarkę. Możesz nadal korzystać z tej roli, dopóki nie zamkniesz tej sesji. Jest to znany problem, który umożliwia jednoczesne cofnięcie każdej sesji po wygaśnięciu aktywacji.

Jeśli opóźnienie różni się od tych dwóch scenariuszy, należy otworzyć bilet pomocy technicznej.
