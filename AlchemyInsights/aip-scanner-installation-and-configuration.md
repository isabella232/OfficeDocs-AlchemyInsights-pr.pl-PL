---
title: 'Skaner AIP: instalacja i konfiguracja'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358103"
---
# <a name="aip-scanner-installation-and-configuration"></a>Skaner AIP: instalacja i konfiguracja

**Aby zainstalować skaner AIP, postępuj zgodnie z zalecanymi wytycznymi:**

1. Jeśli uaktualniasz i nie wykonujesz czystej instalacji, upewnij się, że przestrzegałeś wskazówek dotyczących [uaktualniania skanera usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) i ujednoliconego klienta etykietowania, zobacz [uaktualnianie skanera usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Sprawdź, czy są zgodne ze [wszystkimi zapory i wymagania dotyczące ustawień infrastruktury sieciowej](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Upewnij się, że [zasady są ustawione](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatyczne etykietowanie lub mają domyślną etykietę w zasadach.
4. Upewnij się, że odpowiedni typ pliku jest skonfigurowany pod kątem etykiety/ochrony zgodnie z opisem w [obszarze Typy plików obsługiwane przez klienta usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Ponadto, jeśli chcesz zmienić zachowanie domyślne, postępuj zgodnie z tymi wskazówkami: [Zmiana domyślnego poziomu ochrony plików](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Sprawdź, czy konto użytkownika skonfigurowane do uruchamiania usługi skanera ma uprawnienia dostępu do wszystkich skonfigurowanych repozytoriów.
6. Jeśli nadal występują problemy, wyeksportuj dzienniki skanera i dodaj je do biletu pomocy technicznej.

**Eksportowanie dzienników skanera ochrony informacji platformy Azure**

1. Przejdź do %localappdata%\Microsoft\MSIP w kontekście użytkownika z uruchomieniem usługi skanera.
2. Siąz całą zawartość w folderze MSIP.
3. Zapisz dzienniki w wybranej lokalizacji i dołącz je do żądania usługi.
4. Można również użyć [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Aby uzyskać dodatkowe informacje, zobacz:**
- [Wdrażanie skanera usługi Azure Information Protection w celu automatycznego klasyfikowania i ochrony plików](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Określanie i używanie parametru Token dla set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Uruchamianie cyklu odnajdowania i wyświetlanie raportów dla skanera](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Zapoznaj się z dokumentacją usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Wymagania dotyczące usługi Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Pobierz klienta usługi Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
