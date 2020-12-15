---
title: Narzędzie do diagnostyki usług dla pulpitu wirtualnego systemu Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680227"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Narzędzie do diagnostyki usług dla pulpitu wirtualnego systemu Windows

Pulpit wirtualny systemu Windows (WVD) oferuje narzędzie diagnostyczne, które umożliwia administratorom identyfikowanie błędów za pośrednictwem jednego interfejsu. To narzędzie rejestruje informacje dotyczące diagnostyki, ilekroć WVD jest używana przez osobę, która przypisała rolę WVD. Każdy dziennik zawiera informacje dotyczące roli WVD, w której występują działania, komunikaty o błędach wyświetlane podczas sesji oraz informacje o dzierżawie i użytkowniku. Analiza dzienników Azure może być skonfigurowana do przechwytywania dziennika aktywności utworzonego przez narzędzie diagnostyczne. W tym celu wykonaj następujące czynności:

1. Tworzenie obszaru roboczego Analiza dzienników za pomocą [usługi Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) lub [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Połącz komputery z systemem Windows z usługą Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Pobierz identyfikator obszaru roboczego i klucz podstawowy obszaru roboczego. Kreator konfiguracji potrzebuje tych informacji, aby poprawnie skonfigurować agenta i umożliwić mu komunikację z usługą Azure Monitoring.
1. [Przekazywanie danych diagnostycznych do obszaru roboczego](https://go.microsoft.com/fwlink/?linkid=2128284). Możesz wypchnąć dane diagnostyczne od dzierżawy WVD do analizy dziennika w obszarze roboczym.
1. [Zidentyfikuj i Diagnozuj problemy](https://go.microsoft.com/fwlink/?linkid=2128338) , które są wewnętrzne lub zewnętrzne w stosunku do WVD.

Aby dowiedzieć się więcej o konfigurowaniu narzędzia diagnostycznego usługi dla WVD, zobacz [Korzystanie z funkcji diagnostycznej analizy dzienników](https://go.microsoft.com/fwlink/?linkid=2128084).
