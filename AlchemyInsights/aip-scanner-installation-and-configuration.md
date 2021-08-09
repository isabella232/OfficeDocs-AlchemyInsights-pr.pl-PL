---
title: 'Skaner AIP: instalacja i konfiguracja'
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
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934267"
---
# <a name="aip-scanner-installation-and-configuration"></a>Skaner AIP: instalacja i konfiguracja

**Aby zainstalować skaner AIP, postępuj zgodnie z zalecanymi wytycznymi:**

1. Jeśli uaktualniasz i nie wykonujesz czystej instalacji, upewnij się, że zostały przestrzegać wytycznych dotyczących uaktualniania skanera [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i ujednoliconego klienta etykiet, zobacz Uaktualnianie skanera Azure Information [Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Upewnij się, że są spełnione wszystkie wymagania dotyczące [zapór i infrastruktury sieci.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Upewnij się, [że zasady są ustawione na](https://docs.microsoft.com/azure/information-protection/configure-policy) etykiety automatyczne lub mają etykietę domyślną w zasadach.
4. Upewnij się, że odpowiedni typ pliku jest skonfigurowany do obsługi etykiet/ochrony zgodnie z opisem w tece Typy plików obsługiwane przez klienta [usługi Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Ponadto, jeśli chcesz zmienić zachowanie domyślne, postępuj zgodnie z tymi wskazówkami: [Zmienianie domyślnego poziomu ochrony plików.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Sprawdź, czy konto użytkownika skonfigurowane do uruchamiania usługi skanera ma uprawnienia dostępu do wszystkich skonfigurowanych repozytoriów.
6. Jeśli nadal masz problemy, wyeksportuj dzienniki skanera i dodaj je do biletu pomocy technicznej.

**Eksportowanie dzienników skanera informacji o usłudze Azure Information Protection**

1. W kontekście użytkownika z usługą skanera przejdź do lokalizacji %localappdata%\Microsoft\MSIP.
2. Spakuj całą zawartość w folderze MSIP.
3. Zapisz dzienniki w wybranej lokalizacji i dołącz je do zgłoszenia serwisowego.
4. Możesz również użyć funkcji [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Aby uzyskać dodatkowe informacje, zobacz:**
- [Wdrażanie programu Azure Information Protection w celu automatycznego klasyfikowania i chronienia plików](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Określanie i używanie parametru Token w celu uwierzytelniania Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Uruchamianie cyklu odnajdowania i wyświetlanie raportów dla skanera](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Przejrzyj dokumentację usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Wymagania dotyczące usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Pobierz klienta usługi Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
