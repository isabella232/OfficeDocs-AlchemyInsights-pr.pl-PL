---
title: Nie można aktywować pakietu Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928379"
---
# <a name="unable-to-activate-office"></a>Nie można aktywować pakietu Office

**Uwaga:** Jeśli korzystasz ze starszej wersji programu Windows (na przykład Windows 7), upewnij się, że domyślną obsługą jest TLS 1.2. Aby uzyskać więcej informacji, zobacz Aktualizowanie w celu włączenia [protokołów TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako domyślnych protokołów bezpiecznego w winieHTTP w Windows.

- Sprawdź, czy stan Twojej subskrypcji wskazuje, że upłynęła jej ważność.
- Upewnij się, że masz subskrypcję zezwalającą na licencje klienta, np. Office 365 Business lub Business Premium, oraz [upewnij się, że użytkownik ma przypisaną licencję](/microsoft-365/admin/manage/assign-licenses-to-users).
- Upewnij się, że użytkownik loguje się do pakietu Office za pomocą tego samego konta, do którego jest przypisana licencja.
- Sprawdź [stronę kondycji usługi Office 365](/office365/enterprise/view-service-health), aby zobaczyć, czy opisano na niej znane problemy z tą usługą.
- Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu aplikacji platformy Microsoft 365 do Internetu. Zobacz [Adresy URL i zakresy adresów IP usługi Office 365](/office365/enterprise/urls-and-ip-address-ranges "Adresy URL i zakresy adresów IP usługi Office 365").

**Porada** Na komputerach z systemem Windows możemy diagnozować i automatycznie rozwiązywać wiele typowych problemów z logowaniem do pakietu Office. Pobierz i uruchom  **[Asystenta odzyskiwania i pomocy technicznej dla usługi Office 365](https://aka.ms/SaRA-OfficeSignInScenario)**, aby skorzystać z naszego zautomatyzowanego narzędzia.

Wykonaj następujące czynności rozwiązywania problemów:

- Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników. [Usuń](/microsoft-365/admin/manage/remove-licenses-from-users) i [przypisz ponownie](/microsoft-365/admin/manage/assign-licenses-to-users) licencję pakietu Office, a następnie [zaloguj się do pakietu Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.
- Uruchamianie [narzędzia do rozwiązywania problemów z aktywacją](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Resetowanie stanu aktywacji pakietu Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Resetowanie stanu aktywacji pakietu Office")
- [Wykonywanie naprawy online pakietu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Aby poznać dodatkowe rozwiązania do rozwiązywania problemów, zobacz:  

- [Błędy „Produkt bez licencji” i błędy aktywacji w pakiecie Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Błąd „Niestety, nie można nawiązać połączenia z kontem. Spróbuj ponownie później” podczas aktywowania pakietu Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)