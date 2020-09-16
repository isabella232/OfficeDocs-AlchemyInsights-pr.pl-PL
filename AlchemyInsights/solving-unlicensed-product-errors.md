---
title: Rozwiązywanie problemów z błędami produktu bez licencji
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737963"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Sugestie dotyczące rozwiązywania problemów "produkt bez licencji"

Aby rozwiązać błędy dotyczące "produktu bez licencji", spróbuj wykonać następujące czynności:

- Sprawdź, czy Twój status abonamentu wygasł.
- Upewnij się, że masz abonament, który zezwala na licencje klienta, takie jak aplikacje Microsoft 365 dla firm lub Business Premium, i [upewnij się, że użytkownik ma przydzieloną licencję](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Upewnij się, że użytkownik loguje się do pakietu Office przy użyciu tego samego konta, do którego przypisano licencję.
- Sprawdź [stronę kondycja usługi](https://docs.microsoft.com/office365/enterprise/view-service-health) , aby sprawdzić, czy występują znane problemy z usługą.
- Sprawdź ustawienia zapory, oprogramowania antywirusowego i ustawień serwera proxy, aby upewnić się, że nie zablokują one aplikacji Microsoft 365 w celu uzyskania dostępu do Internetu. Zobacz [adresy URL i zakresy adresów IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Możesz również wypróbować następujące akcje rozwiązywania problemów: 

- Otwórz aplikację pakietu Office i [Wyloguj się](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z istniejących kont użytkowników. [Usuń](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [ponownie Przypisz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencję pakietu Office, a następnie [Zaloguj się do pakietu Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) przy użyciu konta użytkownika, którego dotyczy problem.
- Uruchom [Narzędzie do rozwiązywania problemów z aktywacją](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Zresetuj stan aktywacji pakietu Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Wykonaj naprawę online pakietu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Aby poznać dodatkowe rozwiązania do rozwiązywania problemów, zobacz: 

- [Błędy „Produkt bez licencji” i błędy aktywacji w pakiecie Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Błąd „Niestety, nie można nawiązać połączenia z kontem. Spróbuj ponownie później” podczas aktywowania pakietu Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)