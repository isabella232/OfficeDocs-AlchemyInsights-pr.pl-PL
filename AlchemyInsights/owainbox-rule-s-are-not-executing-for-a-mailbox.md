---
title: 1332 OWA — reguły skrzynki odbiorczej nie są wykonywane dla skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040912"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Reguła skrzynki odbiorczej nie działa zgodnie z oczekiwaniami

Sprawdź następujące ustawienia w programie Outlook w sieci Web:

- Wiadomość może być przekierowywana, przesyłana dalej lub odpowiadana na nie automatycznie w oparciu o reguły skrzynki odbiorczej tylko raz. Reguła przekierowywania (reguła skrzynki odbiorczej lub reguła przepływu poczty, znana także jako reguła transportu) może dodać do wiadomości maksymalnie dziesięciu adresatów. Aby uzyskać więcej informacji, zobacz [Limity reguł dziennika, transportu i skrzynki odbiorczej.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Reguły skrzynki odbiorczej nie działają w alternatywnej skrzynce pocztowej dziennika. Aby uzyskać więcej informacji na temat alternatywnej skrzynki pocztowej dziennika, zobacz [Alternatywna skrzynka pocztowa dziennika.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Aby rozwiązać te problemy, zobacz [artykuł z bazy 2829319.](https://support.microsoft.com/kb/2829319)

Jeśli poprzednie problemy nie mają zastosowania, uruchom raport diagnostyczny reguł skrzynki odbiorczej przed eskalacją problemu do pomocy technicznej firmy Microsoft:

1. Otwórz skrzynkę pocztową w Outlook w sieci Web i kliknij przycisk <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Ustawienia**  >  **Wyświetl wszystkie Outlook Ustawienia**  >  **Poczta**  >  **Reguły.**

2. U dołu strony kliknij pozycję Jeśli reguły nie działają, kliknij tutaj, **aby wygenerować raport diagnostyczny**.
