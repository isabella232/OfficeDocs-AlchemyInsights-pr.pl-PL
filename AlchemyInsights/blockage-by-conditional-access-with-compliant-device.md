---
title: Dostęp warunkowy ze zgodnym urządzeniem jest blokowany
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036000"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Dostęp warunkowy ze zgodnym urządzeniem jest blokowany

**Wysoce zalecane narzędzia**

- [Narzędzie do rozwiązywania problemów z rejestracją](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) urządzeń — kompleksowe narzędzie, które ułatwia rozwiązywanie najczęstszych problemów z rejestracją urządzeń.
- [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — narzędzie służące do zapewnienia, że urządzenie może uzyskać dostęp do punktów końcowych rejestracji urządzeń za pomocą konta systemowego.
- [Skrypt oczyszczania urządzenia usługi Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) — narzędzie służące do wyszukiwania przestarzałych urządzeń i zarządzania nimi w środowisku.

Oto kilka typowych powodów, dla których dostęp warunkowy może nie posunie się w przypadku zgodnego urządzenia lub dlaczego użytkownicy otrzymują komunikat Nie można przejść z tego komunikatu podczas żądania logowania do zasobu organizacyjnego. 

1. **Urządzenie z usługą MDM nie jest w stanie wymaganym:**

Sprawdź, czy urządzenie zostało zarejestrowane za pomocą zatwierdzonego dostawcy MDM, takiego jak Intune, *i oznaczone jako zgodne.* Aby uzyskać więcej informacji o usłudze Intune, zobacz ten [dokument.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Aby lepiej zrozumieć zgodność urządzeń i usługę Intune, zobacz Ustawianie reguł dla urządzeń, które zarządzasz za pomocą usługi Intune, za pomocą zasad [zgodności.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Jeśli masz problemy z zarejestrowaniem urządzenia w usłudze Intune, zobacz Rozwiązywanie problemów z [rejestracją urządzenia w firmie Microsoft.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Aby uzyskać dalszą pomoc techniczną Intune, utwórz wniosek o pomoc techniczną. Aby to zrobić, odwiedź stronę [Pomoc i obsługa techniczna Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Urządzenie nie jest przyłączone do sieci organizacji:**

Aby uzyskać dostęp do zasobów organizacji, urządzenie musi być połączone z siecią organizacji za pośrednictwem bezpośredniego połączenia lub wirtualnej sieci prywatnej (VPN), a także dołączane do lokalnego lub usługi Azure Active Directory. Aby dołączyć urządzenie służbowe do sieci organizacji, zobacz Dołączanie urządzenia służbowego do [sieci organizacji.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Aby zarejestrować urządzenie osobiste/BYOD, zobacz Rejestrowanie urządzenia osobistego [w sieci organizacji.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Aby sprawdzić, czy urządzenie dołączyło do sieci, możesz wykonać tutaj instrukcje dotyczące zarejestrowanych urządzeń [lub](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) urządzeń [służbowych.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Aby zawęzać ten problem do łączności sieciowej organizacji, postępuj zgodnie z poniższymi wskazówkami:

    1. Zaloguj się do systemu Windows przy użyciu konta służbowego, na przykład alain@contoso.com.
    2. Połącz się z siecią organizacji przez sieć VPN lub DirectAccess.
    3. Po połączeniu naciśnij klawisze **logo Windows+L,** aby zablokować urządzenie.
    4. Odblokuj urządzenie przy użyciu konta służbowego, a następnie ponownie spróbuj uzyskać dostęp do problematycznej aplikacji lub usługi.

Jeśli ponownie pojawi się komunikat o błędzie Nie można **przejść** z tego miejsca, problem prawdopodobnie występuje w innym miejscu.

3. **System operacyjny nie jest obsługiwany:**

Upewnij się, że używasz obsługiwanej wersji systemu operacyjnego, na przykład:

- **Klient Windows:** Windows 7 lub nowszy

- **Windows Server:** Windows Server 2008 R2 lub nowszy

- **macOS:** macOS X lub nowszy

- **Android i iOS:** Najnowsza wersja systemów operacyjnych android i iOS dla urządzeń przenośnych

4. **Przeglądarka internetowa nie jest obsługiwana:**

Poniżej znajdziesz obsługiwane przeglądarki. W przypadku obsługi przeglądarki Chrome w systemie Windows 1703 lub nowszym wymagane jest rozszerzenie konta systemu Windows 10. W przypadku edge 85+, użytkownik musi być zalogowany, aby poprawnie przekazać informacje o zgodności urządzenia. Aby uzyskać więcej informacji, zobacz [tutaj](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1:** Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, przeglądarka zarządzana Intune, Safari
- **Android:** **Microsoft Edge:** przeglądarka zarządzana Intune, Chrome
- **Telefon Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Tutaj znajdziesz więcej informacji na **temat** procedury rozwiązywania problemów i komunikatu Nie można uzyskać do [tej wiadomości.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
