---
title: Czy chcesz zgłosić do firmy Microsoft spam fałszywie dodatni?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396625"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Masz normalne wiadomości oznaczone jako spam?

Może to być frustrujące, gdy legalna wiadomość e-mail trafia do folderu Wiadomości-śmieci lub do kwarantanny. Rozważmy te najbardziej typowe przyczyny wyników fałszywie dodatnich:

**Zastępowanie dzierżawy (najczęściej)** Działania naprawcze należy w pełni do Twojej kontroli.

Prześlij wiadomość na Microsoft 365 Defender celu analizy zasad i reguł, które mają wpływ na to; Szczegóły ponownie mogą być dostępne w ciągu kilku minut.
Przejrzyj lub zmodyfikuj odpowiednie zasady lub reguły. 

**Zastępowanie przez użytkownika końcowego (typowe)** Działania naprawcze należy w pełni do Twojej kontroli. 

Prześlij wiadomość na Microsoft 365 Defender celu analizy zasad i reguł, które mają wpływ na to; Szczegóły ponownie mogą być dostępne w ciągu kilku minut. 

Jeśli wiadomość została zablokowana, ponieważ została wysłana z adresu na liście zablokowanych nadawców użytkownika, nagłówki zawierają werdykt filtrowania spamu "SFV:BLK".

**Uwierzytelnianie poczty e-mail nadawców** Jest on częściowo w ramach Twojej kontroli nad rozwiązywaniem problemów.

Prześlij wiadomość, aby przeanalizować błędy uwierzytelniania poczty e-mail nadawcy w momencie dostarczania; wyniki są dostępne w ciągu dnia. 

Jeśli jesteś właścicielem infrastruktury wysyłania, sprawdź, jak ją dostosować do spf, DKIM i DMARC, aby upewnić się, że docelowe systemy poczty e-mail zaufają wiadomościom wysyłanym z Twojej domeny. Możesz również skontaktować się z nadawcami, aby rozwiązać ich konfiguracje DNS.

**Werdykty filtrowania w firmie Microsoft** Jest on częściowo w ramach Twojej kontroli nad rozwiązywaniem problemów.

Prześlij wiadomość i zgłoś jako bezpieczną; Ponownie mogą być dostępne wyniki w ciągu dnia. Użyj listy zablokowanych/zezwalających na dzierżawę, jeśli nie zgadzasz się z werdyktami filtrowania w określonych sytuacjach. Nie należy jednak trwale pomijać werdyktów filtrowania firmy Microsoft. 

Więcej informacji można znaleźć w następujących artykułach:

- Umożliwia użytkownikom końcowych przesyłanie wiadomości do firmy Microsoft. Firma Microsoft używa tych przesyłania w celu poprawy skuteczności technologii ochrony poczty e-mail i pojawia się w raportach przesyłania, które mogą być używane jako wskaźnik do aktualizowania zasad. 

- Aby obejrzeć krótki klip wideo na temat przesyłania wiadomości do analizy, zobacz [Przesyłanie wiadomości do analizy.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Przesyłanie administratorów w celu przesyłania podejrzeń o spam, wyłudzy, adresy URL i pliki do firmy Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Zarządzanie listą zezwalania/blokowania dzierżawy](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Nagłówki wiadomości w programie Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Ochrona przed spamem ruchu wychodzącego w uceniu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)