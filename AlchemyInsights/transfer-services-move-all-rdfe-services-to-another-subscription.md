---
title: Usługi przesyłania — przenoszenie wszystkich usług RDFE do innej subskrypcji
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
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940076"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Usługi przesyłania — przenoszenie wszystkich usług RDFE do innej subskrypcji

**Przenoszenie zasobów**

Zasoby platformy Azure można przenosić do innej subskrypcji platformy Azure lub grupy zasobów w ramach tej samej subskrypcji za pomocą portalu Azure Portal, Azure PowerShell, interfejsu azure cli lub interfejsu API rest w celu przenoszenia zasobów.

Przed przeniesieniem zasobów zobacz:

- [Lista kontrolna przed przeniesieniem zasobów](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Usługi, które można przenosić](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Jak sprawdzić poprawność przenoszenia](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Wskazówki dotyczące przenoszenia usług](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Aby przenieść istniejące zasoby do innej grupy zasobów lub innej subskrypcji, możesz użyć:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Samouczek: [przenoszenie zasobów platformy Azure do innej grupy zasobów lub innej subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Rozwiązywanie problemów z błędami za pomocą usługi Azure Resource Manager**

Zapoznaj się z poniższymi artykułami, aby dowiedzieć się więcej o niektórych typowych błędach wdrażania platformy Azure i uzyskać informacje na ich temat. Jeśli nie możesz znaleźć kodu błędu dla błędu wdrożenia, zobacz [Znajdowanie kodu błędu.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Rozwiązywanie problemów z błędami wdrażania](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Rozwiązywanie problemów z przenoszeniem zasobów platformy Azure do nowej grupy zasobów lub subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Zwróć uwagę, że jeśli chcesz uaktualnić subskrypcję platformy Azure, na przykład przełączyć się z bezpłatnej usługi na płatność na czas, konieczne będzie przekonwertowanie subskrypcji.

- Aby uaktualnić bezpłatną wersję próbną, zobacz Uaktualnianie bezpłatnej wersji próbnej lub subskrypcji platformy Microsoft Imagine Azure do wersji [Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Aby zmienić konto w usłudze Pay-as-you-go, zobacz Zmienianie subskrypcji usługi [Azure Pay-As-You-Go na inną ofertę.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Aby dodać lub skojarzyć subskrypcję platformy Azure z Azure Active Directory dzierżawy:**

1. Zaloguj się i wybierz subskrypcję, której chcesz używać, na stronie [Subskrypcje w Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Wybierz **pozycję Zmień katalog**.
3. Przejrzyj wyświetlone ostrzeżenia, a następnie wybierz pozycję **Zmień**.
4. Katalog zostanie zmieniony dla subskrypcji i zostanie wyświetlony komunikat o sukcesie.
5. Użyj *przełącznika* katalogu, aby przejść do nowego katalogu. Poprawne wyświetlanie wszystkich danych może potrwać do 10 minut.

**Zalecane dokumenty**

- [Przenoszenie własności subskrypcji platformy Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Przenoszenie zasobów do nowej grupy zasobów lub subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Zarządzanie zasobami za pomocą portalu Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
