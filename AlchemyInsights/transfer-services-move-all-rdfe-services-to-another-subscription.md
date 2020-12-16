---
title: Transfer usług — przenoszenie wszystkich usług frontonu reddog do innej subskrypcji
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692172"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer usług — przenoszenie wszystkich usług frontonu reddog do innej subskrypcji

**Przenoszenie zasobów**

Zasoby platformy Azure można przenieść do innej subskrypcji platformy Azure lub grupy zasobów w ramach tej samej subskrypcji za pomocą usługi Azure Portal, platformy Azure CLI, usługi Azure CLI lub interfejsu API usługi w celu przeniesienia zasobów.

Aby można było przenosić zasoby, zobacz:

- [Lista kontrolna przed przeniesieniem zasobów](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Usługi, które można przenosić](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Jak sprawdzić poprawność przeniesienia](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Przenoszenie wskazówek dotyczących usług](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Aby przenieść istniejące zasoby do innej grupy zasobów lub abonamentu, możesz skorzystać z następujących czynności:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Środowisko Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Usługa Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [INTERFEJS API USŁUGI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Samouczek: [przenoszenie zasobów platformy Azure do innej grupy zasobów lub subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Rozwiązywanie problemów z usługą Azure Resource Manager**

Zapoznaj się z poniższymi artykułami, aby dowiedzieć się więcej o typowych błędach wdrażania usługi Azure oraz otrzymywać informacje umożliwiające ich usunięcie. Jeśli nie możesz znaleźć kodu błędu dotyczącego błędu wdrażania, zobacz [Znajdowanie kodu błędu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Rozwiązywanie problemów z błędami wdrażania](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Rozwiązywanie problemów dotyczących przenoszenia zasobów platformy Azure do nowej grupy zasobów lub subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Pamiętaj, że jeśli chcesz uaktualnić subskrypcję platformy Azure, na przykład przełączenie się za darmo w celu płacenia na bieżąco, musisz przekonwertować abonament.

- Aby uaktualnić bezpłatny okres próbny, zobacz [uaktualnianie bezpłatnego okresu próbnego lub abonamentu Microsoft Wyobraźmy sobie na abonament na bieżąco](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Aby zmienić konto Płać na bieżąco, zobacz [Zmienianie abonamentu na usługę Azure Pay na bieżąco do innej oferty](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Aby dodać lub skojarzyć subskrypcję platformy Azure Active Directory:**

1. Zaloguj się i wybierz abonament, którego chcesz użyć, na [stronie Subskrypcje w portalu Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Wybierz pozycję **Zmień katalog**.
3. Przejrzyj wyświetlone ostrzeżenia, a następnie wybierz pozycję **Zmień**.
4. Po zmianie katalogu dla subskrypcji zostanie wyświetlony komunikat o powodzeniu.
5. Użyj przełącznika *katalogów* , aby przejść do nowego katalogu. Poprawne wyświetlanie wszystkich elementów może potrwać do 10 minut.

**Polecane dokumenty**

- [Przenoszenie własności subskrypcji platformy Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Przenoszenie zasobów do nowej grupy zasobów lub subskrypcji](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Zarządzanie zasobami za pomocą portalu Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
