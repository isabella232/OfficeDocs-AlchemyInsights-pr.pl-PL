---
title: Pisanie zwrotne haseł nie działa
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324933"
---
# <a name="password-writeback-is-not-working"></a>Pisanie zwrotne haseł nie działa

**Mam problemy z konfiguracją zapisu hasła**

- Pisanie hasła to funkcja premium.
- Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:
  - W organizacji musi być przypisana co najmniej jedna licencja
  - **Użytkownicy tylko w chmurze** — Office 365 płatnej wersji SKU usługi Microsoft (O365) lub Azure AD Basic
  - **Użytkownicy chmury i(lub)** lokalni — Azure AD — wersja Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
    - Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz Wymagania dotyczące licencjonowania dotyczące samodzielnego resetowania hasła [w usłudze Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Masz co najmniej jedno konto administratora i jedno konto użytkownika testowego z jedną odpowiednią licencją.
- Aby działało, należy połączyć usługę Azure AD Połączenie z Kontroler domeny Emulator podstawowym. Usługę Azure AD Połączenie w celu używania klucza podstawowego Kontroler domeny,  klikając prawym przyciskiem myszy właściwości łącznika synchronizacji usługi Active Directory, a następnie wybierając pozycję Skonfiguruj partycje **katalogu.** W tym miejscu poszukaj sekcji **ustawień** połączenia kontrolera domeny i zaznacz pole wyboru używaj tylko **preferowanych kontrolerów domen.**
    **Uwaga:Jeśli** preferowanym kontrolerem domeny nie jest emulator programu PDC, usługa Azure AD Połączenie nadal będzie out out to the PDC w celu pisania hasła.
- Resetowanie hasła zostało skonfigurowane i włączone w dzierżawie. Aby uzyskać więcej informacji, zobacz Umożliwianie użytkownikom [resetowania haseł usługi Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Upewnij się, że konto administratora używane do włączania funkcji zapisu hasła jest kontem administratora chmury (utworzone w usłudze Azure AD, a nie w lokalnej usłudze AD)
- Masz jedno lub wielolesiowe wdrożenie lokalne usługi AD z zainstalowanym programem Windows Server 2008 R2, Windows Server 2012 lub Windows Server 2012 R2 z zainstalowanymi najnowszymi pakietami Service Pack
- Zainstalowano narzędzie do synchronizacji usługi Azure AD Połączenie oraz przygotowane środowisko usługi AD do synchronizacji z chmurą. Przed przetestowaniem zapisu hasła, upewnij się, że najpierw ukończono pełne importowanie i pełną synchronizację z usług AD i Azure AD w usłudze Azure AD Połączenie.
- Aby dowiedzieć się więcej, zobacz, jak wykonać pełną synchronizację i [pełne importowanie w usłudze Azure AD Połączenie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mam problem z łącznością zapisu hasła**

1. Pobieranie i włączanie najnowszej wersji usługi [Azure AD Połączenie](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracja zapory: narzędzie Połączenie Azure AD (1.1.443 i wyżej) będzie potrzebowało dostępu **wychodzącego HTTPS** do:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Zezwalaj na bezczynne połączenia na czas co najmniej 2–3 minut

**Nadal mam problemy z zapisem hasła**

- Jeśli nadal masz trudności, spróbuj wyłączyć i ponownie w ramach narzędzia do zapisu hasła w narzędziu do Połączenie Azure AD
- Aby dowiedzieć się więcej, zobacz, jak wyłączyć i [ponownie włączyć funkcję zapisu hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
