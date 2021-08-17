---
title: Narzędzie do diagnostyki usługi dla Windows pulpitu wirtualnego
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052396"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Narzędzie do diagnostyki usługi dla Windows pulpitu wirtualnego

Windows Pulpit wirtualny (WVD) oferuje narzędzie diagnostyczne, które pozwala administratorom identyfikować błędy za pomocą jednego interfejsu. To narzędzie rejestruje informacje diagnostyczne za każdym razem, gdy WVD jest używane przez osobę z przypisaną rolą WVD. Każdy dziennik zawiera informacje o roli WVD biorącej udział w działaniu, komunikaty o błędach wyświetlane w trakcie sesji oraz informacje o dzierżawie i użytkowniku. Usługę Azure Log Analytics można skonfigurować do przechwytywania dziennika aktywności utworzonego za pomocą narzędzia diagnostycznego. W tym celu wykonaj następujące czynności:

1. Utwórz obszar roboczy analizy dziennika za pomocą [portalu Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Połączenie Windows komputerów do programu Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Uzyskaj identyfikator obszaru roboczego i klucz podstawowy obszaru roboczego. Kreator konfiguracji potrzebuje tych informacji do poprawnego skonfigurowania agenta i zapewnienia komunikacji z monitorem Azure.
1. [Wypychanie danych diagnostycznych do obszaru roboczego](https://go.microsoft.com/fwlink/?linkid=2128284). Możesz wypychać dane diagnostyczne z dzierżawy WVD do analizy dziennika dla swojego obszaru roboczego.
1. [Identyfikowanie i diagnozowanie problemów](https://go.microsoft.com/fwlink/?linkid=2128338) wewnętrznych lub zewnętrznych w odniesieniu do WVD.

Aby dowiedzieć się więcej o konfigurowaniu narzędzia diagnostyki usługi dla funkcji WVD, zobacz Używanie analizy dziennika [dla funkcji diagnostyki.](https://go.microsoft.com/fwlink/?linkid=2128084)
