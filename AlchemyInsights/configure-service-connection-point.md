---
title: Konfigurowanie punktu połączenia usługi (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037295"
---
# <a name="configure-service-connection-point-scp"></a>Konfigurowanie punktu połączenia usługi (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Przyczyna:** Nie można odczytać obiektu SCP i pobrać informacji o dzierżawie usługi Azure AD
- **Rozwiązanie:** zobacz sekcję [Konfigurowanie punktu połączenia usługi.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Plan działań**

- Sprawdź, czy urządzenie otrzymało regułę zasad grupy dla kontrolowanej weryfikacji.
- Upewnij się, że klucz rejestru został utworzony przez urząd zasad grupy.
- Upewnij się, że masz 2 klucze utworzone przy użyciu identyfikatora katalogu i domeny onmicrosoft.

**Konfigurowanie ustawienia rejestru po stronie klienta dla ustawienia SCP**

Użyj poniższego przykładu, aby utworzyć obiekt zasady grupy (GPO) w celu wdrożenia ustawienia rejestru, które konfiguruje wpis SCP w rejestrze urządzeń.

1. Otwórz konsolę zasady grupy zarządzania i utwórz nowy magazyn zasad grupy w swojej domenie.
     - Podaj nazwę nowo utworzonego klienta (na przykład ClientSideSCP)

2. Przeedytuj wpis zasad grupy i znajdź następującą ścieżkę: Konfiguracja **komputera > Preferencje > Windows > Rejestru.**

3. Kliknij prawym przyciskiem myszy **pozycję Rejestr i** wybierz > element **rejestru.**

4. Na **karcie Ogólne** skonfiguruj następujące opcje:
  
- **Akcja:** Aktualizacja
    
- **Gałąź:** HKEY_LOCAL_MACHINE
    
- **Ścieżka klucza:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nazwa wartości:** TenantId
    
- **Typ wartości:** REG_SZ
    
- **Dane wartości:** Identyfikator GUID lub identyfikator katalogu wystąpienia usługi Azure AD (tę wartość można znaleźć w portalu Azure Portal > właściwości usługi **Azure Active Directory > właściwości > katalogu)**
 
- Kliknij przycisk **OK**.
 
5. Kliknij prawym przyciskiem myszy **pozycję Rejestr i** wybierz > element **rejestru.**

6. Na **karcie Ogólne** skonfiguruj następujące opcje:
  
- **Akcja:** Aktualizacja
    
- **Gałąź:** HKEY_LOCAL_MACHINE
    
- **Ścieżka klucza:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nazwa wartości:** TenantName
    
- **Typ wartości:** REG_SZ
    
- **Dane wartości:** zweryfikowana nazwa domeny, jeśli korzystasz ze środowiska feder finansowego, takiego jak usługi AD FS. Zweryfikowana nazwa domeny lub onmicrosoft.com domeny (na przykład contoso.onmicrosoft.com, jeśli korzystasz ze środowiska zarządzanego)

- Kliknij przycisk **OK**.

7. Zamknij edytor nowo utworzonego edytora zasad grupy.

8. Połącz nowo utworzony zestaw zasad grupy z żądaną nazwą użytkownika zawierającą komputery przyłączone do domeny, które należą do twojej populacji kontrolowanego rzutowania.

Aby uzyskać więcej informacji, zobacz Kontrolowane sprawdzanie poprawności hybrydowego dołączania do [usługi Azure AD — usługa Azure AD | Dokumenty Microsoft i](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) rozwiązywanie problemów dotyczących urządzeń przyłącznych do hybrydowej  [usługi Azure Active Directory | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









