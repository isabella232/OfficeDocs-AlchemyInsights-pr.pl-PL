---
title: 1332 OWA - reguł skrzynki odbiorczej są nie może być wykonane dla skrzynki pocztowej
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555783"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Reguły skrzynki odbiorczej nie działa zgodnie z oczekiwaniami

Sprawdź następujące ustawienia w programie Outlook w sieci web:

- Wiadomości mogą być przekierowane, przekazany został lub odpowiedzi automatycznie na podstawie reguł skrzynki odbiorczej tylko jeden raz. Trwa przeadresowanie reguła (reguła skrzynki odbiorczej lub reguły przepływu poczty, znany również jako reguły transportu) można dodać maksymalnie dziesięć adresatów przekazywanie do wiadomości. Aby uzyskać więcej informacji zobacz [ograniczenia reguły dziennika, transportu i skrzynki odbiorczej](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Reguły skrzynki odbiorczej nie działają na Skrzynka pocztowa dziennika alternatywny. Aby uzyskać więcej informacji o skrzynce pocztowej rejestrowanie alternatywny zobacz [Skrzynka pocztowa dziennika alternatywny](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Aby rozwiązać te problemy, zobacz [KB 2829319](https://support.microsoft.com/kb/2829319).

Jeżeli nie stosuje się poprzednie wydania, uruchom raport diagnostyczny reguły skrzynki odbiorczej przed zgłosić ten problem firmie Microsoft Support:

1. Otwieranie skrzynki pocztowej w programie Outlook w sieci web, a następnie kliknij przycisk <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Ustawienia** > **wyświetlić wszystkie ustawienia programu Outlook** > **korespondencji** > **zasady**.

2. U dołu strony kliknij przycisk **Jeśli reguły nie działają kliknij tutaj, aby wygenerować raport diagnostyczny**.
