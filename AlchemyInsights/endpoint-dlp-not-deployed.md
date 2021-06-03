---
title: Ochrona DLP punktu końcowego nie jest wdrożona na urządzeniu użytkownika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731591"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Ochrona DLP punktu końcowego nie jest wdrożona na urządzeniu użytkownika

Jeśli ustawienie zapobieganie utracie danych w punkcie końcowym (DLP, Endpoint data loss prevention) nie ma zastosowania do urządzenia użytkownika, potwierdź, że spełniasz następujące wymagania:

- Windows 10 x64 kompilacja 1809 lub nowszy jest instalowana na urządzeniu.
- Zainstalowany jest klient ochrony przed złośliwym oprogramowaniem w wersji 4.18.2009.7 lub nowszej.
- Urządzenie jest **jednym z** tych:
    
    - Azure Active Directory (Azure AD)
    - Dołączyć do hybrydowej usługi Azure AD
    - Zarejestrowano AAD

- Aby wymusić akcje zasad, upewnij się, że Chromium Microsoft Edge jest zainstalowana na urządzeniu końcowym.

Aby uzyskać dodatkowe wymagania dotyczące wdrażania ochrony przed utratą danych w punktach końcowych, zobacz Wprowadzenie do ochrony przed utratą danych [w punkcie końcowym.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)