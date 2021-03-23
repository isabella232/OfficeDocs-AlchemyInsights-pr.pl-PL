---
title: Dostęp warunkowy z urządzeniem przyłączony do domeny jest blokowany
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038109"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Dostęp warunkowy z urządzeniem przyłączony do domeny jest blokowany

**Wysoce zalecane narzędzia**

[Narzędzie do rozwiązywania problemów z rejestracją](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) urządzenia — narzędzie, które pomaga w rozwiązywaniu najczęstszych problemów z rejestracją urządzenia.

[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — skrypt, który pomaga zapewnić, że urządzenie może uzyskać dostęp do punktów końcowych rejestracji urządzeń w ramach konta systemowego.

[Skrypt oczyszczania urządzenia usługi Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) — skrypt, który umożliwia szukanie przestarzałych urządzeń i zarządzanie nimi w środowisku.

Oto kilka typowych powodów, dla których dostęp warunkowy może powodować niepowodzenie działania urządzenia, które przyłączyło się do domeny (hybrydowa usługa Azure AD).

1. **Na urządzeniu nie ma narzędzia Azure AD PRT** — musisz się upewnić, że urządzenie ma token odświeżania podstawowego usługi Azure AD (PRT). Aby uzyskać więcej informacji na temat prt, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Aby sprawdzić, czy masz narzędzie Azure AD PRT, uruchom polecenie na urządzeniu i sprawdź, czy `dsregcmd/status` "AzureAdPrt" ma pozycję "YES".

Jeśli argument "AzureAdPrt" ma stan "NIE", sprawdź następujące kwestie:

- Niezależnie od tego, czy masz środowisko **federacyjnych** z usługami AD FS i jest to nieosiągalne w sieciach domowych użytkowników: W takim przypadku upewnij się, że punkty końcowe "nazwa_użytkownikamixed" są dostępne z ekstranetu. Jeśli usługi AD FS są za siecią VPN, upewnij się, że użytkownicy łączą się z siecią VPN i zalogują się ponownie na urządzeniu. Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Czy usługa TPM** urządzenia jest błędna, a zatem nie może uwierzytelnić urządzenia: sprawdź, czy moduł TPM ma stan "Gotowe". Jeśli nie, uruchom program i poczekaj, aby urządzenie ponownie `dsregcmd/leave` dołączyło do usługi Azure AD. Następnie spróbuj ponownie. Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Korzystasz z zewnętrznego** dostawcy tożsamości, który nie obsługuje WS-Trust protokołu . Jak opisano w naszych pracach, w tym przypadku hybrydowe urządzenia przyłączone do usługi Azure AD nie mogą działać. Skontaktuj się z dostawcą tożsamości, aby uzyskać pomoc techniczną.

2. Użytkownicy korzystają z przeglądarki Chrome bez kont systemu **Windows 10** lub rozszerzenia pakietu Office Chrome nie używają automatycznie prt na urządzeniach przyłączony do AAD lub przyłączony hybrydowych **—AAD:** Spowoduje to niepowodzenie wszystkich zasad dostępu warunkowego opartych na urządzeniu z wyświetlonym komunikatem o błędzie "Niezarejestrowane urządzenie". Aby prawidłowo używać przeglądarki Chrome, musisz zainstalować "Konta systemu Windows 10" lub "Rozszerzenie pakietu Office dla przeglądarki Chrome użytkowników" za pomocą programu SCCM lub Intune. Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Jeśli nie jest możliwe zdalne wypychanie rozszerzenia, powiadom użytkowników, aby ręcznie zainstalują jedno z powyższych rozszerzeń, aby uzyskać dostęp do aplikacji korzystających z dostępu warunkowego opartego na urządzeniach. Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Urządzenie zostało poprawnie sprzężenia hybrydowego usługi **Azure AD, ale** zostało przypadkowo usunięte lub wyłączone ze względu na zmiany synchronizacji w programie Azure AD Connect lub w portalu Azure: W takim przypadku obiekt urządzenia nie jest już rozpoznawany jako urządzenie w pełni sprzężenia, nawet jeśli stan "AzureAdJoined" i "PRT" są wyświetlane jako prawidłowe na urządzeniu.

Aby rozwiązać ten problem, uruchom na urządzeniach, których to dotyczy, i pozwól im ponownie dołączyć `dsregcmd/leave` do usługi Azure AD. Aby uzyskać więcej informacji, zobacz [ten dokument.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Jeśli twoje urządzenia znajdują się w aktualizacji systemu Windows 10, 1809, z serwerem proxy w sieci VPN/chmurze i widzą problemy z stanem "AzureAdPrt" lub dowolną aplikacją z problemem z logowaniem jednokrotnym (program Outlook nie łączy się ze skrzynką pocztową, mimo że był prT), upewnij się, że masz tę poprawkę [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) lub aktualizację skumulowaną z kwietnia [KB4549949,](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) aby zapobiec błędom PRT na tych komputerach.

















