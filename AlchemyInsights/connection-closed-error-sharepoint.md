---
title: Błąd połączenia bazowego został zamknięty w SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233436"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Błąd "Połączenie podstawowe zostało zamknięte" w SharePoint

Jeśli w programie SharePoint jest wyświetlany komunikat o błędzie "Połączenie podstawowe zostało zamknięte", może to być związane z wymuszeniem wartości TLS 1.0/1.1. Aby uzyskać więcej informacji, zobacz następujące artykuły:

- [Przygotowanie do protokołu TLS 1.2 w usłudze Office 365 i usłudze Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Błędy uwierzytelniania występują, jeśli klient nie obsługuje protokołu TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Jeśli użytkownicy mają Windows 7, upewnij się, że sprawdzają pakiety [TLS Cipher Suites](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)w Windows 7.