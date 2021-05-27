---
title: Reguły ograniczania powierzchni ataków
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676438"
---
# <a name="attack-surface-reduction-rules"></a>Reguły ograniczania powierzchni ataków

Wykluczenie plików lub folderów może znacznie zmniejszyć ochronę zapewnianą przez reguły ograniczania powierzchni ataków. Pliki, które zostałyby zablokowane przez regułę, mogą być uruchamiane i nie są rejestrowane żadne raporty ani zdarzenia. Wszystkie reguły, które zezwalają na wykluczenia, mają zastosowanie wyłączenie.

Wykluczenia asr mają taką samą składnię jak Program antywirusowy Microsoft Defender wykluczeń. Aby uzyskać szczegółowe informacje, [zobacz Konfigurowanie i weryfikowanie](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)wykluczeń Program antywirusowy Microsoft Defender skanowania. Aby uniknąć problemów, przejrzyj [typowe błędy, których można uniknąć podczas definiowania wykluczeń.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Nie wszystkie reguły asr obsługują wykluczenia. Aby sprawdzić, czy reguła obsługuje wykluczenia, zobacz tabelę Reguły ograniczania powierzchni [ataków.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Reguły ograniczania powierzchni ataków

Miejsce ataków twojej organizacji obejmuje wszystkie miejsca, w których atakujący może naruszonć urządzenia lub sieci organizacji. Zmniejszenie powierzchni ataków oznacza ochronę urządzeń i sieci organizacji, co pozostawia atakującym mniej sposobów przeprowadzania ataków. Konfigurowanie reguł ograniczania powierzchni ataków w programie Microsoft Defender dla punktu końcowego może być pomocne.

Aby uzyskać więcej informacji, zobacz:

- [Mapuj identyfikator GUID reguły ASR na nazwę](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Wymagania dotyczące reguł asr:
    - [Windows 10 Pro, wersja 1709 lub nowsza](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, wersja 1709 lub nowsza](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, wersja 1803 (półroczny kanał) lub nowsza](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Określ prawidłowe wyłączenie, które ma być stosowane

1. W dzienniku firmy Microsoft-Windows-Windows Defender/operacyjnym poszukaj Windows-1121 lub 1122.

1. Oceń scenariusz blokowy i kontekst oraz potwierdź, że należy odblokować ten scenariusz.

1. Odczytaj wartość Path (Ścieżka) w szczegółach zdarzenia, czyli wartość definiującą wykluczenie.
    - Należy jak najsądniej o wyjątku.
    - W razie potrzeby zastosuj symbol wieloznaczny (na przykład zamień zmienną użytkownika).

1. Zastosuj wykluczenie zgodnie z potrzebami twojego wdrożenia. Aby uzyskać szczegółowe informacje, [zobacz Dostosowywanie reguł zmniejszania powierzchni ataków.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Wykluczenie nie jest honorowane

1. Określanie, czy reguła obsługuje wykluczenia. Aby uzyskać szczegółowe informacje, [zobacz Reguły ograniczania powierzchni ataków.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Przejrzyj zastosowane wykluczenia i sprawdź, czy dane zdarzeń nie mają literówek lub symboli wieloznacznych, które są nieprawidłowo interpretowane. Aby uzyskać więcej informacji, zobacz [Obsługiwane typy wykluczeń.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. jeśli wpływ reguły na tę regułę jest zbyt wysoki, rozważ przeniesienie (wstecz) reguły do trybu inspekcji w celu przeprowadzenia dalszych sprawdzania poprawności. Aby uzyskać szczegółowe informacje, zobacz Jak działają funkcje [programu Microsoft Defender dla punktu końcowego w trybie inspekcji.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Zbierz dane pomocy technicznej, aby otworzyć sprawę pomocy technicznej, używając tego polecenia:
    
   ** MDEClientAnalyzer.cmd -v**

    Aby uzyskać więcej informacji, zobacz [Problemy z komputerami dołączania do programu Microsoft Defender dla punktów końcowych.](issues-with-onboarding-machines.md)
