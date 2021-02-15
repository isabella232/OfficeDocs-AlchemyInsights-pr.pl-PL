---
title: Pisanie zwrotne hasła nie działa
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243518"
---
# <a name="password-writeback-is-not-working"></a>Pisanie zwrotne hasła nie działa

**Mam problemy z konfiguracją zapisu hasła**

- Funkcja zwrotu hasła jest funkcją klasy premium.
- Upewnij się, że rozumiesz wymagania dotyczące licencjonowania:
  - W organizacji musi być przypisana co najmniej jedna licencja
  - **Tylko użytkownicy w chmurze** — dowolna płatna usługa Office 365 (O365) lub usługa Azure AD Basic
  - **Użytkownicy chmury i/lub** lokalni — Azure AD Premium P1 lub P2, Enterprise Mobility + Security (EMS) lub Secure Productive Enterprise (SPE)
    - Aby dowiedzieć się więcej o wymaganiach licencjonowania, zobacz Wymagania licencjonowania dotyczące samodzielnego resetowania hasła w [usłudze Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Masz co najmniej jedno konto administratora i jedno testowe konto użytkownika z jedną odpowiednią licencją.
- Aby działało, należy połączyć program Azure AD Connect Kontroler domeny podstawowym emulatorem hasła. Program Azure AD Connect można skonfigurować do używania klucza  podstawowego Kontroler domeny klikając prawym przyciskiem myszy właściwości łącznika synchronizacji usługi Active Directory, a następnie wybierając pozycję Skonfiguruj **partycje katalogowe.** W tym miejscu poszukaj sekcji **ustawień** połączenia kontrolera domeny i zaznacz pole wyboru "Użyj **tylko preferowanych kontrolerów domen".**
  > [!NOTE]
  > Jeśli preferowany kontroler domeny nie jest emulatorem pdc, program Azure AD Connect nadal będzie się kontaktował z tym kontrolerem w celu zapisu hasła.
- Resetowanie hasła zostało skonfigurowane i włączone w dzierżawie. Aby uzyskać więcej informacji, zobacz "Umożliwianie użytkownikom resetowania haseł usługi [Azure AD".](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Upewnij się, że konto administratora używane do włączania funkcji zapisu zwrotnego haseł jest kontem administratora chmury (utworzone w usłudze Azure AD, a nie w lokalnej usłudze AD)
- Masz jedno lub wielo lassowe wdrożenie lokalne usługi AD z zainstalowanymi najnowszymi pakietami Service Pack dla systemów Windows Server 2008 R2, Windows Server 2012 lub Windows Server 2012 R2
- Masz zainstalowane narzędzie Azure AD Connect i masz przygotowane środowisko usługi AD do synchronizacji z chmurą. Przed przetestowaniem zapisu hasła upewnij się, że najpierw ukończono pełne importowanie i pełną synchronizację z usług AD i Azure AD w programie Azure AD Connect.
- Aby dowiedzieć się więcej, zobacz, jak wykonać pełną synchronizację i [pełne importowanie w programie Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mam problem z łącznością zapisu zwrotnego haseł**

1. Pobieranie i włączanie najnowszej wersji programu [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracja zapory: Narzędzie Azure AD Connect (1.1.443 i więcej) będzie potrzebowało wychodzącego **dostępu HTTPS** do:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Zezwalaj na utrzymywanie bezczynnych połączeń przez co najmniej 2–3 minuty

**Nadal mam problemy z zapisem hasła**

- Jeśli nadal masz problemy, spróbuj wyłączyć i ponownie włączyć usługę odzyskiwania hasła w narzędziu Azure AD Connect
- Aby dowiedzieć się więcej, zobacz, jak [wyłączyć i ponownie włączyć funkcję zapisu hasła](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
