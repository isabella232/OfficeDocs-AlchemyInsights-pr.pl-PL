---
title: Problemy z urządzeniami dołączającymi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141656"
---
# <a name="issues-with-onboarding-machines"></a>Problemy z urządzeniami dołączającymi

Mogą wystąpić problemy z komputerami dołączania do usługi MDATP. Jeśli masz dostęp do maszyny użytkownika końcowego, wykonaj następujące kroki:

1. Pobierz narzędzie diagnostyczne [analizatora łączności klienta.](https://aka.ms/mdatpanalyzer)
2. Wyodrębnij i uruchom plik MDATPAnalyzer.cmd.
3. Zlokalizuj dziennik diagnostyczny w folderze o nazwie MDATPClientAnalyzerResult, ten sam folder, w którym jest pobierane narzędzie Analizator.
4. Przejrzyj plik dziennika, MDATPClientAnalyzer.txt, aby znaleźć problemy z łącznością lub ustawieniami serwera proxy internetowego.