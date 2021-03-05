---
title: Informacje Exchange Server aktualizacji zabezpieczeń
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481948"
---
# <a name="about-exchange-server-security-updates"></a>Informacje Exchange Server aktualizacji zabezpieczeń

Firma Microsoft wydała serię krytycznych aktualizacji zabezpieczeń dla Exchange Server lokalnych. Wersje serwerów, których dotyczy problem, to wszelkie poziomy aktualizacji Exchange Server 2010, 2013, 2016 i 2019. Nie ma to wpływu na usługę Exchange Online, ale jeśli masz niektóre lokalne serwery programu Exchange z powodu konfiguracji hybrydowej, są one potencjalnie narażone.

Aby zaktualizować serwery lokalne, muszą być uruchomione co najmniej następujące wersje programu Exchange:

- Exchange 2010 z dodatkiem Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 CU 19 lub CU 18
- Exchange Server 2019 CU 8 lub CU 7

Zobacz poniższe ogłoszenie dotyczące lokalizacji poprawek: Wydano: marzec [2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901) r. Exchange Server aktualizacji zabezpieczeń

**Ważne uwagi:**

Instalacja aktualizacji nie będzie działać, jeśli na serwerach lokalnych nie są uruchomione wymagane wersje programu Exchange, zgodnie z listą powyżej.

W przypadku ręcznego instalowania aktualizacji zapoznaj się z sekcją "Znane problemy" artykułów z bazy wiedzy dotyczących aktualizacji, aby uzyskać ważne informacje. Aktualizacje zabezpieczeń MUSZĄ być uruchamiane z poziomu wiersza polecenia CMD/PowerShell z podwyższonym poziomem uprawnień!
