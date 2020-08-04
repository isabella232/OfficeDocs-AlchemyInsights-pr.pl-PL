---
title: Profile sieci Wi-Fi usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555316"
---
# <a name="intune-wi-fi-profiles"></a>Profile sieci Wi-Fi usługi Intune

Pomyślne wdrożenie łączności Wi-Fi dla klientów MDM zależy od poprawnie wdrożonego profilu, który odzwierciedla wymagania firmowej infrastruktury Wi-Fi. Aby przejrzeć odpowiednie ustawienia dla analizowych platform klienckich, zobacz: 

[Dodawanie ustawień sieci Wi-Fi dla urządzeń z systemem Android w usłudze Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Dodawanie ustawień sieci Wi-Fi dla urządzeń dedykowanych i w pełni zarządzanych systemu Android Enterprise w usłudze Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Dodawanie ustawień sieci Wi-Fi dla urządzeń z systemem iOS i iPadOS w usłudze Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Dodawanie ustawień sieci Wi-Fi dla urządzeń z systemem Windows 10 i nowszych w usłudze Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importowanie ustawień sieci Wi-Fi dla urządzeń z systemem Windows w usłudze Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Typowe problemy**

**Wdrażam profil sieci Wi-Fi zależny od wdrożonego certyfikatu określonego w profilu sieci Wi-Fi. Jednak profile konfiguracji są wyświetlane stan błędu.**

Sprawdź, czy urządzenie odebrało certyfikat.

1. W usłudze Intune przejdź do **opcji Wszystkie urządzenia** i wybierz **konfigurację urządzenia**> urządzenia .

2. Sprawdź, czy wszystkie oczekiwane profile są wymienione i w stanie pomyślnym.

3. W przypadku profilu systemu Android, jeśli masz certyfikaty pośrednie w łańcuchu certyfikatów, upewnij się, że są one wdrażane na urządzeniach z systemem Android.

    Aby sprawdzić stan certyfikatu, przejdź do **profili konfiguracji urządzenia**Android pośredni certyfikat urzędu  >  **Profiles**  >  **Android intermediate CA**  >  **certyfikacji.**  >  **Trusted Certificate**

Jeśli nadal widzisz błędy, przejrzyj procedury i sekcje rozwiązywania problemów. Aby uzyskać więcej informacji, zobacz [Omówienie rozwiązywania problemów z profilami certyfikatów SCEP za pomocą usługi Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Wdrożeniu profilu sieci Wi-Fi na urządzeniu. Usługa Intune pokazuje, że zakończyła się pomyślnie, ale urządzenie nie łączy się z siecią Wi-Fi.**

Pomyślny stan oznacza, że usługa Intune pomyślnie wdrożyła profil skonfigurowany. Jednak te konfiguracje mogą nie odpowiadać wymaganiom sieci i/lub uwierzytelniania. Aby uzyskać więcej informacji na temat próby połączenia, przejrzyj dzienniki w usłudze infrastruktury i uwierzytelniania (na kontrolerze punktu dostępu Wi-Fi i serwerze NPS/Radius). Może być nawiązywać współpraca z zespołem infrastruktury sieciowej lub dostawcą sieci Wi-Fi innej firmy w celu zbierania i przeglądania dzienników.