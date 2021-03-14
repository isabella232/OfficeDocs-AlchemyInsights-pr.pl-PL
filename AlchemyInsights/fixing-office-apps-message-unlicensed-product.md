---
title: Nie można aktywować pakietu Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704940"
---
# <a name="unable-to-activate-office"></a>Nie można aktywować pakietu Office

- Sprawdź, czy stan Twojej subskrypcji wskazuje, że upłynęła jej ważność.
- Upewnij się, że masz subskrypcję zezwalającą na licencje klienta, np. Office 365 Business lub Business Premium, oraz [upewnij się, że użytkownik ma przypisaną licencję](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Upewnij się, że użytkownik loguje się do pakietu Office za pomocą tego samego konta, do którego jest przypisana licencja.
- Sprawdź [stronę kondycji usługi Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health), aby zobaczyć, czy opisano na niej znane problemy z tą usługą.
- Sprawdź ustawienia zapory, oprogramowania antywirusowego i serwera proxy, aby upewnić się, że nie blokują one dostępu aplikacji platformy Microsoft 365 do Internetu. Zobacz [Adresy URL i zakresy adresów IP usługi Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Adresy URL i zakresy adresów IP usługi Office 365").

**Porada** Na komputerach z systemem Windows możemy diagnozować i automatycznie rozwiązywać wiele typowych problemów z logowaniem do pakietu Office. Pobierz i uruchom  **[Asystenta odzyskiwania i pomocy technicznej dla usługi Office 365](https://aka.ms/SaRA-OfficeSignInScenario)**, aby skorzystać z naszego zautomatyzowanego narzędzia.

Wykonaj następujące czynności rozwiązywania problemów:

- Otwórz aplikację pakietu Office i [wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników. [Usuń](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [przypisz ponownie](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencję pakietu Office, a następnie [zaloguj się do pakietu Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.
- Uruchamianie [narzędzia do rozwiązywania problemów z aktywacją](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Resetowanie stanu aktywacji pakietu Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Resetowanie stanu aktywacji pakietu Office")
- [Wykonywanie naprawy online pakietu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Aby poznać dodatkowe rozwiązania do rozwiązywania problemów, zobacz:  

- [Błędy „Produkt bez licencji” i błędy aktywacji w pakiecie Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Błąd „Niestety, nie można nawiązać połączenia z kontem. Spróbuj ponownie później” podczas aktywowania pakietu Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)